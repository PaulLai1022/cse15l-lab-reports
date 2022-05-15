- I can edit it through the text editior
<img width="679" alt="Screen Shot 2022-05-13 at 4 46 24 PM" src="https://user-images.githubusercontent.com/71100835/168402045-9cd46b21-b1bd-43b1-8b40-c9f2802e6a15.png">

- I can log in by using the only ieng6 
<img width="566" alt="Screen Shot 2022-05-13 at 4 50 12 PM" src="https://user-images.githubusercontent.com/71100835/168402212-70fa2ffd-c120-452c-bd0c-066e69bb37dc.png">

- I successfully upload the picture via alias
<img width="566" alt="Screen Shot 2022-05-13 at 6 28 14 PM" src="https://user-images.githubusercontent.com/71100835/168405765-e9fc1b0f-69aa-4cbe-b450-3fccde22f6c9.png">

---
<img width="754" alt="Screen Shot 2022-05-14 at 5 05 06 PM" src="https://user-images.githubusercontent.com/71100835/168451949-1cf2d09c-2246-425a-9a1c-5edad7dc45d8.png">



---
I successfully copy the whole markdown-pharse director to my ieng6 account via using `scp -r markdown-parser cs15lsp22xxx@ieng6.ucsd.edu:.` and :. means I want it to go to the home director. 

<img width="698" alt="Screen Shot 2022-05-14 at 4 38 36 PM" src="https://user-images.githubusercontent.com/71100835/168451403-2e49baa4-e3b8-4fa3-8e16-399da0eb4098.png">

Then I log in via using `ssh ieng6`, and `cd` to my markdown-pharse directory and compile then run the test by using 
`javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar DemoPracTest.java`
`java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore xxx`
<img width="694" alt="Screen Shot 2022-05-14 at 4 43 34 PM" src="https://user-images.githubusercontent.com/71100835/168451494-b89ce90d-1ec3-4c1c-99f3-a48b2b67a346.png">

<img width="684" alt="Screen Shot 2022-05-14 at 4 43 44 PM" src="https://user-images.githubusercontent.com/71100835/168451496-1a9be9d2-e5fe-423d-9b63-88f8992e1716.png">

I initially started with the commend `scp -r markdown-pharse cs15lsp22avz@ieng6.ucsd.edu:.; ssh ieng6 "cd markdown-pharse;javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java;java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"` but the test ended up not compiling, so I latter on switch to the commend `scp -r markdown-pharse cs15lsp22avz@ieng6.ucsd.edu:.; ssh ieng6 "cd markdown-pharse;/software/CSE/oracle-java-17/jdk-17.0.1/bin/javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java;/software/CSE/oracle-java-17/jdk-17.0.1/bin/java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"` and it worked as successfully like the following pictures shown. 
<img width="630" alt="Screen Shot 2022-05-14 at 4 57 11 PM" src="https://user-images.githubusercontent.com/71100835/168451784-3c7d0470-0189-425c-b272-4ed26d8dd657.png">
<img width="633" alt="Screen Shot 2022-05-14 at 4 57 34 PM" src="https://user-images.githubusercontent.com/71100835/168451790-9691858d-1947-40ed-b95b-59ea7e8b52d1.png">
