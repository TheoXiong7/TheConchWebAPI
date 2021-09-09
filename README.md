# The Conch - Web API Documentation

This documentation is made to help understand The Conch's Web API.
```
Base URL > https://www.sch.codes/api
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
```
Example:
	In > https://www.sch.codes/api/getuser/<key>/joe3000

	Out > {"Name":"Joe Mama","Playlist":"['Change - J. Cole', 'These Walls - Kendrick Lamar', 'Ghostown - Kanye West/PARTYNEXTDOOR', 'I wonder - Kanye West']","Username":"joe3000"}
```
## /addtolist
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
```
Example:
	In > https://www.sch.codes/api/addtolist/<key>/joe3000/Family Business - Kanye West

	Out > {"Success":"Song added to playlist."}
```
## Errors
```
{'Error' : 'null key'}
{'Error' : 'null username'}
{'Error' : 'Song exists in playlist.'}
```
