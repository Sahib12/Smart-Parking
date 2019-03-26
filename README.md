# Introduction

To create a system through which we can solve the parking problem in our country. Every free space can be used for parking vehicles .These free spaces can be open land, parking area of any building, shopping mall etc. In fact one can lend the residential parking space when they are away for office or holiday.  Solving this problem by using Arduino Boards and Raspberry Pi at parking slots for detecting parked vehicles and developing a hybrid application prototype using Ionic Framework and Cordova which gives the direction to nearest parking spot with details of its location. User can navigate to the available spot using google maps application and also see previous booking details.

# Working

* At each and every parking slot an Arduino board with IR sensor connected to a Raspbery pi is installed, which will be used to detect whether a parking slot is occupied or not.
​
* A node server will run on the raspberry pi which will enable the users to book a parking slot in advance via REST API calls.
​
* A node application will run on the raspberry pi which will continuously send the state of the Infrared sensor (Whether the parking slot is occupied or not) to a centralized database (We have used Firebase Realtime Database).​

* Geohashes are used for storing the location coordinates of these parking slots because geohashes enable us to sort the parking slots according to their coordinates (Latitude and Longitude).​

* A hybrid application is built using Ionic Framework v1 and Cordova. This application will be used by the users to​
Get the list of nearest available parking slots, book a parking slot, get directions to it on google maps and to get the list of their past bookings.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install foobar
```
WQWERT
## Usage

```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon'
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
