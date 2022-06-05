How you found the tests with different results (Did you use vimdiff on the results of running a bash for loop? Did you search through manually? Did you use some other programmatic idea?)

__Via using vimdiff, we can compare the result between two different java file, and at the result of vimdiff, the system will markout the difference between two. To do so, I created two bashscipt files and bash script two of them into a different result.txt file, then compare it using vimdiff__

<img width="809" alt="Screen Shot 2022-06-05 at 3 40 28 PM" src="https://user-images.githubusercontent.com/71100835/172073575-ca8cca50-ee24-4727-8c21-823445d329c4.png">

~~~
bash script.sh > <my designated file name>
bash script2.sh > <my designated file name>
vimdiff <my designated file name 1> <my designated file name 2>
~~~
___

For example, according to the ouput I can see that test 22 and 32 are different. 

[test 22 page](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/22.html.test)

[test 22 download](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/22.md)

[test 32 page](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/32.html.test)

[test 32 download](https://github.com/nidhidhamnani/markdown-parser/blob/8dd87e6914ae40a4321aac8e2483e349de40b03c/test-files/32.md)
___

<img width="844" alt="Screen Shot 2022-06-05 at 3 50 32 PM" src="https://user-images.githubusercontent.com/71100835/172073859-94a85244-a463-484a-8293-6891954dc62e.png">
In test 22 we can see that the provided java file has no output while mine has extra output

In the mean time, the expected output is 
<img width="1440" alt="Screen Shot 2022-06-05 at 3 52 11 PM" src="https://user-images.githubusercontent.com/71100835/172073915-86f33a3b-9e20-4a87-986c-93ffaaa27fd1.png">
which you can see is ti*tle

For test 22, one of the bug we can fix is to fix the backslash detection 
~~~
/
~~~ 
because as we can see in the output everything after baf*/ should be deleted and I think the issued happened at the / before bar

<img width="1440" alt="Screen Shot 2022-06-05 at 3 59 18 PM" src="https://user-images.githubusercontent.com/71100835/172074108-880efe9a-de0b-44ba-8ea9-9b833bf3ca8d.png">
___
In test 32 we can see that the provided java file has no output while mine has extra output

<img width="887" alt="Screen Shot 2022-06-05 at 4 01 02 PM" src="https://user-images.githubusercontent.com/71100835/172074141-d54b387f-7a4b-41a6-a536-7368180016b5.png">

In the mean time, the expected output is 
<img width="1440" alt="Screen Shot 2022-06-05 at 4 04 33 PM" src="https://user-images.githubusercontent.com/71100835/172074239-5da39893-4cef-4de2-93d9-83b1960d1b60.png">

For test 32, one of the bug we can fix is to fix the backerror detection 
~~~
<
~~~ 
I feel like the code change is kinda similar with test 22 but different in term of type of word being detected
<img width="1440" alt="Screen Shot 2022-06-05 at 4 07 27 PM" src="https://user-images.githubusercontent.com/71100835/172074322-01182684-2be8-460b-a799-1a18d8c6a6ee.png">


