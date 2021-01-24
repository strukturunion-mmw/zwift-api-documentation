# List RideOns

This allows an authenticated user to retrieve a list of all RideOns given to a specific rider for a specific activity.

## Endpoint request parameters

**URL** : `api/profiles/{riderId}/activities/{activityId}/rideon`

**Method** : `GET`

**Auth required** : True

**Required POST URL contained parameters**

```
  "riderId": "integer id of the rider receiving the RideOn"

  "activityId": "integer id of the activity for the RideOn given"
```

## Success Response

**Code** : `200 OK`

**response**
A Json object containig all RideOns 

```json
{}
```


