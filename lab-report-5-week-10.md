# Week 10 Lab

## Method of Finding Test Files
> The script.sh file was edited to print out each file that was being filed before returning the output.
> Then, two results.txt files were created in the two separate directories of the markdown parsers that were being compared.
> Lastly, the vimdiff command was used to open the two results.txt files to compare the differences in output.

### Test Files
[Test File 1](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/17.md)

[Test File 2](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/192.md)

## Test File 1 (17.md)
* The shared implementation of markdown-parser produced the expected result.
* My own implement of markdown-parse produced the incorrect result.

### Shared Implementation Output
![test17](https://user-images.githubusercontent.com/78109412/172078159-46f02bb2-8749-40d8-8119-cc1c25708af6.JPG)

### Own Implementation Output
![test172](https://user-images.githubusercontent.com/78109412/172078303-4ce2b3f1-c007-4cdc-b633-cbfd915b4719.JPG)

### Expected Output
![expectedoutput17](https://user-images.githubusercontent.com/78109412/172078422-a6584e4f-8cb5-4510-bb2d-43c616defb24.JPG)
> Since there are no valid links along with missing parantheses and brackets, the output should be empty. \n
> Expected output: []

### Implementation Issue
![codechange1](https://user-images.githubusercontent.com/78109412/172078779-654c0c1b-fadc-4bad-8e9f-d258862ef68d.JPG)
* Additional checks are needed for the opening and closing brackets separately. 
* This code only checks that both brackets are missing.
* As a result, opening brackets are being added as there is no case that checks for the closing bracket.

## Test File 2(192.md)
* The shared implementation produced the expected result.
* My own implementation did not product the expected result.

### Shared Implementation Output
![test192](https://user-images.githubusercontent.com/78109412/172079348-82f411d7-6319-49b5-bbb5-bad454887e3c.JPG)

### Own Implementation Output
![test1922](https://user-images.githubusercontent.com/78109412/172079381-2ecc3666-42a3-47fd-a904-7e3ea00de9f0.JPG)

### Expected Output
![expectedoutput192](https://user-images.githubusercontent.com/78109412/172079468-43ef9ad0-951c-4048-884b-4f9f62f652b5.JPG)
> There are no valid links as links should be contained within opening and closing parantheses. The output should be empty as a result.

### Implementation Issue
![codechange2](https://user-images.githubusercontent.com/78109412/172079775-6a5a8454-a2af-4216-b56b-b4da8407b5eb.JPG)
* The code only determines where the open and closing parantheses are suppose to be in the case that they are missing.
* However, if both are missing and there is no valid link, any code beyond the brackets will be considered a valid link.
* The code needs to be changed in order to return empty if both parantheses are not found for each line.

