- 👋 Hi, I’m @Saifullah98309
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Saifullah98309/Saifullah98309 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
from geopy.geocoders import Nominatim

def get_location(address):
    geolocator = Nominatim(user_agent="location_tracker")
    location = geolocator.geocode(address)
    
    if location:
        print(f"Address: {address}")
        print(f"Latitude: {location.latitude}")
        print(f"Longitude: {location.longitude}")
    else:
        print(f"Location not found for address: {address}")

if __name__ == "__main__":
    address = input("Enter the address you want to track: ")
    get_location(address)
