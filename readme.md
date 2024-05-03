

# Bill Generator

The **Bill Generator** is a Python tool designed to parse text input containing information about purchased items and generate a bill. It utilizes regular expressions to extract relevant data such as product names, quantities, and prices from the input text.

## Features

- Extracts product information from text input
- Handles numbers written as words (e.g., 'one', 'two', etc.)
- Supports conversion of comma-separated numbers to floats
- Excludes specific words from product names (e.g., 'kilo', 'dollar', etc.)
- Prints the bill in a tabular format
- Converts the bill data into a pandas DataFrame

## Installation

1. Clone the repository to your local machine:

```bash
git clone https://github.com/example/bill-generator.git
```

2. Navigate to the project directory:

```bash
cd bill-generator
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

1. Import the `BillGenerator` class from the `bill_generator.py` module into your Python script or interactive environment:

```python
from bill_generator import BillGenerator
```

2. Create an instance of the `BillGenerator` class with the text containing the purchase information as the input:

```python
text = "I bought three Samsung smartphones 150 $ each, four kilos of fresh banana for 1,2 dollar a kilogram, and one Hamburger with 4,5 dollar"
bill = BillGenerator(text)
```

3. Print the bill using the `printBill()` method:

```python
bill.printBill()
```

4. Optionally, convert the bill data into a pandas DataFrame using the `toDF()` method:

```python
bill_df = bill.toDF()
print(bill_df)
```

## Examples

Here's an example of how to use the Bill Generator:

```python
from bill_generator import BillGenerator

# Text containing purchase information
text = "I bought three Samsung smartphones 150 $ each, four kilos of fresh banana for 1,2 dollar a kilogram, and one Hamburger with 4,5 dollar"

# Create a BillGenerator instance
bill = BillGenerator(text)

# Print the bill
bill.printBill()

# Convert bill data to a DataFrame
bill_df = bill.toDF()
print(bill_df)
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

You may need to adjust the installation instructions or other details based on your specific setup and requirements.
