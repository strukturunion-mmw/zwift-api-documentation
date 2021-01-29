# Read rider profile

This allows an authenticated user to retrieve the public profile information of a specific rider

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `/api/profiles/{riderId}`

**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "riderId": "integer id of the rider for whom the profile is requested"
```

## Success Response

**Code** : `200 OK`

**response**
A json object containing the rider's public profile information

```json
{
    "id": 3649459,
    "publicId": "e9f441c0-7a08-4b0e-8fd1-2ca7d81d263c",
    "firstName": "Ronni",
    "lastName": "Rouleur",
    "male": true,
    "imageSrc": "https://static-cdn.zwift.com/prod/profile/de873b18-1901594",
    "imageSrcLarge": "https://static-cdn.zwift.com/prod/profile/de873b18-1901594",
    "playerType": "NORMAL",
    "countryAlpha3": "fra",
    "countryCode": 250,
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
      "defaultActivityPrivacy": "NOT_SET"
    },
    "socialFacts": {
      "profileId": 3649459,
      "followersCount": 1,
      "followeesCount": 0,
      "followeesInCommonWithLoggedInPlayer": 0,
      "followerStatusOfLoggedInPlayer": "SELF",
      "followeeStatusOfLoggedInPlayer": "SELF",
      "isFavoriteOfLoggedInPlayer": false
    },
    "worldId": null,
    "enrolledZwiftAcademy": false,
    "playerTypeId": 1,
    "playerSubTypeId": null,
    "currentActivityId": null,
    "address": null,
    "age": 22,
    "bodyType": 0,
    "connectedToStrava": false,
    "connectedToTrainingPeaks": false,
    "connectedToTodaysPlan": false,
    "connectedToUnderArmour": false,
    "connectedToWithings": false,
    "connectedToFitbit": false,
    "connectedToGarmin": false,
    "connectedToRuntastic": false,
    "connectedToZwiftPower": false,
    "stravaPremium": false,
    "bt": "01239198-899d-4f5b-9147-bb2217e26165",
    "dob": "1/27/1999",
    "emailAddress": "ronni.rouleur@peloton.fr",
    "height": 1850,
    "location": "",
    "preferredLanguage": null,
    "mixpanelDistinctId": "0a011a01-0694-4c1a-af16-1429af8000dd",
    "profileChanges": false,
    "weight": 79000,
    "b": false,
    "createdOn": "2021-01-27T14:40:14.319+0000",
    "source": "zwift-public",
    "origin": null,
    "launchedGameClient": null,
    "ftp": 0,
    "userAgent": null,
    "runTime1miInSeconds": 0,
    "runTime5kmInSeconds": 0,
    "runTime10kmInSeconds": 0,
    "runTimeHalfMarathonInSeconds": 0,
    "runTimeFullMarathonInSeconds": 0,
    "cyclingOrganization": null,
    "licenseNumber": null,
    "bigCommerceId": null,
    "publicAttributes": {},
    "privateAttributes": {},
    "achievementLevel": 100,
    "totalDistance": 0,
    "totalDistanceClimbed": 0,
    "totalTimeInMinutes": 0,
    "totalInKomJersey": 0,
    "totalInSprintersJersey": 0,
    "totalInOrangeJersey": 0,
    "totalWattHours": 0,
    "totalExperiencePoints": 0,
    "totalGold": 0,
    "runAchievementLevel": 100,
    "totalRunDistance": 0,
    "totalRunTimeInMinutes": 0,
    "totalRunExperiencePoints": 0,
    "totalRunCalories": 0,
    "powerSourceType": "Power Source",
    "powerSourceModel": "zPower",
    "virtualBikeModel": "---",
    "numberOfFolloweesInCommon": 0,
    "affiliate": "zwift_cycling_affiliate_ericschlange_apr19",
    "avantlinkId": null,
    "fundraiserId": null
  }
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [Rider Profiles](../README.md#rider-profiles) Rider Profile related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
