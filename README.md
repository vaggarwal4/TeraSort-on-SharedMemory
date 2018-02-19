# TeraSort-on-SharedMemory

"in.txt" is a gensort generated text. You can create one with this http://www.ordinal.com/gensort.html

## Creating a Gensort Text file:
Go to directory where you've installed gensort.
Type ./gensort -a [no_of_Records] [filename.txt]
Each line of the record contains 100 bytes
So [no_of_Records] * 100 = size of file.
Example: ./gensort -a 10000000 pennyInput.txt --> will create a 1GB text file
The sorting is done on keys i.e. first 10 bytes of each records and then the corresponding value is appended.

## Validating the Sorted output file:
Using ./valsort [filename] you can test the sorted file
