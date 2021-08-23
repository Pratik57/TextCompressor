# TextCompressor

### This tool uses Huffman Coding to compress data! 
**Huffman Coding** is a popular technique used for Lossless Data Compression. 
    
*Lossless compression* is a class of data compression algorithms that allows the original data to be perfectly reconstructed from the compressed data. It is preffered for text file compression, 

*Lossy compression* permits reconstruction only of an approximate amount of the original data, though usually with greatly improved compression rates. It is generally preferred for audio, video and image files.


A Huffman code is a particular type of optimal prefix code that is commonly used for lossless data compression. The output from Huffman's algorithm can be viewed as a variable-length code table for encoding a source symbol (such as a character in a file). The algorithm derives this table from the estimated probability or frequency of occurrence (weight) for each possible value of the source symbol.

Prefix Codes, means the codes (bit sequences) are assigned in such a way that the code assigned to one character is not the prefix of code assigned to any other character. This is how Huffman Coding makes sure that there is no ambiguity when decoding the generated bitstream. 


**How Compression Works**


- ****Build Huffman Tree:****
  - Input is an Array or Hashmap of unique characters along with their frequency of occurrences and output is Huffman Tree.
  - Create a leaf node for each unique character and build a Min Heap (or a priority queue) of all leaf nodes
  - Extract two nodes with the minimum frequency from the min heap.
  - Create a new internal node with a frequency equal to the sum of the two nodes frequencies. Make the first extracted node as its left child and the other  extracted node as its right child. Add this node to the min heap.
  - Repeat steps 2 and 3 until the heap contains only one node. The remaining node is the root node and the tree is complete.

- ****Print codes from Huffman Tree:****
  - Traverse the tree formed starting from the root. Maintain an auxiliary array. While moving to the left child, write 0 to the array. While moving to the right child, write 1 to the array. Print the array when a leaf node is encountered.


**How De-compression Works**
- Decompression is simply a matter of translating the stream of prefix codes to individual byte values, usually by traversing the Huffman tree node by node as each bit is read from the input stream (reaching a leaf node necessarily terminates the search for that particular byte value).


