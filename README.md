import requests

#Function to fetch the latest exchange rates
 def get exchange rates():
api_key="90f49c4598674adc95f311407c7497a7"
url="https://openexchangerates.org/api/latest.json?app_id={api_key}"
response=requests.get(url) data=response.json()

return datal ["rates"]

#Function to convert the currency

det convert currency (amount, from currency, to currency, exchange rates): 
if from_currency ==to currency:

return amount

If from_currency != "USD":
it amount /=exchange_rates [from_currency]
amount*=exchange_rates[to_currency] 

Main program

def main():

exchange_rates=get_exchange rates()

amount=float(input("Enter the amount: "))

from_currency=input("Enter the currency you want to convert from (e.g., usb)=="),upper() 
to_currency=input("Enter the currency you want to convert to (e.g., EUR):").upper()

converted_amount=convert_currency(amount, from_currency, to_currency, exchange_rates) print(f"{amount} {from_currency} = {converted_amount} {to_currency}")
#Run the program
If_name_=="_main_"
main()
