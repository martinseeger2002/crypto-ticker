# Import required libraries
import requests
import json
from tkinter import *

# Set the URLs for the prices
litecoin_url = "https://min-api.cryptocompare.com/data/price?fsym=LTC&tsyms=USD"
dogecoin_url = "https://min-api.cryptocompare.com/data/price?fsym=DOGE&tsyms=USD"
bitcoin_url = "https://min-api.cryptocompare.com/data/price?fsym=BTC&tsyms=USD"

# Get the prices from the URLs
litecoin_price = requests.get(litecoin_url).json()
dogecoin_price = requests.get(dogecoin_url).json()
bitcoin_price = requests.get(bitcoin_url).json()

# Set up the Tkinter window
root = Tk()
root.geometry("300x100")
root.title("Cryptocurrency Prices")

# Create the labels for the prices
Label(root, text="Litecoin price: $" + str(litecoin_price['USD']), font=("Arial", 16)).pack()
Label(root, text="Dogecoin price: $" + str(dogecoin_price['USD']), font=("Arial", 16)).pack()
Label(root, text="Bitcoin price: $" + str(bitcoin_price['USD']), font=("Arial", 16)).pack()

# Run the Tkinter event loop
root.mainloop()
