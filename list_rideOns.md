# List RideOns

This allows an authenticated user to retrieve a list of all RideOns given to a specific rider for a specific activity.

## Endpoint request parameters

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `api/profiles/{riderId}/activities/{activityId}/rideon`

**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "riderId": "integer id of the rider receiving the RideOn"

  "activityId": "integer id of the activity for the RideOn given"
```

## Success Response

**Code** : `200 OK`

**response**
A json object containig all RideOns 

```json
{}
```

## See also

- [RideOns](https://github.com/strukturunion-mmw/zwift-api-documentation/blob/main/endpoints_rideOns.md) RideOn related endpoints

