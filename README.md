# This module requests information for other websites.
import requests


cityName = input("PLease Enter The City Name:")
print(cityName)
print('Displaying City Weather Report For'+ cityName)


# This puts the city of the user input into the website.
url = "https://wttr.in/" +cityName




# This sends a request to the website.
res = requests.get(url) 
print(res.text)
