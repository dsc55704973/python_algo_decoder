# Pythonic Text File Decoder
## # python_algo_decoder
### A simple pythonic algorithm to decode an unstructured, randomized text file (a simple exercise in intelligence)

### Quick Summary
Thank you for reviewing this simple bit of code that I recently submitted as part of a technical exam.  The task was to decode a message from a randomized, unstructred text file containing labeled pairs (an integer and a string). The key to decoding this mysterious message is to read the last word from three consecutive layers of the data after it has been restructed as a pyramid.

#### Exhibit A: Unstructured Txt File

<img width="631" alt="Screenshot 2024-04-13 at 4 17 53 PM" src="https://github.com/dsc55704973/python_algo_decoder/assets/66639071/efad9feb-6260-4616-88a1-960edc485325">

### Structure of Pyramid:
[1]

[2,3]

[4,5,6]

[7,8,9,10] 

...

### Format of Text File to Decode:
1 top

2 of

3 secret

4 power

5 excite

6 message

7 dog

8 opposite

9 oxygen

10 whole

...

### Output
** The algorithm, when set to parameters [1,3,6], will output:

#### ['top','secret','message']

### Method
The steps taken to leverage python to execute the decodification of this message are as follows:

#### Step 1: TXT OBJECT CONVERSION
The file provided is a text file (.txt), comprised of two columns: an integer column (leftmost column) and a string (rightmost column).  Since all colummns within a .txt file are rendered as strings, we must first convert the leftmost column representing integer-based coding to...integer values; likewise, we must ensure that we preserve the corresponding code values in the rightmost column as strings.  To accomplish this, we may use a combination of simple logic, nested loops, and the split().split() method to tell our function to read the left column as integers and the right column as strings values, with which we may proceed to execute the program.

#### Step 2: BUILD THE PYRAMID


#### Step 3: DECODE THE MESSAGE ('TOP SECRET MESSAGE')






