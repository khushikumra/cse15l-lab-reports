# Lab 5 Report: Khushi Kumra 
CSE 15L
## Step 1 - Student Post

Subject: Help! Unexpected Error in Matrix Processing

Hey everyone, I'm encountering a strange error in my Java program that deals with matrix processing. I've attached a screenshot below to show the issue.

![Screenshot](studentissue.png)

The program is supposed to process a matrix and display the elements. However, I'm getting an error that I can't quite figure out. I suspect it has something to do with how I'm iterating through the matrix. Any suggestions on what might be causing this?


## Step 2 - TA Response

Subject: Re: Help! Unexpected Error in Matrix Processing

Hey there! Thanks for reaching out. The error could be related to how you're iterating through the matrix. Maybe something about the loop conditions? Can you run the bash script and provide what the error message says?



## Step 3 - Student Result + Bug Description

![Screenshot](studentissueterminal.png)


Description of Bug:

The program generates an ArrayIndexOutOfBoundsException when attempting to access an out-of-bounds index in the processMatrix method. This error is caused by the loop conditions using <= instead of <, leading to an attempt to access the nonexistent fourth row and fourth column in a 3x3 matrix.



## Step 4 - Information

File & Directory Structure:

- MatrixProcessor.java (Java file)
- run.sh (Bash script)
Contents of Each File Before Fixing the Bug:

MatrixProcessor.java before fixing the bug:


![Screenshot](studentissue.png)


run.sh:

![Screenshot](runbeforerror.png)

Full Command Line to Trigger the Bug:

![Screenshot](terminalforerror.png)

Description of Bug Fix:

In the processMatrixWithError method of MatrixProcessorWithError.java, you have to update the loop conditions to use < instead of <= to prevent accessing out-of-bounds indices:

![Screenshot](successfulcode.png)

![Screenshot](successfulTerminal.png)

## Part 2 - Reflection


