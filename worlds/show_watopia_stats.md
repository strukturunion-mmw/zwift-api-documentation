# Show Watopia Stats

This allows an authenticated user to show current stats on Watopia public world, like rider-count, time or date

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `/relay/worlds`

**Method** : `GET`

**Auth required** : True

## Success Response

**Code** : `200 OK`

**response**
A json object containing the rider's profile information

```json
{
  "status": "200: OK",
  "response": [
    {
      "worldId": 1,
      "name": "Public Watopia",
      "playerCount": 14262,
      "currentWorldTime": 197906487970,
      "currentDateTime": 1611922562,
      "friendsInWorld": []
    }
  ]
}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [Worlds](../README.md#worlds) Rider Profile related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
