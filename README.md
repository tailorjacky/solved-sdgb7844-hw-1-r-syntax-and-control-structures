Download Link: https://assignmentchef.com/product/solved-sdgb7844-hw-1-r-syntax-and-control-structures
<br>
Submit two files through Blackboard: (a) .Rmd R Markdown file with answers and code and (b) Word document of knitted R Markdown file. Your file should be named as follows: “HW1-[Full Name]-[Class Time]” and include those details in the body of your file.

Please submit your solutions only once! Complete your work individually and comment your code for full credit. For an example of how to format your homework see the files related to the Lecture 1 Exercises and the RMarkdown examples on Blackboard.

<ol>

 <li>The vectors name, state.area, and state.region are pre-loaded in R and contain US state names, area (in square miles), and region respectively.

  <ul>

   <li>Identify the data type for name, state.area, and state.region.</li>

   <li>What is the longest state name (including spaces)? How long is it?</li>

   <li>Compute the average area of the states which contain the word “New” at the start of the state name. Use the function substr().</li>

   <li>Use the function table() to determine how many states are in each region. Use the function kable() to include the table in your solutions. (Notes: you will need the R package <em>knitr </em>to be able to use kable(). See the RMarkdown example in the Assignments folder on Blackboard for an example.)</li>

  </ul></li>

</ol>

1

<ol start="2">

 <li>Perfect numbers are those where the sum of the proper divisors (i.e., divisors other than the number itself) add up to the number. For example, 6 is a perfect number because its divisors, 1, 2, and 3, when summed, equal 6.

  <ul>

   <li>The following code was written to find the first 2 perfect numbers: 6 and 28; however, there are some errors in the code and the programmer forgot to add comments for readability. Debug and add comments to the following:</li>

  </ul></li>

</ol>

num.perfect &lt;- 2 count &lt;- 0 iter &lt;- 2

while(count &lt;= num.perfect){ divisor &lt;- 1

for(i 2:(iter-1)){ if(iter%%i==0) divisor &lt;- c(divisor, i)

} # end for loop

if(sum(divisor)=iter){

print(paste(iter, ” is a perfect number”, sep=””) count &lt;- count + 1 } # end if iter &lt;- iter + 1

} # end while loop

<ul>

 <li>Use the function date() at the start and at the end of your amended code. Then compute how long the program approximately takes to run (you can do this subtraction by hand). Find the run time when you set perfect to 1, 2, 3, and 4. Create a table of your results (Note: use the first table format in the RMarkdown Example file in the Assignments folder on Blackboard) . What are the first four perfect numbers?</li>

 <li>Let x &lt;- 1:4 and define y to be the vector of run times. Plot y vs x using the code below. Is the relationship between the discovery of perfect numbers and run times on your computer linear? Justify your answer.</li>

</ul>

plot(x, y, pch=20, type=”b”, xlab=”number of perfect numbers discovered”, ylab=”cumulative length of time (in seconds)”, main=”Cumulative Run Times to Discover Perfect Numbers”, las=TRUE)

SDGB 7844, C.H. Nagaraja                                                                                                                                                                                                                         Page 2 of 3

<ol start="3">

 <li>The geometric mean of a numeric vector <em>x </em>is computed as follows:</li>

</ol>

<em>.</em>

<ul>

 <li>Using a for loop, write code to compute the geometric mean of the numeric vector <em>x &lt; </em>−<em>c</em>(4<em>,</em>67<em>,</em>3). Make sure your code (i) removes any NA values and (ii) prints an error message if there are any non-positive values in x.</li>

 <li>Test your code on the following cases and show the output: (i) {NA<em>,</em>4<em>,</em>67<em>,</em>3}, (ii) {0<em>,</em>NA<em>,</em>6}, (iii) {67<em>,</em>3<em>,</em>∞}, and (iv) {−∞<em>,</em>67<em>,</em>3}.</li>

</ul>

SDGB 7844, C.H. Nagaraja                                                                                                                                                                                                                         Page 3 of 3