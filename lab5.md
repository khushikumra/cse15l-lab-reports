# Lab 5 Report: Khushi Kumra 
CSE 15L
## Step 1 - Student Help Request

Subject: Help! Unexpected Error in Matrix Processing

Hey everyone, I'm encountering a strange error in my Java program that deals with matrix processing. I've attached a screenshot below to show the issue.

![Screenshot](link-to-screenshot.png)

The program is supposed to process a matrix and display the elements. However, I'm getting an error that I can't quite figure out. I suspect it has something to do with how I'm iterating through the matrix. Any suggestions on what might be causing this?


## Step 2 - TA Response

Subject: Re: Help! Unexpected Error in Matrix Processing

Hey there! Thanks for reaching out. The error might be related to how you're iterating through the matrix. Can you try looking into the loop conditions in your `processMatrixWithError` method? Specifically, check if the indices go out of bounds. Let me know what you find.



## Step 3 - # Command to run for the screenshot
./run.sh

Terminal Output:

Original Matrix:
1 2 3 
4 5 6 
7 8 9 
Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException: Index 3 out of bounds for length 3
    at MatrixProcessorWithError.processMatrixWithError(MatrixProcessorWithError.java:13)
    at MatrixProcessorWithError.main(MatrixProcessorWithError.java:8)

Description of Bug:
The program generates an ArrayIndexOutOfBoundsException when attempting to access an out-of-bounds index in the processMatrixWithError method. This error is caused by the loop conditions using <= instead of <, leading to an attempt to access the nonexistent fourth row and fourth column in a 3x3 matrix




## Step 4 - File & Directory Structure:

MatrixProcessorWithError.java (Java file)
run.sh (Bash script)
Contents of Each File Before Fixing the Bug:

MatrixProcessorWithError.java:


public class MatrixProcessorWithError {
    // ... (Same as provided in the previous response)
}

run.sh:
#!/bin/bash
javac MatrixProcessorWithError.java
java MatrixProcessorWithError

Full Command Line to Trigger the Bug:

./run.sh

Description of Bug Fix:

In the processMatrixWithError method of MatrixProcessorWithError.java, update the loop conditions to use < instead of <= to prevent accessing out-of-bounds indices:

public static void processMatrix(int[][] matrix) {
    // Fix the bug by using < instead of <= in loop conditions
    for (int i = 0; i < matrix.length; i++) {
        for (int j = 0; j < matrix[i].length; j++) {
            System.out.print(matrix[i][j] + " ");
        }
        System.out.println();
    }
}


## Step 8


![no args](catnoargs.png)

**Keys Pressed**
vim ListExamples.java 



**Commands and Effects Summary**


## Step 9


![no args](catnoargs.png)

**Keys Pressed**
&lt;up&gt; &lt;up&gt; &lt;up&gt; &lt;enter&gt; &lt;up&gt; &lt;up&gt; &lt;up&gt; &lt;enter&gt; 




**Commands and Effects Summary**

went up three time o access javac -cp command. went up another three times to acces java -cp command
