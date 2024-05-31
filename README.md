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
2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. **Dataset Preparation**:
    - Place your ePOD images in the `data/` directory.
    - Run the `epod_image_installer.ipynb` notebook to preprocess the images.
2. **Barcode Detection**:
    - Execute the `image_classification.ipynb` notebook to classify and detect barcodes.
3. **OCR and Data Extraction**:
    - Perform OCR on the images using the `data_extraction.ipynb` notebook.
4. **Export Data**:
    - Export the extracted data to an Excel file by running the final cells in the `data_extraction.ipynb` notebook.

## Project Structure
- `data/`: Directory containing the ePOD images.
- `notebooks/`: Directory containing the Jupyter notebooks for preprocessing, barcode detection, and data extraction.
  - `epod_image_installer.ipynb`: Notebook for preprocessing ePOD images.
  - `image_classification.ipynb`: Notebook for classifying images and detecting barcodes.
  - `data_extraction.ipynb`: Notebook for performing OCR and extracting data.
- `requirements.txt`: File listing the required Python packages.
- `output/`: Directory where the extracted data and results are stored.

## Results
The project demonstrated the feasibility of automating the extraction of essential data from ePOD documents. docTR was identified as the preferred OCR library due to its superior performance on various document formats.

## Recommendations
- Further exploration of machine learning models and domain-specific approaches can enhance text extraction accuracy.
- Using paid APIs like AWS Textract and Google Vision could provide a comprehensive solution for text detection and extraction.

## Conclusion
This project showcases the potential of OCR and NLP in automating data extraction from ePOD documents, paving the way for future advancements in document processing and analysis.

## Acknowledgements
Special thanks to the eShipz team for their guidance and support throughout this project.
