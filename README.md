# StockMarketApp

This Flask web application is designed to return real-time stock market information from api.marketstack.com API to users in WhatsApp using Twilio. The application is built using Python 3 and Flask, and integrates with the Twilio messaging API to enable users to receive updates on the stock market in real-time.

# Prerequisites
Before you can use this application, you will need to obtain an API key from both api.marketstack.com and Twilio. You can sign up for a free account at api.marketstack.com to obtain an API key for accessing real-time stock market information. Similarly, you will need to sign up for a Twilio account and obtain an account SID, auth token, and a Twilio phone number to enable messaging to and from the application.

# Installation
1. Clone this repository onto your local machine.

2. Create a virtual environment for the application using your preferred method. For example, using virtualenv:

		virtualenv env
		source env/bin/activate

3. Install the required packages using pip:

		pip install -r requirements.txt
		
4. Create a .env file in the root directory of the project and add the following environment variables:

		MARKETSTACK_API_KEY=<your-marketstack-api-key>
		TWILIO_ACCOUNT_SID=<your-twilio-account-sid>
		TWILIO_AUTH_TOKEN=<your-twilio-auth-token>
		TWILIO_PHONE_NUMBER=<your-twilio-phone-number>
		
5. Run the application using the following command:

		flask run
		
# Usage
i)To use the application, you will need to have a WhatsApp account and have added the Twilio phone number as a contact in your WhatsApp account.

ii)Send a message to the Twilio phone number in WhatsApp with the symbol of the stock you want information about, for example, "AAPL" for Apple Inc.
			The application will return the current stock market information for the specified symbol in a message to your WhatsApp account.
# Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request.

