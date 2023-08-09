# Invoice to PDF Conversion Script

This repository contains a Python script that automates the conversion of invoice data from Excel files in the "invoices" folder to visually organized PDF invoices in the "PDFs" folder. Each PDF invoice is generated based on the data in the corresponding Excel file.

## Files

1. `invoice_to_pdf.py`: This Python script reads Excel files from the "invoices" folder, extracts invoice data, and generates PDF invoices in the "PDFs" folder. The generated PDFs include invoice number, date, product details, and total sum.

2. `invoices/`: This directory contains Excel files (invoices) that include invoice data. The filenames follow the format "InvoiceNumber-Date.xlsx".

3. `PDFs/`: This directory is where the generated PDF invoices will be stored.

## Usage

1. Place the Excel invoice files in the "invoices" folder.
2. Install the required library: `pandas`, `fpdf` (install using `pip install pandas fpdf`).
3. Run the script using the command: `python invoice_to_pdf.py`.
4. The script will process the Excel files and generate corresponding PDF invoices in the "PDFs" folder.

## Features

- **Automated Conversion**: The script streamlines the conversion of Excel invoices to PDFs, saving time and effort.

- **Customizable Layout**: The generated PDF invoices include invoice number, date, product details, and total sum. The layout can be customized to meet specific branding or design requirements.

## Dependencies

- Python 3.x
- `pandas` library (install using `pip install pandas`)
- `fpdf` library (install using `pip install fpdf`)

## Limitations and Future Enhancements

- The script currently supports Excel files with a specific naming convention ("InvoiceNumber-Date.xlsx"). Future enhancements could include flexible filename parsing.

- Enhancements can be made to add support for additional customization, such as company logo inclusion and different fonts.

## Conclusion

The Invoice to PDF Conversion Script project showcases the power of automation in transforming raw invoice data into organized and visually appealing PDF invoices. This tool is designed to improve efficiency in invoice management.

---
