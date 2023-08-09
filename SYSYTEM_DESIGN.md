# Invoice to PDF Conversion Script System Design

## Overview

The Invoice to PDF Conversion Script project automates the process of converting Excel invoices into visually organized PDF documents. Leveraging the `pandas` and `fpdf` libraries, this system demonstrates the power of Python in transforming raw financial data into professional and efficient documents.

## Architecture

The architecture of the Invoice to PDF Conversion Script project consists of the following components:

1. **Excel Invoices (`invoices/`):** This directory contains Excel files (invoices) following the naming convention "InvoiceNumber-Date.xlsx." Each file contains invoice data, including product details, amounts, and prices.

2. **PDF Generation Script (`invoice_to_pdf.py`):** This Python script reads Excel invoices from the `invoices/` directory, extracts invoice data, and generates corresponding PDF invoices in the `PDFs/` directory. The generated PDFs include essential invoice details and product breakdowns.

3. **Generated PDFs (`PDFs/`):** This directory is where the script stores the generated PDF invoices, each reflecting the data from the respective Excel invoice.

## Data Flow

1. The `invoice_to_pdf.py` script iterates through Excel files in the `invoices/` directory.
2. For each Excel file, the script extracts invoice data using the `pandas` library.
3. The script utilizes the `fpdf` library to generate a PDF invoice layout, incorporating invoice number, date, product details, and total sum.
4. The generated PDF invoice is saved in the `PDFs/` directory with a filename corresponding to the input Excel file.

## File Structure

- `invoice_to_pdf.py`
- `invoices/`
    - `InvoiceNumber-Date.xlsx`
    - ...
- `PDFs/`
    - `InvoiceNumber-Date.pdf`
    - ...
- `LICENSE` (License file)
- `README.md` (Project documentation)

## Interaction Flow

1. User places Excel invoice files in the `invoices/` directory.
2. User runs the script `invoice_to_pdf.py`.
3. The script processes each Excel invoice and generates corresponding PDF invoices in the `PDFs/` directory.

## Dependencies

- Python 3.x
- `pandas` library (install using `pip install pandas`)
- `fpdf` library (install using `pip install fpdf`)

## Limitations and Future Enhancements

- The script currently supports Excel files with a specific naming convention. Future enhancements could include more flexible filename parsing.

- Additional customization features could be added, such as support for including company logos and varying fonts.

## Conclusion

The Invoice to PDF Conversion Script project showcases how automation can streamline the conversion of raw financial data into structured and presentable PDF invoices. This system design forms the basis for further refining and expanding the capabilities of the project.

---
