<h1 align="center">
  Vienna Smart Meter
</h1>
<h4 align="center">An unofficial python wrapper for the <a href="https://www.wienernetze.at/smartmeter" target="_blank">Wiener Netze Smart Meter</a> private API.
</h4>

## Fork

This is a fork of https://github.com/platysma/vienna-smartmeter
As the original Repo is broken and no longer maintained, I try to keep on track with API-changes of Wiener Netze.
- async-client is currently not maintained and most likely broken
- additional endpoints have been added (as the Wiener Netze API changed)
- possible future developement: Wiener Netze offers an Endpoint named "Benachrichtigungen". This is currently not implemented

## Features

- Access energy usage for specific meters
- Get profile information
- View, create & delete events (Ereignisse)

## Installation

Install with pip:

`pip install 'vienna-smartmeter @ git+https://github.com/fleinze/vienna-smartmeter.git'`

## How To Use

Import the Smartmeter client, provide login information and access available api functions:

```python
from vienna_smartmeter import Smartmeter

username = 'YOUR_LOGIN_USER_NAME'
password = 'YOUR_PASSWORD'

api = Smartmeter(username, password)
print(api.profil())
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Make sure to add or update tests as appropriate.

## License

This project is licensed under the terms of the **MIT** license.

## Legal

Disclaimer: This is not affliated, endorsed or certified by Wiener Netze. This is an independent and unofficial API. Strictly not for spam. Use at your own risk.
