Download Link: https://assignmentchef.com/product/solved-programming-project-7-payroll-c-program-that-processes-a-payroll
<br>
<h4><u></u><u>Concepts tested by the program</u>:</h4>

1.  Working with arrays

2.  Using file operations

3. Using a selection sort to sort parallel arrays

4. Using a binary search with sorted arrays

5. Using a sequential (linear) search with unsorted arrays

6. Implementing functions besides function main()

<h4><strong><u>Project Description</u></strong></h4>

Write a C++ program that processes a payroll. Your program will calculate the wages for each employee, given the number of hours worked and the payrate per hour. It will search for two employees by number, one with a binary search (see page 462) and one with a linear search (see page 459). A selection sort (see page 476) will sort the arrays so that the employee numbers are in ascending order.

<h4><strong><u>Project Specifications</u></strong></h4>

<strong><u>Input</u></strong> for this project has two sources.  The user must enter the names of the input and output files from the keyboard. The user will enter two employee numbers from the keyboard in response to prompts.  The input file should have one line for each employee with the 3 required items: employeeID, hoursWorked, and payRate (separated by whitespace on the file) The last line of the file <strong><u>must always have only -1</u></strong>.

<strong><u>Output</u></strong> also has two sources.  The program title and the programmer name should appear on both the console and the file. If the input file does not open, an error message should appear on the console and no attempt should be made to open the output file for any output or processing. The message “Processing complete” should appear on the console after the programmer name and just before the main program ends (make it the last statement before “return;”).  The console output will show the prompts with the search numbers. The file output should show the unsorted table of the input items with the wages, followed by the sorted table with the same 4 columns. The column numbers with decimal amounts should line up on the decimal point under the column headings.

<h4><strong><u>Processing Requirements</u></strong></h4>

Your program should use the following one-dimensional arrays:

<strong><em>empId</em></strong>: an array of long integers to hold employee identification numbers. Assume there will be no more than 20 identification numbers, but your code should check that the file doesn’t attempt to enter more. If an attempt is made to enter 21, process only the first 20.

<strong><em>hours</em></strong>: an array of doubles to hold the number of hours worked by each employee. Fractional hours are possible.

<strong><em>payRate</em></strong>: an array of doubles to hold each employee’s hourly pay rate.

<strong><em>wages</em></strong>: an array to hold each employee’s gross wages.

The program should relate the data in each array through the subscripts. For example, the number in element 0 of the hours array should be the number of hours worked by the employee whose identification number is stored in element 0 of the empId array. That same employee’s pay rate should be stored in element 0 of the payRate array.

1) Calculate the wages for each employee and place into an array with the related subscript.

2) Write the unsorted arrays on the output file.

3) Prompt for and input from the keyboard an empID to use for the linear search.

4) Next sort the empID long integers using the <u>selection sort</u> algorithm. If an exchange is made for empID, be sure to make the corresponding exchanges in the three associated items.

5) Write the sorted arrays on the output file.

6) Prompt for and input from the keyboard an empID to use for the binary search.

The Selection sort algorithm, Binary Search and Linear Search algorithms should be three separate functions that will be called from the function main().  Modify the code in your text for this project. Do NOT use any output statements in these functions. You may use more functions in your design.




You may assume that the input file is constructed correctly, and will always contain -1 at the end. Be sure to test for an empty file (one that contains ONLY -1) and a file with more than 20 employees. Print an error message to the screen if there are no employees, and do NOT attempt to open the output file. If your file has more than 20 employees, just

process the first 20 (without an error message.)

To input the file items without reading past the end of the file (-1 is the sentinel), use a while loop with two conditions: the empID in a temporary variable that is not negative and the number of employees less than 20. Inside your loop body: Store the “good” employee number, input the number of hours and the payRate in the arrays. The last item in your loop should be the next employee number from the file.

Project 7: Payroll employee