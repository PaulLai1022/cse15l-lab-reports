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
