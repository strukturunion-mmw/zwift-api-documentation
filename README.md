![cover image](/coverimage.jpg)

This UNOFFICIAL documentation of the ZWIFT mobile API is the result of what we have collected from existing projects and 
from our own observations, watching the ZWIFT website and companion app *in action*. It likely is by no means complete 
nor adorsed or supported by ZWIFT. No guarantees for any functionality are given as ZWIFT may change it's API at any 
time without notice.  

Note that this is not a "ready-to-use" code in a specific language, but it is a mere helper, allowing to easier implement 
API calls to ZWIFT in your own application. It is meant to serve as a reference for general working concepts as well as 
for lookup of parameters, call specifics etc. 

Please SHARE your insights on the API with us, so the documentation can be completed over time.  

Special thanks go out to the following projects for the groundwork laid:  
- [Ogadai/zwift-mobile-api](https://github.com/Ogadai/zwift-mobile-api)
- [darenc/zwift-php](https://github.com/darenc/zwift-php)
- [jeroni7100/zh-zml](https://github.com/jeroni7100/zh-zml)
- [zwift-client](https://pypi.org/project/zwift-client/)

Ride on!

# Instant Testing
To test API calls with instant feedback and for quick troubleshooting you may want to check out the <br>
[ZWIFT API Test WebApp](https://zwiftapi.strukturunion.de), which allows you to use your own credentials for live 
feedback from ZWIFT.


# Known endpoints

## Rider Profiles
- [Retrieve own rider profile](/riderProfiles/read_my_profile.md) Retrieve own rider profile of authenticated user
- [Retrieve any rider profile](/riderProfiles/read_rider_profile.md) Retrieve profile of a specific rider
- [List any rider's followers](/riderProfiles/list_followers.md) List all riders that follow a specific rider
- [List any rider's followees](/riderProfiles/list_followees.md) List all riders being followed by a specific rider
- *currently working on commpleting this part of the documentation*

## RideOns
- [Give RideOn](/rideOns/give_rideOn.md) Give RideOn to another rider's activity (current or past)
- [Read RideOns](/rideOns/read_rideOns.md) Read RideOn Information of a specific RideOn
- [List RideOns](/rideOns/list_rideOns.md) List all RideOns for a rider on an activity

## Activities
- *planned to work on this part of the documentation*

## Worlds
- [Show Watopia Stats](/worlds/show_watopia_stats.md) Show current stats on Watopia public world
- [List all Riders in Watopia](/worlds/show_riders_in_watopia.md) Show all current riders in Watopia public world 
- *currently working on commpleting this part of the documentation*
