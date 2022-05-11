# homebridge-skodaconnect
Control your locks on your Skoda Car via SkodaConnect-API


# config.json

```
{
        "accessory": "SkodaConnect",
        "name": "My Car",
        "vin": "ABC123",
        "username": "youremail@domain.com",
        "password": "ABC123"
}
```

## Configuration Params

|             Parameter            |                       Description                       | Required |
| -------------------------------- | ------------------------------------------------------- |:--------:|
| `name`                           | name of the accessory                                   |     ✓    |
| `vin`                            | vin number of the car                                   |          |
| `username`                       | username for SkodaConnect service                       |     ✓    |
| `password`                       | password for SkodaConnect service                       |     ✓    |


## Basic Auth

This is a fork from the original script written by gadget-man (homebridge-bmw-connected)

These API calls are designed to allow you to interact with your SkodaConnect Account. They were reverse engineered from [the official Skoda/VW Connect Website](https://www.msg-volkswagen.de/).

Your use of these API calls is entirely at your own risk.  They are neither officially provided nor sanctioned.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

In order to authenticate against the API you will need to be registered on [SkodaConnect](https://www.skoda-auto.com/connectivity/myskoda-app).

You will need:

1. Your SkodaConnect registered email address.
2. Your SkodaConnect registered password.


You can get the client_id details from either decompiling the Android App or from intercepting communications between your phone and the Volkswagen server.  This is left as an exercise for the reader ☺

## Help

  - Make sure to specify all parameters

## Installation

1. Install homebridge using: `npm install -g homebridge`
2. Install this plugin using: `npm install -g homebridge-skodaconnect`
3. Update your config file
