# Assignment 1: Creating VM-based services with OpenStack

> [!NOTE]
> As I was having trouble connecting to the presistent VM using the Client VM in crownlabs, I connected from my machine through ssh. To be able to see openstack's web GUI, I ran the command `ssh -L 8080:localhost:80 -J bastion@ssh.crownlabs.polito.it crownlabs@VM_ADDRESS` and accessed `http://localhost:8080` on my browser.

## Section 2

To start, I log in to the admin dashboard and enable DHCP for the public subnets.
![enabling-dhcp](images/1.png)

Then, I have to make sure I am in the admin project.

![admin](images/2.png)