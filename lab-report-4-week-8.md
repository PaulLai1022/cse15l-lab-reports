- snippet preview on vscode
<img width="1081" alt="Screen Shot 2022-05-29 at 5 12 46 PM" src="https://user-images.githubusercontent.com/71100835/170897204-8e82f29c-2860-4a0a-b57b-97f8d16a6026.png">
<img width="1089" alt="Screen Shot 2022-05-29 at 5 13 11 PM" src="https://user-images.githubusercontent.com/71100835/170897220-12ef0e57-57ae-4fa5-9e53-2ad27fcce143.png">
<img width="1093" alt="Screen Shot 2022-05-29 at 5 13 25 PM" src="https://user-images.githubusercontent.com/71100835/170897233-bcacd46c-0603-4818-a694-973c932e530c.png">

- the expecte output


- MarkdownParseTest.java: tests for snippets
<img width="966" alt="Screen Shot 2022-05-30 at 11 54 55 AM" src="https://user-images.githubusercontent.com/71100835/171047598-99a8bb11-199f-4155-9b42-c03abfc74988.png">

- Output Failures
<img width="574" alt="Screen Shot 2022-05-30 at 11 53 56 AM" src="https://user-images.githubusercontent.com/71100835/171047491-43801689-2a40-44d6-a186-5098ddc6ada5.png">

---
# Answer to Question
**Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.**
- I think one possible soltion is to fix the code in MarkdownParse.javac via ignoring the characters bewteen the two backticks or from a backtick until the line ends. In this case, we are able to avoid the no-needed open bracket for example in line 1 and the no-needed end bracket at line 7, which will allow the program to detect the expected output ucsd.edu becase the second right endbracket is recognized. 

**Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.**
- I feel like the solution for a.com(()) is to have a count to cound the number of open and close bracket, and at the end we would be able to print all them out if the cnt is a even number. And the solution for the example.com test case is to search for "](" instead of doing the search separately. In thise case, we would be able to skip the no-needed end bracket in line 5, which ]( would be able to recognized and the example.com will be included in the following output. 

**Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.
- As we look in to the code, we could witness that the iteration of the loop in MardownParse stops when any text and line is found betwen the open and close parenthesis. In this case, we would skip github and but twitter would stay. Moreover, my program could omit the line from returned which in ths case the format of the ouput would be more correct. 

**If your code already works on some/all test cases, include an explanation of what were the code changes that allowed the tests to pass.
- All of them failed lmaooo


