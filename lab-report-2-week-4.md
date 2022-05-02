**Code Change 1**

[Code change 1](https://github.com/PaulLai1022/markdown-pharse/commit/b94741697c42c1ab8c0a5d2e18b603a49566b275)

<img width="1216" alt="Screen Shot 2022-05-02 at 1 59 50 PM" src="https://user-images.githubusercontent.com/71100835/166326789-b3f6886b-0c64-458f-bf65-3b2915dadfe1.png">

[File for failure inducing input1](https://PaulLai1022.github.io/markdown-pharse/test-file.md)

***The symptoms shown for input1***
<img width="882" alt="Screen Shot 2022-05-02 at 2 05 54 PM" src="https://user-images.githubusercontent.com/71100835/166327708-b0ad3a52-5334-4e7f-9984-1ab523996835.png">

**Description**
So the first error we fix is while the EOF is a \n by adding a if statement for the openParen that if we couldn't find it we break it. This bug has caused lots of issues among the whole class so we decide to fix it first. 

