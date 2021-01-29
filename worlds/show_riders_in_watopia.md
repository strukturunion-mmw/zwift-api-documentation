# List all Riders in Watopia

This allows an authenticated user to show show all current riders in Watopia public world, including their current riding
stats, their sub-word (map) etc. 

**CAUTION:**

*This can be a **huuuuge** dataset! On a busy time with 30.000+ riders on ZWIFT you get stats for ALL of them*

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `relay/worlds/1`

**Method** : `GET`

**Auth required** : True

## Success Response

**Code** : `200 OK`

**response**
A json object containing the current riders in Watopia

```json
{
  "status": "200: OK",
  "response": {
    "worldId": 1,
    "name": "Public Watopia",
    "playerCount": 14275,
    "currentWorldTime": 197906586595,
    "currentDateTime": 1611922660,
    "friendsInWorld": [
      {
        "playerId": 87767,
        "firstName": "Jim",
        "lastName": "Donovan",
        "male": true,
        "countryISOCode": 840,
        "totalDistanceInMeters": 10231,
        "rideDurationInSeconds": 1059,
        "playerType": "ZWIFT_STAFF",
        "followerStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
        "rideOnGiven": false,
        "currentSport": "CYCLING",
        "enrolledZwiftAcademy": false,
        "mapId": 1,
        "ftp": 290,
        "runTime10kmInSeconds": 2614
      },
      {
        "playerId": 2161,
        "firstName": "Phillis",
        "lastName": "Huntington",
        "male": true,
        "countryISOCode": 901,
        "totalDistanceInMeters": 31886,
        "rideDurationInSeconds": 2859,
        "playerType": "NORMAL",
        "followerStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
        "rideOnGiven": false,
        "currentSport": "CYCLING",
        "enrolledZwiftAcademy": false,
        "mapId": 2,
        "ftp": 317,
        "runTime10kmInSeconds": 3600
      }
    ]
  }
}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [Worlds](../README.md#worlds) Rider Profile related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
