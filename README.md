# tetriodata

This repository contains tar archives compressed with xz containing full tetraleague exports from https://tetr.io/about/api/#userlistsleagueall in csv format.


The fieldnames for the csv files are:
```
field_names = ["_id", "username", "role", "xp", "supporter", "verified", "country", "gamesplayed", "gameswon", "rating", "glicko", "rank", "bestrank", "apm", "pps", "vs", "timestamp", "rd"]
```
decaying is not included

The timestamp is created as follows:
```
timestamp = datetime.utcfromtimestamp(cached_at / 1000)
```
