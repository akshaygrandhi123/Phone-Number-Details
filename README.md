# Phone Number Analyzer

This Python script uses the `phonenumbers` library to analyze a given phone number and provide information about its timezone, carrier, and geographic location.

## Installation

1. Ensure you have Python installed on your system. This script was tested with Python 3.9, but should work with other versions as well.

2. Install the `phonenumbers` library using pip:

   ```
   pip install phonenumbers
   ```

## Usage

1. Clone the repository to your local machine:

   ```
   git clone https://github.com/your-username/phone-number-analyzer.git
   ```

2. Navigate to the project directory:

   ```
   cd phone-number-analyzer
   ```

3. Run the script:

   ```
   python phone_number_analyzer.py
   ```

4. When prompted, enter a phone number in the format `+[country code] [number]`, for example, `+1 1234567890`.

5. The script will then output the following information:

   - The parsed phone number object
   - The timezone(s) associated with the phone number
   - The carrier name
   - The geographic location description

## Code Explanation

The code uses the following functions from the `phonenumbers` library:

- `phonenumbers.parse(number)`: Parses the input phone number into a `phonenumbers.PhoneNumber` object.
- `timezone.time_zones_for_number(phone)`: Retrieves the timezone(s) associated with the phone number.
- `carrier.name_for_number(phone, "en")`: Retrieves the carrier name for the phone number (in English).
- `geocoder.description_for_number(phone, "en")`: Retrieves the geographic location description for the phone number (in English).

The script then prints the obtained information to the console.

## Contributions

If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/your-username/phone-number-analyzer).
