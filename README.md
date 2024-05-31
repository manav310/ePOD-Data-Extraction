# ePOD Data Extraction Based on OCR and NLP

## Project Overview
This project focuses on extracting essential data from electronic proof of delivery (ePOD) documents using Optical Character Recognition (OCR) and Natural Language Processing (NLP) techniques. The aim is to streamline the processing of ePOD documents to enhance operational efficiency in logistics and delivery management.

## Features
- **Dataset Acquisition and Preprocessing**: Handling file operations, image enhancement, and annotation.
- **Barcode Detection**: Exploration of various barcode detection libraries.
- **OCR Implementation**: Using libraries like Tesseract and docTR for text extraction.
- **Information Extraction**: Employing regular expressions for key-value pair identification.
- **Data Export**: Exporting the extracted data to an Excel file for further analysis.

## Technologies Used
- **OCR Libraries**: Tesseract, docTR
- **Barcode Detection Libraries**: pyzbar, ZXing, Dynamsoft Barcode Reader
- **Programming Languages**: Python
- **Image Processing**: OpenCV
- **Data Manipulation**: Pandas

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/epod-data-extraction.git
    cd epod-data-extraction
    ```
2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. **Dataset Preparation**:
    - Place your ePOD images in the `data/` directory.
    - Run the preprocessing script:
      ```bash
      python preprocess_data.py
      ```
2. **Barcode Detection**:
    - Execute the barcode detection script:
      ```bash
      python detect_barcodes.py
      ```
3. **OCR and Data Extraction**:
    - Perform OCR on the images:
      ```bash
      python perform_ocr.py
      ```
    - Extract key-value pairs from the text:
      ```bash
      python extract_information.py
      ```
4. **Export Data**:
    - Export the extracted data to an Excel file:
      ```bash
      python export_data.py
      ```

## Project Structure
- `data/`: Directory containing the ePOD images.
- `scripts/`: Directory containing the preprocessing, barcode detection, OCR, and data extraction scripts.
- `output/`: Directory where the extracted data and results are stored.
- `requirements.txt`: File listing the required Python packages.

## Results
The project demonstrated the feasibility of automating the extraction of essential data from ePOD documents. docTR was identified as the preferred OCR library due to its superior performance on various document formats.

## Recommendations
- Further exploration of machine learning models and domain-specific approaches can enhance text extraction accuracy.
- Using paid APIs like AWS Textract and Google Vision could provide a comprehensive solution for text detection and extraction.

## Conclusion
This project showcases the potential of OCR and NLP in automating data extraction from ePOD documents, paving the way for future advancements in document processing and analysis.

## Acknowledgements
Special thanks to the eShipz team for their guidance and support throughout this project.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any questions or feedback, please contact [Your Name] at [your.email@example.com].
