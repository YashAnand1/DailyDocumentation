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
sudo apt install openssh-server
systemctl start ssh
systemctl status ssh
systemctl enable ssh
ssh yashanand@192.168.122.128
Entered VM's IP and then password after saying yes i want to continue connecting.
scp -r /home/user/yes1/yes1/etcd-inventory yashanand@192.168.122.128:/home/yashanand/ //local to remote
scp -r (recursively/This flag is necessary when you want to copy entire directories and all their contents to the specified destination.) <file path on local> <remoteuser@remoteip>:pathwherecontenttobesaved
```
- faced issue with `Failed to start sshd.service: Unit sshd.service not found.` after running systemctl status sshd.service - because was not asked to in the article. even after installing openssh-server, faced same issue. Used systemctl status ssh and was shown ssh.service was
- `ssh.service - OpenBSD Secure Shell server  Loaded: loaded (/lib/systemd/system/ssh.service; disabled` displayed - solved using `sudo systemctl enable ssh`
- Also worked on understanding systemctl and what it does
