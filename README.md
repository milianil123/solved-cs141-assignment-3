Download Link: https://assignmentchef.com/product/solved-cs141-assignment-3
<br>
<h1>The Greatest and the Least of These</h1>




Write a program with a loop that lets the user enter a series of positive integers. The user should enter -99 to signal the end of the series. After all the numbers have been entered, the program should display the largest and the smallest numbers entered. Use “The greatest of a set of numbers” algorithm (see below) to solve the problem.

<strong> </strong>

<strong><em>“The greatest of a set of numbers” algorithm: </em></strong>

<strong><em> </em></strong>

<ol>

 <li><em>Get (input) the first number, <u>set it to be the greatest for now</u>. </em></li>

 <li><em>Get the next number. </em></li>

 <li><em>If the new number is bigger than the “greatest” one – set the new one to be the “greatest”. </em></li>

 <li><em>Repeat steps 2 – 4 until all the numbers are consumed. </em></li>

</ol>

<strong><em> </em></strong>

<strong><em>Requirements: </em></strong>

<ol>

 <li>Your code must run correctly on the test cases below.</li>

 <li>DO NOT use arrays or ArrayLists to store the numbers in the series. Numbers must be analyzed on the spot and “discarded”.</li>

</ol>

<strong> </strong>

<strong><u>Test cases</u> </strong>

<ol>

 <li>User input (1 number): <em>-99</em>

  <ul>

   <li>Produces output “<em>No numbers were entered</em>”</li>

  </ul></li>

 <li>Input 2 numbers: <em>1 , -99</em>

  <ul>

   <li>Output: <em>the largest number: 1 ; the smallest number: 1</em></li>

  </ul></li>

 <li>Input 5 numbers :<em>1 , 2 ,55, 0, -99</em></li>

</ol>

Output: <em>the largest number: 55 ; the smallest number: 0</em>




Name your solution project GreatestAndLeast.java.

<strong> </strong>

<h1>e<sup>x </sup>Approximations</h1>

<strong> </strong>

The value e<sup>x</sup> can be approximated by the following sum:

1 + x + x<sup>2</sup>/2! + x<sup>3</sup>/3! + …+ x<sup>n</sup>/n!




The expression n! is called the factorial of n and is defined as: n! = 1*2*3* …*n.




Write a program that takes a value of x as input and outputs four approximations of e<sup>x</sup> done using four different values of n: 5, 10, 50, and 100. Output the value of x the user entered and the set of all four approximations into the screen.

Sample formula use: calculating e<sup>7 </sup>using approximation with n = 5    1 + 7 + 7<sup>2</sup>/2! + 7<sup>3</sup>/3! + 7<sup>4</sup>/4! + 7<sup>5</sup>/5!







<h2>Requirements</h2>

<ol>

 <li><u>Input validation</u> is needed – do not allow the user to enter anything but integer. Use exception-handling technique discussed in class and implemented in InputValidation.java example to complete the feature.</li>

 <li>Please do not do any calculations by writing out the entire sums by hand, use loops and running total calculations instead.</li>

 <li>Factorial function produces large numbers and it grows very quickly. If you start using regular integers to store factorials, you’ll get integer overflows easily. I would suggest using long to store factorials. On top of that, I would recommend to adjust your calculations in such a way that you never get to calculate the actual factorial values. Look at the pattern in the sum: each next term of the sum can be derived from the previous one by means of a very simple calculation.</li>

 <li>Test your code. Make sure the calculations are correct by checking the actual values of e<sup>x </sup> The bigger the value of n – the closer the resulting value must be to the actual value of e<sup>x.</sup></li>

</ol>




Name your solution project Approximations.java.




<strong> </strong>

<h1>File with Random Numbers</h1>




Write a program that generates 100 random integers in a given range and stores the integers in a file with a given name. When numbers are written into the file each integer is placed on a separate line.

<strong><em>Requirements </em></strong>

The program must:

<ol>

 <li>Ask user for a file name where the numbers will be written to. If the file does not exist it must be created. <u>If the file does exist its content is being replaced.</u></li>

 <li>Ask user to provide the range of random integers to be generated.

  <ul>

   <li>Use exception mechanism to validate user input to be of correct type. See InputValidation.java to get example of how to do that. Use two validation loops to make the user provide</li>

   <li>Both numbers of the range provided by the user must be <u>positive integers</u>. Continue asking user for input until the numbers fit the requirements.</li>

  </ul></li>

 <li>The user may give the numbers of the range in incorrect order. Make sure that lower limit is smaller than upper limit. If it is not the case – swap the numbers.</li>

 <li>Open the file with the given name, generate random numbers and write them in the file, placing each new number on a new line.</li>

 <li>Use try/catch block to handle possible IOExceptions. Your main() must not throw any exceptions.</li>

</ol>