# CurrencyConvert
Currency Exchange Rate Converter
This is a simple Flask application that converts one currency to another currency based on the latest exchange rate using the Alpha Vantage API.





How to run the application
Clone the repository and navigate to the root folder.
Create a virtual environment using python -m venv venv command and activate it using source venv/bin/activate (on Linux/Mac) or venv\Scripts\activate (on Windows).
Install the required packages using pip install -r requirements.txt.
Set your Alpha Vantage API key as the API_KEY variable in app.py.
   (Steps:
      1. Go to the Alpha Vantage website and create an account if you don't have one already.
      2. After you've logged in, navigate to the API Documentation page.
      3. Scroll down to the "Currency Exchange Rates" section and click on the "Get your free API key today" button.
      4. Follow the instructions to generate your API key. You should receive an email with the API key shortly after you complete the form.
      5. Copy the API key from the email or from the Alpha Vantage website.
      6. Open app.py in a text editor and find the line that says API_KEY = 'GDC2AES9MZ33F6W4'.
      7. Replace the value 'GDC2AES9MZ33F6W4' with your API key (enclosed in quotes).
      8. Save the file.)
Run the application using python app.py.
Open your web browser and navigate to http://127.0.0.1:5000/.
Enter the amount, the source currency, and the target currency, and click the "Convert" button to get the result.






Files in the repository
app.py - This is the main Python file that contains the Flask application.
templates/home.html - This is the HTML template for the home page of the application.
requirements.txt - This file contains a list of the required packages to run the application.





How it works
The application has a single route, /, which handles both GET and POST requests. When the user submits the form, the application sends a request to the Alpha Vantage API to get the latest exchange rate between the two currencies. It then calculates the result based on the exchange rate and the amount entered by the user. The result is rounded to two decimal places and displayed on the home page along with the exchange rate, the source currency code and name, the target currency code and name, and the last refreshed time. If an error occurs, a "Bad Request" message is displayed on the home page.

License
