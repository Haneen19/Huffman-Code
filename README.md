# Huffman Compression Tool

## Overview

The Huffman Compression Tool is a Python application that implements the Huffman coding algorithm for compressing and decompressing files. This tool uses a frequency-based method to efficiently reduce the size of files while maintaining the integrity of the original data. It features a simple user interface built with Gradio, allowing users to upload files for compression and download the decompressed output.

### Features

- **File Compression**: Compresses files using Huffman coding.
- **File Decompression**: Decompresses the previously compressed files to retrieve the original content.
- **Compression Ratio Calculation**: Provides information about the size of the original file, compressed file, and the compression ratio.
- **User-Friendly Interface**: Simple and intuitive Gradio interface for easy file upload and download.

## How It Works

1. **Frequency Dictionary**: The tool reads the input file and builds a frequency dictionary for the bytes in the file.
2. **Huffman Tree**: It constructs a Huffman tree based on the frequency of each byte.
3. **Code Generation**: Each byte is assigned a unique binary code based on its position in the Huffman tree.
4. **Compression**: The tool compresses the input file by replacing the bytes with their corresponding Huffman codes and writes the compressed data to a new file.
5. **Decompression**: The compressed file can be decompressed to retrieve the original content, verifying that the compression process was successful.

## Usage

1. Clone this repository to your local machine or download the source code.
2. Install the required libraries:
   ```bash
   pip install gradio

 ``

3. Run the application:
  ```bash
python huffman_compression.py

   ````
4. Upload a file to compress using the Gradio interface.
5. Download the decompressed file after the process is complete.


## Example
You can use the tool by selecting a text file from your local filesystem. After compression, the tool will provide the compression results, including the original and compressed file sizes, the compression ratio, and a link to download the decompressed file.

