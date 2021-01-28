# Read RideOn

This allows an authenticated user to retrieve information on her/his **given** RideOn on a specific activity

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `api/activities/{activityId}/rideon`
 
**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "activityId": "integer id of the activity for which the RideOn was given"
```

## Success Response

**Code** : `200 OK`

**response**
A json object containing the information on the RideOn

```json
{
  "activityId": 123,
  "activityId_str": "123",
  "createDate": "2021-01-20T20:01:16.140+0000",
  "fullName": "Rick Somename",
  "id": 123,
  "id_str": "123",
  "profile": {
    "countryCode": 123,
    "firstName": "Rick",
    "id": 123,
    "id_str": "123",
    "imageSrc": "https://static-cdn.zwift.com/prod/profile/bedd4b6d-123",
    "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/bedd4b6d-123",
    "lastName": "Some Name",
    "playerType": "NORMAL",
    "publicId": "15cc4997-7ee2-450b-a8f1-123",
    "socialFacts": {
      "followerStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
      "isFavoriteOfLoggedInPlayer": False
    }
  },
  "profileId": 123,
  "profileImageUrl": "https://static-cdn.zwift.com/prod/profile/bedd4b6d-123"
}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [RideOns](https://github.com/strukturunion-mmw/zwift-api-documentation/blob/main/README.md#rideons) RideOn related endpoints

- [Endpoints overview](https://github.com/strukturunion-mmw/zwift-api-documentation/blob/main/README.md#known-endpoints) Overview of all documented API endpoints
