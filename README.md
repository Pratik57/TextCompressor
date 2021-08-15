# TextCompressor

### This tool uses Huffman Coding to compress data! 
**Huffman Coding** is a popular technique used for Lossless Data Compression. 
    
*Lossless compression* is a class of data compression algorithms that allows the original data to be perfectly reconstructed from the compressed data. It is preffered for text file compression, 

*Lossy compression* permits reconstruction only of an approximate amount of the original data, though usually with greatly improved compression rates. It is generally preferred for audio, video and image files.

Data compression ratio , also known as compression power, is a measurement of the relative reduction in size of data representation produced by a data compression algorithm. It is typically expressed as the division of uncompressed size by compressed size. Thus, a representation that compresses a file's storage size from 10 MB to 2 MB has a compression ratio of 10/2 = 5 

A Huffman code is a particular type of optimal prefix code that is commonly used for lossless data compression. The process of finding or using such a code proceeds by means of Huffman coding, an algorithm developed by David A. Huffman.
The output from Huffman's algorithm can be viewed as a variable-length code table for encoding a source symbol (such as a character in a file). The algorithm derives this table from the estimated probability or frequency of occurrence (weight) for each possible value of the source symbol.
Prefix Codes, means the codes (bit sequences) are assigned in such a way that the code assigned to one character is not the prefix of code assigned to any other character. This is how Huffman Coding makes sure that there is no ambiguity when decoding the generated bitstream. 
