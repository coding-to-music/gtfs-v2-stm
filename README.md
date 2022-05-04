# gtfs-v2-stm

## calls STM GTFS API only no UI, produces JSON file

# 🚀 Javascript full-stack 🚀

https://github.com/coding-to-music/gtfs-v2-stm

https://gtfs-v2-stm.vercel.app -- calls STM GTFS API only no UI

by ansel brandt https://github.com/anselbrandt

https://github.com/anselbrandt/gtfs-v2-stm

## Environment Values

```java
STMKEY=""
```

# GTFS Realtime V2 Feed from Montreal STM

This example code fetches the realtime GTFS feed from the Société de transport de Montréal (STM) [GTFS-REALTIME V2 API](https://developpeurs.stm.info/documentation/gtfsrtv2).

An API key is required from the [STM Developer Portal](https://developpeurs.stm.info)

#### Install

```
yarn
```

#### Run

```
yarn start
```

Vehicle information will be in the form:

```
{
  id: '29060',
  vehicle: {
    trip: {
      tripId: '239563421',
      startTime: '19:18:00',
      startDate: '20211111',
      routeId: '179'
    },
    position: {
      latitude: 45.53441619873047,
      longitude: -73.66036224365234,
      bearing: 292,
      speed: 3.055579900741577
    },
    currentStopSequence: 21,
    currentStatus: 'IN_TRANSIT_TO',
    timestamp: '1636677622',
    congestionLevel: 'CONGESTION',
    vehicle: { id: '29060' },
    occupancyStatus: 'STANDING_ROOM_ONLY'
  }
}
```

\*`congestionLevel` property is not on all vehicles.

#### GTFS Realtime Overview

[Google Transit APIs -> Realtime Transit](https://developers.google.com/transit/gtfs-realtime)

#### GTFS V2 Data Structure and Type Definitions

[https://github.com/google/transit/blob/master/gtfs-realtime/proto/gtfs-realtime.proto](https://github.com/google/transit/blob/master/gtfs-realtime/proto/gtfs-realtime.proto)

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/gtfs-v2-stm.git
git push -u origin main
```

## Heroku

```java
heroku create gtfs-v2-stm


 ›   Warning: heroku update available from 7.60.1 to 7.60.2.
Creating ⬢ gtfs-v2-stm... !
 ▸    You've reached your app limit of 100 apps. Delete some apps or open a ticket at
 ▸    https://help.heroku.com/new/increase-limits to have this limit increased.
```

## Heroku MongoDB Environment Variables

```java
heroku config:set

heroku config:set MONGODB_URI="your value"
```

## Push to Heroku

```java
git push heroku

# or

npm run deploy
```
