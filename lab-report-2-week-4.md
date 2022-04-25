# Week 4 Lab

## Code Change 1
![codechange1](https://user-images.githubusercontent.com/78109412/165001314-3d81250e-1023-491c-a5cf-4e3e1bc28ade.JPG)
![failure1](https://user-images.githubusercontent.com/78109412/165001611-a9e6145c-5db3-4ad9-9925-ad790e6b185f.JPG)

[Failure-inducing input](https://github.com/kevinhu27/markdown-parser/blob/0f4e555c293ea2e5b9547dc9b0837cadd6ff48ff/test-file2.md)

> The bug is that the code does not have a way to handle missing closing parentheses. 
> The symptom is visible as an error, stating that the index is going out of bounds since the closing paranthesis is missing in the test file.
> To address the bug, an if-statement case is included to handle the missing paranthesis.

## Code Change 2
![codechange2](https://user-images.githubusercontent.com/78109412/165002266-30dbaa19-26ea-412d-9f01-c1e8d9ff459e.JPG)
![failure2](https://user-images.githubusercontent.com/78109412/165002340-18d7e28c-cfa7-4710-82d6-80accca475e3.JPG)

[Failure-inducing input](https://github.com/kevinhu27/markdown-parser/blob/823a0fb30f6442dfd02056509f882f26bf15e934/test-file3.md)

> The bug is that the code does not know how to properly handle missing opening parentheses.
> The sympton is shown as an unexpected output where everything prior to the closing parenthesis is included in the link.
> To address the bug, an if-statement is used to keep track of where the opening parenthesis is suppose to start. 

## Code Change 3
![codechange3](https://user-images.githubusercontent.com/78109412/165002842-ceeca49f-1e51-4801-8043-c2b9af95d0fb.jpg)
![failure3](https://user-images.githubusercontent.com/78109412/165002716-0a7e0eeb-6d78-479f-9a06-3eed9f3dee27.JPG)

[Failure-inducing input](https://github.com/kevinhu27/markdown-parser/blob/45af9c3ebad49f60da1648a8e9d1696cfe1180da/test-file4.md)

> The bug is that the code cannot handle the case where brackets to denote a link are missing. 
> The symptom is shown as an output where the entire contents of the file are considerd to be a single link.
> To address this bug, an if-statement is used to exit the while-loop in the case where there are no links present. 
