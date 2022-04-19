## Installing VScode
![vscode](https://user-images.githubusercontent.com/78109412/162640290-4018a46d-b6ab-41f3-bfdf-6d623e5cb3d7.JPG)
* Download the VScode installer from https://code.visualstudio.com/
* Run the installer and follow the install procedures

## Remotely Connecting 
![remote](https://user-images.githubusercontent.com/78109412/162641804-a06eff50-48aa-4fbb-a50e-9e84e24b43f1.JPG)
* Install OpenSSH Client and OpenSSH Server
* Run `ssh cs15lsp22zzz@ieng6.ucsd.edu` in VScode terminal, replacing 'zzz' with course account id
* Reset/set password for cs15lsp22 account

## Trying Commands
![commands](https://user-images.githubusercontent.com/78109412/162642220-2d67d414-ff65-4855-a0a7-a9128d9a014e.JPG)
* Run terminal commands such as `cd`, `ls`, `cp`, and `cat`
* Pass different arguments to see how the output changes

## Moving Files over SSH with scp
![scp](https://user-images.githubusercontent.com/78109412/162642531-896850f6-95c8-4699-8dcd-7725034cc7b9.JPG)
* Run `scp` to copy WhereAmI.java from local machine to SSH server
* Run `ssh` and `ls` to ensure the file has been copied

## Setting an SSH Key
![sshkey](https://user-images.githubusercontent.com/78109412/162643247-aa86d007-8b2c-446c-8a1a-cef00f6bc28d.JPG)
* Generate a SSH keys using ssh-keygen
* Specify the directory for where the generated files will be stored

![sshcopy](https://user-images.githubusercontent.com/78109412/162643252-9146fc81-9406-48bd-91d2-cccce300d747.JPG)
* Create .ssh directory on SSH server 
* Copy public key over from local machine using `scp`

## Optimizing Remote Running
![optimize](https://user-images.githubusercontent.com/78109412/162643778-b2af7360-3de9-4164-a0da-dbb4e6bc2981.JPG)
* Make a local edit to WhereAmI.java
* Run `scp` to move the locally edited file to SSH server
* Run `ssh` along with compiling and running WhereAmI.java

