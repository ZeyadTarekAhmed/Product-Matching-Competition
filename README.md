# Product Matching System

This project is a Python-based product matching system that combines text similarity and price similarity to match products from a dataset to a master product file. The system is optimized for high accuracy and performance.

## Features
- Cleans and normalizes Arabic text for better text similarity matching.
- Uses TF-IDF vectorization and cosine similarity for text matching.
- Computes price similarity based on relative price differences.
- Combines text and price similarity scores (25% text, 75% price) for optimal matching.
- Outputs results with confidence scores and matching statistics.

## Installation

### Prerequisites
Ensure you have the following installed:
- Python 3.x
- pip
- Git

### Required Libraries
Install the required Python libraries using:
```sh
pip install pandas numpy scikit-learn openpyxl
```

## Usage

### 1. Clone the Repository
```sh
git clone https://github.com/yourusername/product-matching-system.git
cd product-matching-system
```

### 2. Prepare the Input Data
Ensure you have an Excel file named `Product Matching Dataset.xlsx` in the project directory. The file should contain two sheets:
- **Master File**: `sku`, `product_name_ar`, `price`
- **Dataset**: `sku`, `seller_item_name`, `price`

### 3. Run the Script
Execute the following command:
```sh
python match_products.py
```

### 4. Output
The script will generate an output Excel file named `Combined_Matching_Results.xlsx` containing:
- Dataset SKU and seller product details
- Matched SKU from the master file
- Text and price similarity scores
- Final combined score

### 5. Testing
To test the script, put a test data different from my input remove comment (#) from line 79 to 81 and 166to 167 and put your dataset paths to more info about mechanism take a look on the slides file.

## Contributing
Feel free to fork the repository and submit pull requests with improvements.

## License
This project is licensed under the MIT License.

## Submission
After setting up the repository and running the script successfully, submit the GitHub repository URL in the required form.

