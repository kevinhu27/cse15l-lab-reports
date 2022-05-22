# Week 8 Lab
[MarkdownParser Repository](https://github.com/kevinhu27/markdown-parser)

[Reviewed MarkdownParser Repository](https://github.com/cynthia-bao/markdown-parser)

## Code Snippet 1
### Expected Output
![preview1](https://user-images.githubusercontent.com/78109412/169719020-c60ee21e-9402-491b-b1f5-2f3684194494.JPG)

### Test - Own Implementation
![test1](https://user-images.githubusercontent.com/78109412/169719089-22c8f81d-e6c4-4b82-a554-db90a9c9f52a.JPG)

### Test Result
![testresult1](https://user-images.githubusercontent.com/78109412/169719146-d55c9a87-4586-41cf-83cc-945f2d248304.JPG)

### Test - Reviewed Implementation
![testresult1b](https://user-images.githubusercontent.com/78109412/169719520-df44734b-9ab8-4bb2-912d-09b34498a1cc.JPG)

### Test Result
![test1b](https://user-images.githubusercontent.com/78109412/169719495-47f147fa-6539-4ef0-b4be-132bbca8f609.JPG)

> To handle backticks, a code change can be made to skip over them if they are found within the parantheses.
> Since URLs should never contain backticks, omitting them if they are found can be a possible solution.


## Code Snippet 2
### Expected Output
![preview2](https://user-images.githubusercontent.com/78109412/169719593-5f960885-c91e-4e07-90a8-7b53b1571f3b.JPG)

### Test - Own Implementation
![test2](https://user-images.githubusercontent.com/78109412/169719856-51bbf610-c0ca-4996-8e5f-1f3df281f197.JPG)

### Test Result
![testresult2](https://user-images.githubusercontent.com/78109412/169719902-62ca95d4-b068-44e9-8981-da4ef6800c46.jpg)

### Test - Reviewed Implementation
![test2b](https://user-images.githubusercontent.com/78109412/169720518-9f9e533b-bfd2-410b-a145-fd49de0d8f8a.JPG)


## Test Result
![testresult2b](https://user-images.githubusercontent.com/78109412/169720526-9d2dfa2a-0c03-43ea-ba40-9496248a6c38.JPG)

> In order to handle the nesting of links, the location of the parantheses would have to be accounted for.
> A possible code change would be to determine whether the link is located within brackets or parantheses and
> disregard extra parantheses found within where the link is supposed to be located.


## Code Snippet 3
### Expected Output
![preview3](https://user-images.githubusercontent.com/78109412/169720013-300b56a8-d19b-4cc2-8081-51f1038bc557.JPG)

## Test - Own Implementation
![test3](https://user-images.githubusercontent.com/78109412/169720389-e1b117d8-51b9-447c-a1dd-0e3f43d5ce54.JPG)

## Test Result
![testresult3](https://user-images.githubusercontent.com/78109412/169720410-7bc3e614-4310-4454-9cd4-0ebc59f0b626.JPG)

## Test - Reviewed Implementation
![test3b](https://user-images.githubusercontent.com/78109412/169720660-60e86150-648e-4c71-bd3b-1495846617e6.JPG)

## Test Result
![testresult3b](https://user-images.githubusercontent.com/78109412/169720664-00327146-7568-4d78-9a27-682dec15ab7e.JPG)

> A more involved change is required in order to output all of the correct links. 
> By having newlines and parantheses that do not close, it is difficult to determine where links start and end.
> Various changes will need to be made in order to account for this case.

