### Przykład pierwszy E 75 w Polsce ###
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

### Przykład drugi wszytkie dane dostępne dla E75###

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
