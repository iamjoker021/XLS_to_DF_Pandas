# XML to Pandas DataFrame Conversion

This Python script demonstrates how to convert data from an XML file into a Pandas DataFrame, specifying data types for each column based on XML attributes.

## Requirements

- Python 3.x
- Pandas
- xml.etree.ElementTree (usually included in Python's standard library)

## Usage

1. Make sure you have the required dependencies installed.

2. Specify the path of the xls file in xml format

3. Run the notebook

4. The script will parse the XML file, extract the data, infer data types based on XML attributes, and create a Pandas DataFrame.

## How It Works

- The script uses the `xml.etree.ElementTree` library to parse the XML file.
- It extracts data from the XML structure, including data values and data types (specified as XML attributes).
- The extracted data is stored in lists, one for data values and one for data types.
- The script maps XML data types to Pandas data types using a dictionary.
- Finally, it creates a Pandas DataFrame with the specified data types for each column.

## Data Types Mapping

The following data types are mapped from XML to Pandas:

- `String` -> `str`
- `Boolean` -> `bool`
- `Number` -> `float`
- `DateTime` -> `datetime64[ns]`
