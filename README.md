Download Link: https://assignmentchef.com/product/solved-lab-exercise-9-problems
<br>
<ol>

 <li>Write C++ programs</li>

 <li>Compile C++ programs</li>

 <li>Implement programs that use pointers and dynamically allocated memory</li>

</ol>

<h1><a id="user-content-additional-reading" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09#additional-reading" aria-hidden="true"></a>Additional Reading</h1>

This lab exercise requires an understanding of some concepts to solve the problems. You are strongly encouraged to read the following tutorials to help you answer the problems.

<ol>

 <li><a href="https://github.com/ILXL-guides/function-file-organization">Organizing C++ files: function prototypes, implementations, and drivers</a>.</li>

 <li><a href="https://github.com/ILXL-guides/object-parameters-and-return-values">Using objects as parameters and return values in functions</a></li>

 <li><a href="https://github.com/ILXL-guides/arrays-as-parameters">Passing arrays as parameters to functions</a></li>

 <li><a href="https://github.com/ILXL-guides/cpp-file-io">File reading and writing (also includes dealing with arrays)</a></li>

</ol>

<h1><a id="user-content-instructions" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09#instructions" aria-hidden="true"></a>Instructions</h1>

Answer the programming problems sequentially (i.e., answer prob01 before prob02). If you have questions let your instructor or the lab assistant know. You can also consult your classmates.

When you answer two programming problems correctly, let your instructor know and wait for further instruction.

<h1><a id="user-content-lab-exercise-guide" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09#lab-exercise-guide" aria-hidden="true"></a>Lab exercise guide</h1>

Here’s a link to the <a href="https://docs.google.com/document/d/1EX01EtrO-pkHNLVPxiq7HNh1f5KnJZnr_dlJcO4T7t0/edit?usp=sharing" rel="nofollow">Lab exercise guide</a> in case you need to review the lab exercise objectives, grading scheme, or evaluation process.




<h1>Evens Array</h1>

Create a program that checks whether each value in a given array is even or not. The results will be stored in a separate <code>bool</code> array.

We will implement this functionality using the <code>find_evens</code> function.

<h3><a id="user-content-find_evens" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob01#find_evens" aria-hidden="true"></a>find_evens</h3>

<code>find_evens</code> should receive three parameters, an <code>int*</code> that refers to an array, a <code>bool*</code> that refers to another array, and an <code>int</code> for the size of the array. We assume that the size of both arrays are the saame.

Kindly make use of pointer arithmetic and not arrays or array indexes (<code>[]</code>).

The function should check to see if the contents in the <code>int*</code> array are <em>even</em> or <em>odd</em>. Store the value <code>true</code> into the <code>bool</code> array at the corresponding index if the content in the <code>int</code> array at that same index is <code>even</code>, otherwise store the value <code>false</code>. For example:

<strong>int* array values</strong>: {2, 6, 3, 7, 4}

<strong>bool* array values</strong>: {true, true, false, false, true}

<em>NOTE</em>: In the <code>main</code> function, you are given an array with initial values and an initial size. Complete the missing parts of the program by following the instructions in <code>main.cpp</code>. Your function is expected to work with any other values aside from those used in <code>main</code>.

<h2><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob01#sample-output" aria-hidden="true"></a>Sample Output</h2>

<pre><code>01011</code></pre>

Place the <code>find_even</code>‘s function prototype in <code>evens_array.hpp</code> and it’s implementation in <code>evens_array.cpp</code>. The <code>main</code> function already contains some code, but you need to complete the requirements that is described inside the file.

<h1><a id="user-content-submission-checklist" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob01#submission-checklist" aria-hidden="true"></a>Submission checklist</h1>

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob01#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code saved in <code>evens_array.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp evens_array.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Class Average</h1>

Create a program that dynamically creates an array whose size depends on the user’s preference. Pass the array to a <code>calculate_avg</code> function that is responsible for computing the average GPA of the given array. <strong>Use pointer arithmetic throughout your program.</strong>

<h3><a id="user-content-calculate_avg" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob02#calculate_avg" aria-hidden="true"></a>calculate_avg</h3>

Create a function called <code>calculate_avg</code> that calculates the average of a <code>double</code> array and returns that average.

<code>calculate_avg()</code> will have two parameters:

<ol>

 <li>a <code>double*</code> referring to the array</li>

 <li>an <code>int</code> that contains the size of the given array.</li>

</ol>

When the array is size is greater than 0, the function should calculate the average GPA from the given array of grades.

However, when the size of the array is 0, then the function should return 0.

<h3><a id="user-content-main" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob02#main" aria-hidden="true"></a>main</h3>

The <code>main</code> function has mostly been built for you. It is your task to dynamically create a <code>double</code> array, store users’ grades into the array, and pass the array to <code>calculate_avg</code> to compute and then display the students’ average GPA. Read the instructions in <code>main.cpp</code> for more details.

If the user happens to provide a class size of <code>0</code>, then the program should output <code>"You have no class!"</code> and then end the execution of the program without attempting to calculate the average.

Do not forget to deallocate memory that your code dynamically created.

Place the <code>calculate_avg</code>‘s function prototype in <code>calculate_avg.hpp</code> and it’s implementation in <code>calculate_avg.cpp</code>.

<h1><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob02#sample-output" aria-hidden="true"></a>Sample Output</h1>

<pre>How many students are in your class? <b>5</b>Enter the GPA for the students in your class (0.0 - 4.0)Enter the GPA for student #1: <b>3.8</b>Enter the GPA for student #2: <b>2.5</b>Enter the GPA for student #3: <b>4.0</b>Enter the GPA for student #4: <b>1.9</b>Enter the GPA for student #5: <b>3.6</b>Class average: 3.16</pre>

<pre>How many students are in your class? <b>0</b>You have no class!</pre>

Submission checklist

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob02#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>calculate_avg.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp calculate_avg.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Add Array</h1>

Create a program that adds the contents of one array into another array using their corresponding indices. <strong>Use pointer arithmetic throughout your program.</strong>

<h3><a id="user-content-add_array" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob03#add_array" aria-hidden="true"></a>add_array</h3>

Create a function called <code>add_array</code> that takes two arrays of the same size and adds their contents then stores the result in the first array.

<code>add_array</code> will have three parameters in total:

<ol>

 <li>an <code>int*</code> pointing to the first array</li>

 <li>an <code>int*</code> pointing to the second array</li>

 <li>the <code>size</code> of the arrays (we assume that the two arrays always have the same size)</li>

</ol>

The goal of the function is to add all the values from the second array into the first array according to their position in the array. For example, the value in index 0 of the second array will be added to the current value in index 0 of the first array. The sum of both values will replace the old value in index 0 of the first array.

We expect that modifying the first array inside <code>add_array</code> will also change the source array that was passed into this function as an argument because arrays point to the address of the array. Take a look at how the values in the array declared in <code>main</code> change after you call <code>add_array</code>.

<h3><a id="user-content-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob03#output" aria-hidden="true"></a>Output</h3>

All screen output (<code>std::cout</code>) should be placed in the <code>main</code> function while the array manipulation will be in the <code>add_array</code> function.

Use the 2 integer arrays of size 10 in <code>main</code> as parameters to call your <code>add_array</code> function. The function will add the values in both arrays and store the result in the first array.

Most of the code has already been created for you in <code>main.cpp</code>. You only need to fill in the missing parts. Read the instructions inside the file for more details.

Place the <code>add_array</code>‘s function prototype in <code>add_array.hpp</code> and it’s implementation in <code>add_array.cpp</code>.

<h1><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob03#sample-output" aria-hidden="true"></a>Sample Output</h1>

<pre>Inputs for the first array:Enter the integer for index 0: <b>5</b>Enter the integer for index 1: <b>8</b>Enter the integer for index 2: <b>2</b>Enter the integer for index 3: <b>7</b>Enter the integer for index 4: <b>21</b>Enter the integer for index 5: <b>67</b>Enter the integer for index 6: <b>12</b>Enter the integer for index 7: <b>0</b>Enter the integer for index 8: <b>1</b>Enter the integer for index 9: <b>6</b>Inputs for the second array:Enter the integer for index 0: <b>5</b>Enter the integer for index 1: <b>2</b>Enter the integer for index 2: <b>7</b>Enter the integer for index 3: <b>2</b>Enter the integer for index 4: <b>3</b>Enter the integer for index 5: <b>12</b>Enter the integer for index 6: <b>7</b>Enter the integer for index 7: <b>15</b>Enter the integer for index 8: <b>16</b>Enter the integer for index 9: <b>100</b>The first array contains:5 8 2 7 21 67 12 0 1 6The second array contains:5 2 7 2 3 12 7 15 16 100Calling add_array using the first and second array ...After calling add_array, the first array now contains:10 10 9 9 24 79 19 15 17 106</pre>

Submission checklist

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob03#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>add_array.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp add_array.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Pointer Min</h1>

Create a function called <code>min</code> that receives two parameters, an <code>int*</code> and <code>int</code> size. The function should return the minimum value in the array. Assume that the array passed to <code>min</code> will always have at least one element.

Your code should only use pointer arithmetic. Do not use <code>[]</code> notations.

<h1><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob04#sample-output" aria-hidden="true"></a>Sample Output:</h1>

<pre><code>Array: -1 22 54 33 -40 67 8 15Min: -40</code></pre>

Submission checklist

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob04#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>min.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp min.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<h6><code>make all</code></h6>

<h1>Print Array Reverse</h1>

Create a program that displays the contents of an array in reverse.

<h3><a id="user-content-print_array_reverse" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob05#print_array_reverse" aria-hidden="true"></a>print_array_reverse()</h3>

Create a function called <code>print_array_reverse</code> that prints out the contents of an integer array in reverse.

Within this function you are only allowed to use pointer arithmetic to access elements of the array.

You are not allowed to use the <code>[]</code> operator to complete this question.

<code>print_array_reverse()</code> will have two parameters in total:

<ol>

 <li>an <code>int*</code> pointer that refers to an array</li>

 <li>an <code>int</code> that stores the number of elements in the array</li>

</ol>

Your function has two main scenarios it could encounter.

When you have an array with a size that is greater than 0, then it should behave normally and output the array’s contents in reverse.

But, if your function encounters an array with size of 0 or negative, then it should output <code>There are no contents in this array!</code> and go to the next line.

Refer to the sample output to see instances of both.

Complete the code in <code>main.cpp</code>, provide the headers in <code>print_array_reverse.hpp</code> and the implementation in <code>print_array_reverse.cpp</code>.

<h1><a id="user-content-sample-output" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob05#sample-output" aria-hidden="true"></a>Sample Output</h1>

<pre>Enter an integer for the size of the array(Must be less than or equal to 10): <b>10</b>Inputs for the array:Enter the integer for index 0: <b>4</b>Enter the integer for index 1: <b>3</b>Enter the integer for index 2: <b>2</b>Enter the integer for index 3: <b>1</b>Enter the integer for index 4: <b>89</b>Enter the integer for index 5: <b>15</b>Enter the integer for index 6: <b>100</b>Enter the integer for index 7: <b>24</b>Enter the integer for index 8: <b>254</b>Enter the integer for index 9: <b>2</b>The contents of the array in reverse are:2 254 24 100 15 89 1 2 3 4</pre>

<pre>Enter an integer for the size of the array(Must be less than or equal to 10): <b>0</b>Inputs for the array:There are no contents in this array!</pre>

Submission checklist

<ol>

 <li>Created function prototype and stored in <code>.hpp</code> file.</li>

 <li>Created function implementation and stored in <code>.cpp</code> file (see <a href="https://github.com/ILXL-guides/function-file-organization">reference</a>).</li>

 <li>Call function in the driver</li>

 <li>Compiled and ran the driver (<code>main</code>).</li>

 <li>Manually checked for compilation and logical errors.</li>

 <li>Ensured no errors on the unit test (<code>make test</code>).</li>

 <li>Followed advice from the stylechecker (<code>make stylecheck</code>).</li>

 <li>Followed advice from the formatchecker to improve code readbility (<code>make formatcheck</code>).</li>

</ol>

<h1><a id="user-content-code-evaluation" class="anchor" href="https://github.com/peskin55/CPSC121/tree/master/Labs/Lab_09/prob05#code-evaluation" aria-hidden="true"></a>Code evaluation</h1>

Open the terminal and navigate to the folder that contains this exercise. Assuming you have pulled the code inside of <code>/home/student/labex02-tuffy</code> and you are currently in <code>/home/student</code> you can issue the following commands

<pre><code>cd labex02-tuffy</code></pre>

You also need to navigate into the problem you want to answer. To access the files needed to answer problem 1, for example, you need to issue the following command.

<pre><code>cd prob01</code></pre>

When you want to answer another problem, you need to go back up to the parent folder and navigate into the next problem. Assuming you are currently in <code>prob01</code>, you can issue the following commands to go to the parent folder then go into another problem you want to answer; <code>prob02</code> for example.

<pre><code>cd ..cd prob02</code></pre>

Use the <code>clang++</code> command to compile your code and the <code>./</code> command to run it. The sample code below shows how you would compile code save in <code>print_array_reverse.cpp</code> and <code>main.cpp</code>, and into the executable file <code>main</code>. Make sure you use the correct filenames required in this problem. Take note that if you make any changes to your code, you will need to compile it first before you see changes when running it.

<pre><code>clang++ -std=c++17 main.cpp print_array_reverse.cpp -o main./main</code></pre>

You can run one, two, or all the commands below to <code>test</code> your code, <code>stylecheck</code> your code’s design, or <code>formatcheck</code> your work. Kindly make sure that you have compiled and executed your code before issuing any of the commands below to avoid errors.

<pre><code>make testmake stylecheckmake formatcheck</code></pre>

A faster way of running all these tests uses the <code>all</code> parameter.

<pre><code>make all</code></pre>