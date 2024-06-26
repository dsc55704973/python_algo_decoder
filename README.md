# Pythonic Text File Decoder
## # python_algo_decoder
### A simple pythonic algorithm to decode an unstructured, randomized text file (a simple exercise in intelligence)

### Quick Summary
Thank you for reviewing this simple bit of code that I recently submitted as part of a technical exam.  The task was to decode a message from a randomized, unstructured text file containing labeled pairs (an integer and a string). The key to decoding this mysterious message is to read the last word from three consecutive layers of the data after it has been restructured as a pyramid.

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
The file provided is a text file (.txt), comprised of two columns: an integer column (leftmost column) and a string (rightmost column).  Since all columns within a .txt file are rendered as strings, we must first convert the leftmost column representing integer-based coding to...integer values; likewise, we must ensure that we preserve the corresponding code values in the rightmost column as strings.  To accomplish this, we may use a combination of simple logic, nested loops, and the split().split() method to tell our function to read the left column as integers and the right column as strings values, with which we may proceed to execute the program.

<img width="839" alt="Screenshot 2024-04-15 at 12 14 02 AM" src="https://github.com/dsc55704973/python_algo_decoder/assets/66639071/fc408f5c-dd01-475d-a6ce-1c2d3d32a305">


#### Step 2: BUILD THE PYRAMID
The key methodology for decoding the file is to arrange it as a pyramid, where every layer of the pyramid adds another value to the end of the sequence, such that Layer 1 = [1], Layer 2 = [2,3], Layer 3 = [4,5,6], etc.  Accordingly, the last value of every level on the top three levels (that is, indices 1, 3, and 6) represent three words that form the message we are trying to decode.  To execute, we simply need to arrange these values into a list of lists, with each inner list representing a layer of the pyramid.

<img width="1076" alt="Screenshot 2024-04-15 at 12 15 08 AM" src="https://github.com/dsc55704973/python_algo_decoder/assets/66639071/7dba21c0-f42a-407e-9fd4-fcef68a5277c">


#### Step 3: DECODE THE MESSAGE ('TOP SECRET MESSAGE')
The final step is to iterate through the indices we've set as the encoded message (1,3,6) with for loop and return the corresponding strings.  All there is left to do now is return the pyramid and decoded message.

<img width="1069" alt="Screenshot 2024-04-15 at 12 15 52 AM" src="https://github.com/dsc55704973/python_algo_decoder/assets/66639071/81aa9f9b-fb4c-425a-8ed3-aa4371dfa73e">

#### RETURN THE PYRAMID & THE DECODED MESSAGE
After performing the function on the text file, we return a pyramid-structured list, as well as the final decoded message ("top secret message").

<img width="1184" alt="Screenshot 2024-04-15 at 12 38 57 AM" src="https://github.com/dsc55704973/python_algo_decoder/assets/66639071/96b218c5-ab14-44d8-93b6-0a98be699c76">







