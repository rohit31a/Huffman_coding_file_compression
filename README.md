

# ZipItNow - Huffman Coding File Compression

ZipItNow is a project based on Huffman Coding, a lossless compression algorithm implemented in C++. It allows you to compress and decompress text files efficiently.

## How it Works

Huffman Coding is a popular compression technique that assigns variable-length codes to characters based on their frequency of occurrence in the input text. The more frequent a character, the shorter its code.

The compression process involves building a Huffman tree by analyzing the input text's character frequencies. The tree is then used to generate a code table, mapping each character to its corresponding binary code. Finally, the input text is encoded using the generated codes.

To decompress the compressed text, the code table and encoded data are used to rebuild the original text by traversing the Huffman tree.

## Usage

1. Clone the repository or download the project files.

2. Compile the source code using a C++ compiler:
   - For compression:
     ```shell
     g++ encode.cpp huffman.cpp -o ZipItNow
     ```

   - For decompression:
     ```shell
     g++ decode.cpp huffman.cpp -o ZipItNow
     ```

3. To compress a text file:
   ```shell
   ./ZipItNow compress inputFile.txt compressedFile.huf
   ```

4. To decompress a previously compressed file:
   ```shell
   ./ZipItNow decompress compressedFile.huf outputFile.txt
   ```

## Example

To compress a file named `inputFile.txt` and generate the compressed file `compressedFile.huf`, use the following command:
```shell
./ZipItNow compress inputFile.txt compressedFile.huf
```

To decompress the compressed file `compressedFile.huf` and generate the decompressed file `outputFile.txt`, use the following command:
```shell
./ZipItNow decompress compressedFile.huf outputFile.txt
```

## Dependencies

This project does not have any external dependencies. It is implemented using standard C++ libraries.

## Contributing

Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

--
