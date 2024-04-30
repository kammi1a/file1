1.Compression Function ('compress'):
This function takes a string 'inputText' and compresses it using a method called Run-Length Encoding (RLE).
It examines each character in the input text.
For every consecutive sequence of the same character, it counts the occurrences.
Once a different character is encountered or the end of the input text is reached, it appends the count followed by the character to the 'compressedStream'.
The function then returns the compressed string.
2.Decompression Function ('decompress'):
This function takes a compressed string 'compressedText' and decompresses it back to the original text.
It iterates through pairs of characters in the compressed text.
Each pair consists of a count (representing the number of repetitions) and a character.
It constructs the decompressed string by repeating each character according to its count.
Finally, it returns the decompressed string.
3.Main Function:
In the main function, the compression and decompression processes are managed.
It opens three files: 'input.txt' for reading, 'compressed.txt' for writing compressed data, and 'decompressed.txt' for writing decompressed data.
If any of the file operations fail, it displays an error message and exits.
The content of 'input.txt' is read into a string using a 'stringstream'.
The input text is compressed using the 'compress' function and the compressed data is written to 'compressed.txt'.
Then, the compressed text is decompressed using the 'decompress' function and the decompressed data is written to 'decompressed.txt'.
Finally, a message is printed to indicate that the compression and decompression processes are complete.
