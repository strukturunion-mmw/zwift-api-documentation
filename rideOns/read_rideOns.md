# Read RideOn

This allows an authenticated user to retrieve information on all **given** RideOns on a specific activity

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `/api/activities/{activityId}/rideon`

**Alternative Endpoint** : `/api/profiles/{riderId}/activities/{activityId}/rideon`
 
**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "activityId": "integer id of the activity for which the RideOn was given"

  "riderId": "integer id of the rider to whom the RideOn was given"
```

## Success Response

**Code** : `200 OK`

**response**
A json object containing a list of the given RideOns to the rider in the activity

```json
{
    {
      "id_str": "103928038",
      "id": 103920038,
      "activityId": 73762431571836900,
      "activityId_str": "73762431571836912",
      "profileId": 55125215,
      "fullName": "Alberto Zinga",
      "profileImageUrl": "https://static-cdn.zwift.com/prod/profile/37b48c0-545829",
      "profile": {
        "id_str": "55125215",
        "id": 55125215,
        "publicId": "6a651090-37fb-40ea-a3f6-ab48bff1e8f",
        "firstName": "Alberto",
        "lastName": "Zinga",
        "imageSrc": "https://static-cdn.zwift.com/prod/profile/37b4c0-545829",
        "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/37b4c0-545829",
        "countryCode": 56,
        "playerType": "NORMAL",
        "socialFacts": {
          "followerStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
          "isFavoriteOfLoggedInPlayer": false
        }
      },
      "createDate": "2021-01-28T15:48:55.326+0000"
    },
    {
      "id_str": "1039096887",
      "id": 1039096887,
      "activityId": 737624331571836900,
      "activityId_str": "737624331571836912",
      "profileId": 3649459,
      "fullName": "Ronni Rouleur",
      "profileImageUrl": "https://static-cdn.zwift.com/prod/profile/de873b18-1901594",
      "profile": {
        "id_str": "3649459",
        "id": 3649459,
        "publicId": "e9f441c0-7a08-4b0e-8fd1-2ca7d81d263c",
        "firstName": "Ronni",
        "lastName": "Rouleur",
        "imageSrc": "https://static-cdn.zwift.com/prod/profile/de873b18-1901594",
        "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/de873b18-1901594",
        "countryCode": 250,
        "playerType": "NORMAL",
        "socialFacts": {
          "followerStatusOfLoggedInPlayer": "SELF",
          "isFavoriteOfLoggedInPlayer": false
        }
      },
      "createDate": "2021-01-28T15:04:31.283+0000"
    }
}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [RideOns](../README.md#rideons) RideOn related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
