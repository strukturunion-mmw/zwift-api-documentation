Used to collect a Token for a registered User.

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
