# Sithafal_Technogolies_Task-1

# PDF Content Extractor

A Python script to extract text, tables, and images from specific pages of a PDF file using `PyMuPDF` (`fitz`) and `pdfplumber`. This tool is designed to help users easily query and retrieve content from PDF files.

---

## Features

- Extract **text** and **tables** from specified pages using `pdfplumber`.
- Extract **images** from specified pages using `PyMuPDF` (`fitz`).
- Automatically handles missing or invalid directories for image output.
- Provides a detailed response with the extracted data and image paths.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/pdf-content-extractor.git
   cd pdf-content-extractor
   ```

2. Install the required dependencies:
   ```bash
   pip install --upgrade pymupdf pdfplumber
   ```

---

## Usage

1. Place your PDF file in an accessible directory.
2. Update the `pdf_path` variable in the script to point to your PDF file.
3. Run the script:
   ```bash
   python script_name.py
   ```

4. Enter your query in the format:
   ```
   page 1
   page 2
   ```
   The script will process the requested pages and return extracted content.

---

## Example Output

### Query
```
Enter your query: page 1 page 2
```

### Response
```
Data from page 1:
Text:
<Extracted text>

Tables found on this page:
Table 1:
Column1 | Column2
Value1  | Value2

Images extracted from this page:
 /path/to/output/page_1_img1.png

Data from page 2:
Text:
<Extracted text>

No tables found on this page.
Images extracted from this page:
 /path/to/output/page_2_img1.png
 /path/to/output/page_2_img2.png
```

---

## Configuration

- **PDF File Path**: Update the `pdf_path` variable to the path of your PDF file.
- **Image Output Directory**: Update the `image_output_dir` variable to specify where extracted images should be saved.

---

## Dependencies

- [`PyMuPDF`](https://pymupdf.readthedocs.io/en/latest/) for handling PDFs and extracting images.
- [`pdfplumber`](https://github.com/jsvine/pdfplumber) for extracting text and tables.

Install dependencies with:
```bash
pip install --upgrade pymupdf pdfplumber
```

---

## Limitations

- Only supports querying specific pages.
- Image extraction is limited to raster images embedded in the PDF.
- Requires the user to provide the correct page numbers in the query.

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes and submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Author

[Your Name](https://github.com/vivek090909)  
Feel free to reach out with suggestions, questions, or issues.
```

### Customization Notes:
- Replace `script_name.py` with your actual script filename.
- Replace `your-username` and other placeholders with your GitHub username and project-specific details.
