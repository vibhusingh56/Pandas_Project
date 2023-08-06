# PDF Number Extractor

This Python script extracts all the numbers (both integers and decimals) from a PDF file and creates a table as its output using the Pandas library.

## Requirements

- Python 3.x
- PyPDF2 library (install using `pip install PyPDF2`)
- Pandas library (install using `pip install pandas`)

## How to Use

1. Install Python 3.x on your system if you haven't already.
2. Install the required libraries by running the following commands:

```bash
pip install PyPDF2
pip install pandas
```

3. Clone or download this repository to your local machine.
4. Place the PDF file from which you want to extract numbers in the same directory as `extract_numbers.py`.
5. Open the terminal or command prompt and navigate to the project directory.
6. Replace `"example.pdf"` in the `pdf_file_path` variable in `extract_numbers.py` with the path to your PDF file.
7. Run the `extract_numbers.py` script by executing the following command:

```bash
python extract_numbers.py
```

8. The script will process the PDF file, extract the numbers, and display a table with the extracted numbers.

## Sample Output

If the PDF file "example.pdf" contains the following content:

```
Page 1:
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
123.45 and 6789 are some numbers in this page.

Page 2:
More numbers can be found here: 987.65 and 42. The total is 1029.65.
```

The script will produce the following output:

```
Extracted Numbers Table:
   Numbers
0   123.45
1     6789
2   987.65
3       42
4  1029.65
```

## Note

- The script uses regular expressions to find numbers in the PDF content, so the accuracy of the extraction depends on the structure of the PDF file.
- Make sure to replace `"example.pdf"` in `extract_numbers.py` with the path to your actual PDF file.
- For complex PDFs with varying structures, you may need to adjust the regular expression pattern in the script to capture all the desired numbers accurately.
