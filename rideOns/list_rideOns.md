# List RideOns

This allows an authenticated user to retrieve a list of all RideOns given to a specific rider for a specific activity.

## Endpoint request parameters

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `api/profiles/{riderId}/activities/{activityId}/rideon/?created_before={created_before}&start={start}&limit={limit}`

**Method** : `GET`

**Auth required** : True

**Required GET URL contained parameters**

```
  "riderId": "integer id of the rider receiving the RideOn"

  "activityId": "integer id of the activity for the RideOn given"
```

**Optional GET URL contained parameters**

```
  "created_before": "timestamp up until rideOns were given" / default: now

  "start": "Number of records to skip before starting output / default: 0
  
  "limit": "Number of records to return" / default (max): 20
```

## Success Response

**Code** : `200 OK`

**response**
A json object containing all RideOns 

```json
{}
```

## See also

- [ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de) Test the API with instant feedback

- [RideOns](../README.md#rideons) RideOn related endpoints

- [Endpoints overview](../README.md#known-endpoints) Overview of all documented API endpoints
