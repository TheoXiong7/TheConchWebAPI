# The Conch - Web API Documentation

Theo Xiong, Oliver Moscow
```
Base URL > https://www.sch.codes/api
```
## datatype [user]
```
Params:
	spotify_email
	username
	user_stations
```
## datatype [station]
```
Params:
	station_id
	station_name
	muxplayback_id
	muxstream_id
```
## endpoint [/new_user]
```
Methods > POST
Request Params >
	api_key[str]
	spotify_email[str]
	username[str] : letters and numbers only, no spaces or special characters
Return Params > 
	status[str]
```
```
Example > curl https://www.sch.codes/api/new_user?api_key=key&spotify_email=johndoe%40gmail.com&username=johndoe123
```
## endpoint [/get_user_stations]
```
Methods > POST, GET
Request Params >
	api_key[str]
	spotify_email[str]
Return Params > 
	user_stations[list]
```
```
Example > https://www.sch.codes/api/get_user_stations?api_key=key&spotify_email=johndoe%40gmail.com
```
## endpoint [/create_station]
```
Methods > POST
Request Params >
	api_key[str]
	spotify_email[str]
	station_name[str]
	muxplayback_id[str]
	muxstream_id[str]
Return Params > 
	stationid[num] or error[str]
```
```
Example > https://www.sch.codes/api/create_station?api_key=key&spotify_email=johndoe%40gmail.com&station_name=Country+Poppin&muxplayback_id=sampleid&muxstream_id=sampleid
```
## endpoint [/get_station_info]
```
Methods > POST, GET
Request Params >
	api_key[str]
	station_id[int]
Return Params > 
	{station_name[str],
	muxplayback_id[str],
	muxstream_id[str]}
```
```
Example > https://www.sch.codes/api/get_station_info?api_key=key&station_id=543213213
```
