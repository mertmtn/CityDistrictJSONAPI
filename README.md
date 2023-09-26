# CityDistrictJSONAPI

This repository created all city and its districts of Türkiye as JSON format. 

All data retrieved from https://www.e-icisleri.gov.tr/Anasayfa/MulkiIdariBolumleri.aspx link on 26.09.2023

## Installation

It published Github Pages like an API
[https://mertmtn.github.io/CityDistrictJSONAPI/all-city-district.json](https://mertmtn.github.io/CityDistrictJSONAPI/all-city-district.json)

## Usage

```javascript
getCityCount("https://mertmtn.github.io/CityDistrictJSONAPI/city-district.json");

async function getCityCount(file) {
  let response = await fetch(file);
  let responseJson = await response.json();  
  console.log(responseJson.cityCount); //Result : 81
}
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.
