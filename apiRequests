import requests
import json
response = requests.get("https://api.exchangeratesapi.io/latest?symbols=USD,GBP")

data = response.text
parsed = json.loads(data)
print(json.dumps(parsed, indent =4))
date = parsed["date"]
print(data)
gbp_rate = parsed["rates"]["GBP"]
usd_rate = parsed["rates"]["USD"]
print("On "+ date + " EUR equals " + str(gbp_rate) + " GBP")
print("On " + date + " EUR equals " + str(usd_rate) + " USD")
