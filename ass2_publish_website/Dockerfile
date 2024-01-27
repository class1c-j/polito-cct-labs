# Get Hugo and build the website

FROM klakegg/hugo:latest AS build

WORKDIR /website

COPY . .

RUN hugo -v

# Get nginx and serve the website

FROM nginx:latest

# Move the created files to the new stage
COPY --from=build /website/public /usr/share/nginx/html 

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
