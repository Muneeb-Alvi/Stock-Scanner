# Stock-Scanner
This is a stock insight and sentiment analyzer used to provide real-time financial data and news sentiment analysis for publicly traded companies. It fetches ask and bid prices, percentage changes and aggregates news sentiment to help users understant the current state of the market. However, it SHOULD NOT be used as the sole tool to base financial decisions on and the infromation provided by the analyzer is NOT financial advice.

The way it works is, you type in the ticker for a stock in lower case and the program will make requests to both APIs to gather the relevant data and then output the ticker, ask price, bid price, relevant news and sentiment.

## APIs Used
### Aletheia API: 
It was used for retrieving ask prices, bid prices and percentage changes of the chosen stock. I chose this API because it had a high daily request limit and it also had a comprehensive datasent with reliable financial metrics which are important for accurate market analysis.
#### API Docs: [Aletheia Docs](https://aletheiaapi.com/docs/#stock-data)

### Marketaux API: 
It was used for gathering news related to the chosen stock and analyzing the sentiment of the news. I chose this API because it also had a high daily request limit and it was more focused on financial news compared to other news APIs. It also provides sentiment analysis of the news for the chosen stock which is valuable if you want to understant trends and impacts in the market.
#### API Docs: [Marketaux Docs](https://www.marketaux.com/documentation)

## How to Use the Feature
### Setup:
* Install Jupyter
* Install the required Python packages: requests.
* Clone this repository to your local machine.

### Configuration:
* Open the Stock_Scanner.ipynb notebook in Jupyter.
* Locate the cell where API keys are set up.
* Replace the API keys present with your actual API keys from Aletheia and MarketAux respectively.
* From your command line in the project directory, run `jupyter notebook`
* This will open Jupyter in your web browser.
* You can now run the notebook cells one by one to interact with the stock data and sentiment analysis features.
* Input the stock symbol when prompted, or type 'quit' to exit the application.

### Prerequisites:
* You will need valid API keys for both [Aletheia](https://aletheiaapi.com/) and [MarketAux](https://www.marketaux.com/), which you can obtain by registering on their respective websites.
* Jupyter and the requests library installed on your machine.
