This allows an authenticated user to give another rider a **rideOn**

A rideOn record, once set/given looks like this, See get_rideOn for information on how to get a rideOn record.

**rideOn record example**

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

**URL** : `api/profiles/{profileId}/activities/{activityId}/rideon`

**Method** : `POST`

**Auth required** : True

**Data constraints**

```json
{
  "‘profileId’": "integer id of the currently authenticated user giving the rideOn"
}
```

**Data example**

```json
{‘profileId’: 1234}
```

## Success Response

**Code** : `200 OK`

**response**
An empty json

```json
{}
```
