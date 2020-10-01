# FAÇA UMA CONTA NO APIGEE - VÁ EM SPECS - NEW

# DEFINIÇÃO DO NOSSO RUNNING EXAMPLE
## WHEATER STACK - GET CURRENT WHEATER TIME
- Faça uma conta em https://weatherstack.com/dashboard
- Copie sua chave de API
- PARAMETROS DA REQUEST: 
    ```
    http://api.weatherstack.com/current
        ? access_key = YOUR_ACCESS_KEY
        & query = Jacarei
    ```
- Objeto de resposta:
  ```
  {
    "request": {
        "type": "City",
        "query": "Jacarei, Brazil",
        "language": "en",
        "unit": "m"
    },
    "location": {
        "name": "Jacarei",
        "country": "Brazil",
        "region": "Sao Paulo",
        "lat": "-23.317",
        "lon": "-45.967",
        "timezone_id": "America/Sao_Paulo",
        "localtime": "2020-09-30 19:57",
        "localtime_epoch": 1601495820,
        "utc_offset": "-3.0"
    },
    "current": {
        "observation_time": "10:57 PM",
        "temperature": 24,
        "weather_code": 386,
        "weather_icons": [
            "https://assets.weatherstack.com/images/wsymbols01_png_64/wsymbol_0016_thundery_showers.png"
        ],
        "weather_descriptions": [
            "Thunderstorm"
        ],
        "wind_speed": 41,
        "wind_degree": 190,
        "wind_dir": "S",
        "pressure": 1017,
        "precip": 0,
        "humidity": 61,
        "cloudcover": 75,
        "feelslike": 24,
        "uv_index": 9,
        "visibility": 10,
        "is_day": "yes"
    }
  }
  ```