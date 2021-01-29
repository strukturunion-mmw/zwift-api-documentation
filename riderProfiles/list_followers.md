# List any rider's followers

This allows an authenticated user to list all riders that follow a specific rider

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `/api/profiles/{riderId}/followers`

**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "riderId": "integer id of the rider for whom the follower-list is requested"
```

## Success Response

**Code** : `200 OK`

**response**
A json object containing a list of followers

```json
{
      "id": 0,
      "followerId": 33514,
      "followeeId": 33388,
      "status": "IS_FOLLOWING",
      "isFolloweeFavoriteOfFollower": false,
      "followerProfile": {
        "id": 33514,
        "publicId": "523d2814-ec6f-4919-836d-c65c8c5fc1",
        "firstName": "John",
        "lastName": "Doe",
        "male": true,
        "imageSrc": null,
        "imageSrcLarge": null,
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
          "profileId": 3314,
          "followersCount": 1,
          "followeesCount": 1,
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
      },
      "followeeProfile": null
    },
    {
      "id": 0,
      "followerId": 177,
      "followeeId": 33318,
      "status": "IS_FOLLOWING",
      "isFolloweeFavoriteOfFollower": false,
      "followerProfile": {
        "id": 13977,
        "publicId": "95e3569e-adca-4df3-84cf-0aae157b5b78",
        "firstName": "Tim",
        "lastName": "Cersky",
        "male": true,
        "imageSrc": "https://static-cdn.zwift.com/prod/profile/83ea831c-1750579",
        "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/83ea831c-1750579",
        "playerType": "NORMAL",
        "countryAlpha3": "esp",
        "countryCode": 724,
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
          "profileId": 177,
          "followersCount": 275,
          "followeesCount": 1167,
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
      },
      "followeeProfile": null
    }
}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [Rider Profiles](../README.md#rider-profiles) Rider Profile related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
