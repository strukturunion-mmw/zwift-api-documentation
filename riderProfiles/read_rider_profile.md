# Read rider profile

This allows an authenticated user to retrieve the public profile information of a specific rider

**Base URL** : 'https://us-or-rly101.zwift.com'

**Endpoint** : `api/profiles/{riderId}`

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
{}
```

## See also

- [Rider Profiles](https://github.com/strukturunion-mmw/zwift-api-documentation/blob/main/riderProfiles/endpoints_riderProfiles.md#rider-profiles) Rider Profile related endpoints

- [Endpoints overview](https://github.com/strukturunion-mmw/zwift-api-documentation/blob/main/README.md#known-endpoints) Overview of all documented API endpoints
