# Week 6 Lab

## Streamlining ssh Configuration
![sshconfig](https://user-images.githubusercontent.com/78109412/167325841-0f2fecdd-f169-4b6d-addb-8ed50d946b4b.JPG)
* Used VScode to create a config file in .ssh directory
* Set host name as ieng6 for ssh login

![part1](https://user-images.githubusercontent.com/78109412/167325986-6e3fdeec-3ff9-4fa9-9b56-84706533bda8.jpg)
* Login to remote server with new username through the command `ssh ieng6`

![scppart1](https://user-images.githubusercontent.com/78109412/167326105-d3727238-6bfb-4f7b-8a02-422a54ce70ca.JPG)
* Use `scp scptest.txt ieng6:~/` to copy scptest.txt to home directory

## Setup Github Access from ieng6
![publickey1](https://user-images.githubusercontent.com/78109412/167326340-61210001-e42c-4e96-9929-45b4555ec90d.JPG)
![publickey2](https://user-images.githubusercontent.com/78109412/167326355-2c652e13-8812-4a06-8021-ffcb5ee2023a.JPG)
* Public and private key is stored in \Users\kevin\.ssh as id_rsa.pub and id_rsa
* Public SSH key on GitHub titled as Personal Windows Computer

![part2](https://user-images.githubusercontent.com/78109412/167326669-54fe2c39-c7e2-4e1b-b95e-c6896b16f2e8.JPG)
* Made change to MarkdownParse.java
* Ran `git commit -m "adding a line` and `git push origin main` to update repository

![linkcommit](https://user-images.githubusercontent.com/78109412/167326825-de423660-5c44-437f-8203-085eaa499220.JPG)
* Commit reflected in GitHub repository 

## Copy whole directories with `scp -r`
![scppart3 1](https://user-images.githubusercontent.com/78109412/167327206-b75d5398-2093-4927-b05a-5154c7ecfa75.JPG)
* Recursively copy the entire markdown-parser directory using the command `scp -r . ieng6:markdown-parse`

![runtest](https://user-images.githubusercontent.com/78109412/167327559-5cbaa442-b348-4c34-9f91-ef9f04bc24ba.JPG)
* Compile and run MarkdownParseTest.java 

