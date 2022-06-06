# Week 10 Lab

## Method of Finding Test Files
> The script.sh file was edited to print out each file that was being filed before returning the output.
> Then, two results.txt files were created in the two separate directories of the markdown parsers that were being compared.
> Lastly, the vimdiff command was used to open the two results.txt files to compare the differences in output.

### Test Files
[Test File 1](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/17.md)

## Test File 1 (17.md)
* The shared implementation of markdown-parser produced the expected result.
* My own implement of markdown-parse produced the incorrect result.

### Shared Implementation Output
![test17](https://user-images.githubusercontent.com/78109412/172078159-46f02bb2-8749-40d8-8119-cc1c25708af6.JPG)

### Own Implementation Output
![test172](https://user-images.githubusercontent.com/78109412/172078303-4ce2b3f1-c007-4cdc-b633-cbfd915b4719.JPG)

### Expected Output
![expectedoutput17](https://user-images.githubusercontent.com/78109412/172078422-a6584e4f-8cb5-4510-bb2d-43c616defb24.JPG)
* Since there are no valid links along with missing parantheses and brackets, the output should be empty.

![codechange1](https://user-images.githubusercontent.com/78109412/172078779-654c0c1b-fadc-4bad-8e9f-d258862ef68d.JPG)
> Additional checks are needed for the opening and closing brackets separately. This code only checks that both brackets are missing.
> As a result, opening brackets are being added as there is no case that checks for the closing bracket.
