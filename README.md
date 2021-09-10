# The Conch - Web API Documentation

This documentation is made to help understand The Conch's Web API.
```
Base URL > https://www.sch.codes/api
```
## /sendaudio
```
Description > Use this endpoint to send audio chunk to a user's .
Methods > POST, PUT
```
```
Usage > https://www.sch.codes/api/sendaudio/<key>/<username>/<audiofile>
	key --> API Key
	username --> Username
	audiofile --> Audio File
```
## /getaudiolist
```
Description > Use this endpoint to retrieve all audios of a user.
Methods > GET
```
```
Usage > https://www.sch.codes/api/getaudiolist/<key>/<username>/
	key --> API Key
	username --> Username
```
## /getallusers
```
Description > Use this endpoint to retrieve id of all users.
Methods > GET
```
```
Usage > https://www.sch.codes/api/getallusers/<key>/
	key --> API Key
```
## /getuser
```
Description > Use this endpoint to retrieve user information.
Methods > POST, GET
```
```
Usage > https://www.sch.codes/api/getuser/<key>/<username>
	key --> API Key
	username --> Username
```
~~## /addtolist~~
```
Description > Use this endpoint to add track to user playlist.
Methods > POST
```
```
Usage > https://www.sch.codes/api/addtolist/<key>/<username>/<track>
	key --> API Key
	username --> Username
	track --> Title of track
```
## Errors
```
{'Error' : 'null key'}
{'Error' : 'null username'}
{'Error' : 'Song exists in playlist.'}
```
## User Data Structure
```
{
	'Username' : 'username<str>',
	'FullName' : 'fullname<str>',
	'Stations' : 'stations<list>',
	'FollowingStations' : 'followingstations<list>',
	'SignupDate' : 'signupdate<str>',
}
```
## Radio Station Data Structure
```
{
	'StationID' : 'stationid<str>',
	'StationName' : 'stationname<str>',
	'Playlist' : 'playlist<url>',
	'FollowsCount' : 'followscount<int>'
}
```
