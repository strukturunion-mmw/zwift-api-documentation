# List any rider's followees

This allows an authenticated user to list all riders being followed by a specific rider

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `api/profiles/{riderId}/followees`

**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "riderId": "integer id of the rider for whom the followee-list is requested"
```

## Success Response

**Code** : `200 OK`

**response**
A json object containing a list of followees

```json
{
      "id": 0,
      "followerId": 33318,
      "followeeId": 19130,
      "status": "IS_FOLLOWING",
      "isFolloweeFavoriteOfFollower": false,
      "followerProfile": null,
      "followeeProfile": {
        "id": 1918830,
        "publicId": "d5e60d96-a519-4362-b6e4-899a3332c",
        "firstName": "Jim",
        "lastName": "Canto",
        "male": true,
        "imageSrc": "https://static-cdn.zwift.com/prod/profile/a2e5fa-1084316",
        "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/a2f73a-1084316",
        "playerType": "NORMAL",
        "countryAlpha3": "che",
        "countryCode": 756,
        "useMetric": true,
        "riding": false,
        "privacy": {
          "approvalRequired": false,
          "displayWeight": false,
          "minor": false,
          "privateMessaging": false,
          "defaultFitnessDataPrivacy": false,
          "suppressFollowerNotification": false,
          "displayAge": true,
          "defaultActivityPrivacy": "PUBLIC"
        },
        "socialFacts": {
          "profileId": 19130,
          "followersCount": 171,
          "followeesCount": 468,
          "followeesInCommonWithLoggedInPlayer": 0,
          "followerStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
          "followeeStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
          "isFavoriteOfLoggedInPlayer": false
        },
        "worldId": null,
        "enrolledZwiftAcademy": false,
        "playerTypeId": 1,
        "playerSubTypeId": null,
        "currentActivityId": null
      }
    },
    {
      "id": 0,
      "followerId": 33318,
      "followeeId": 1330,
      "status": "IS_FOLLOWING",
      "isFolloweeFavoriteOfFollower": true,
      "followerProfile": null,
      "followeeProfile": {
        "id": 131930,
        "publicId": "7955d011-a74b-46f9-a8b6-02a099d20",
        "firstName": "Janna",
        "lastName": "Hastings",
        "male": true,
        "imageSrc": "https://static-cdn.zwift.com/prod/profile/70c929-165146",
        "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/70c9d92165146",
        "playerType": "NORMAL",
        "countryAlpha3": "che",
        "countryCode": 756,
        "useMetric": true,
        "riding": false,
        "privacy": {
          "approvalRequired": true,
          "displayWeight": false,
          "minor": false,
          "privateMessaging": false,
          "defaultFitnessDataPrivacy": false,
          "suppressFollowerNotification": false,
          "displayAge": true,
          "defaultActivityPrivacy": "PUBLIC"
        },
        "socialFacts": {
          "profileId": 1330,
          "followersCount": 3,
          "followeesCount": 3,
          "followeesInCommonWithLoggedInPlayer": 0,
          "followerStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
          "followeeStatusOfLoggedInPlayer": "NO_RELATIONSHIP",
          "isFavoriteOfLoggedInPlayer": false
        },
        "worldId": null,
        "enrolledZwiftAcademy": false,
        "playerTypeId": 1,
        "playerSubTypeId": null,
        "currentActivityId": null
      }
    },
}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [Rider Profiles](../README.md#rider-profiles) Rider Profile related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
