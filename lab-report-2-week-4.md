## **Code Change 1**

[Code change 1](https://github.com/PaulLai1022/markdown-pharse/commit/b94741697c42c1ab8c0a5d2e18b603a49566b275)

<img width="1216" alt="Screen Shot 2022-05-02 at 1 59 50 PM" src="https://user-images.githubusercontent.com/71100835/166326789-b3f6886b-0c64-458f-bf65-3b2915dadfe1.png">

[File for failure inducing input1](https://PaulLai1022.github.io/markdown-pharse/test-file.md)

***The symptoms shown for input1***
<img width="882" alt="Screen Shot 2022-05-02 at 2 05 54 PM" src="https://user-images.githubusercontent.com/71100835/166327708-b0ad3a52-5334-4e7f-9984-1ab523996835.png">

**Description**
So the first error we fix is while the EOF is a \n by adding a if statement for the openParen that if we couldn't find it we break it. This bug has caused lots of issues among the whole class so we decide to fix it first. 

## **Code Change 2**
[Code change 2](https://github.com/PaulLai1022/markdown-pharse/commit/601a5bd784e933d55373b318d3084bea8ed447ca)

<img width="1220" alt="Screen Shot 2022-05-02 at 2 07 50 PM" src="https://user-images.githubusercontent.com/71100835/166327944-ed613000-08c6-4b2e-86d4-bbe22fa6a79d.png">

[File for failure inducing input2](https://PaulLai1022.github.io/markdown-pharse/test-file1.md)

***The symptoms shown for input1***
<img width="975" alt="Screen Shot 2022-05-02 at 2 08 56 PM" src="https://user-images.githubusercontent.com/71100835/166328107-722fe23d-c17a-4809-a4a1-26dc6d1840c6.png">

**Description**
So bascially we input a image file in our tester file, which shall not be shown in the output, but as you can see in the symptoms screen shot we can witness that the image file still printed out by the computer, which is not the expected output .

## **Code Change 3**
