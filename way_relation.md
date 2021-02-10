[MapRoulete Mosty w LDZ](https://maproulette.org/browse/challenges/16108)

[Budynki](https://budynki.openstreetmap.org.pl/#map=13/52.51863/19.76231)

### Przykład way/rel E 75 w Polsce ###
Wyszukiwanie przy pomocy overpass. Minimalna ilość danych (geom)
```
[out:json][timeout:25];
{{geocodeArea:Poland}}->.searchArea;
(
relation["name"="European route E 75 (Poland)"](area.searchArea);
);
out body;
>;
out skel qt;
```

[Link do kwarendy](https://overpass-turbo.eu/s/13tF)

### Przykład way/rel wszytkie dane dostępne dla E75###

```
[out:json][timeout:250];
{{geocodeArea:Poland}}->.searchArea;
(
relation["name"="European route E 75 (Poland)"](area.searchArea);
);
out meta;
>;
out meta qt;

{{style:
  relation {
    text: name;
  }
}}
```

[Link do kwarendy](https://overpass-turbo.eu/s/13tJ)

[Link do kwarendy - rodzaj powierzchni](https://overpass-turbo.eu/s/13tK)

### Analiza relacji w narzędziu ###

[Odcinek Łódzki](http://ra.osmsurround.org/analyzeRelation?relationId=2093779&_noCache=on)



[Osmose pl](http://osmose.openstreetmap.fr/pl/map/#zoom=8&lat=51.988&lon=19.846&item=xxxx&level=1&tags=&fixable=)

