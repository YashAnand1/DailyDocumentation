# Daily Updates
## 02 SEPTEMBER, 2023
## Reached Office: 9:10AM

# Tasks performed:
- ADDED "Please enter correct key" if wrong key is entered in the get code..
- Learnt that we cannot assign nil to strings - have to use "".
- Implemented strings.ToUpper in create.go.
- Discussion from Anoop Sir's meeting: XLSX Sheet & create.go code.
- - create a vm, where the server program (etcd-inventory) will be running, connect with it from host where the client program (itldims) will be. Remove etcd data from client machine. config file to be create for client program, which will be containing content such as ip address. 
- - create specific sheets for deployment - kubectl output should not be mimicked and should only be similar in the form of displayed output as existing sheet needs to provide more information.
- Gained basic understanding of KVM
- Created a VM using Ubuntu 23.04 iso image - followed steps from [Server-World](https://www.server-world.info/en/note?os=Ubuntu_23.04&p=kvm&f=1)
- Learnt how to remove a value from a slice using this [tutorial](https://www.youtube.com/watch?v=931nR5TGCAk&list=PLRAV69dS1uWQGDQoBYMZWKjzuhCaOnBpa&index=15&pp=iAQB)
- Understood more about ssh - watched this [tutorial](https://www.youtube.com/watch?v=qWKK_PNHnnA&pp=ygULd2hhdCBpcyBzc2g%3D) and read this [article](https://fostips.com/enable-ssh-ubuntu-21-04/)
- SSH'd using:
```
sudo apt install ssh
sudo apt openssh-server
systemctl start sshd.service
systemctl status sshd.service
ssh username@remote_server_ip
scp -P 1234 username@remote_server_ip:/PATH/TO/FILE ./ //for remote to local
scp -P 1234 /PATH/TO/FILE username@remote_server_ip:~/ // for local to remote
```
- faced issue with `Failed to start sshd.service: Unit sshd.service not found.` - because was not asked to in the article
- Also worked on understanding systemctl and what it does
