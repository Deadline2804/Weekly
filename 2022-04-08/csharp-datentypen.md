# C# Datentypen

| Datentypen |                                                                                   Wertebereiche |
| :--------- | ----------------------------------------------------------------------------------------------: |
| bool       |                                                                                      true/false |
| byte       |                                                                                       0 bis 255 |
| char       |                                                                  0 bis 65.535 (Unicode-Zeichen) |
| decimal    |                                                    -7,9x10<sup>28</sup> bis 7,9x10<sup>28</sup> |
| double     |                                                  -1,8*10<sup>308</sup> bis 1,8*10<sup>308</sup> |
| float      |                                                    -3,4x10<sup>38</sup> bis 3,4x10<sup>38</sup> |
| int        |                         -2.147.483.648 bis 2.147.483.647 (-2<sup>31</sup> bis 2<sup>31</sup>-1) |
| long       | -9.223.372.036.854.775.808 bis 9.223.372.036.854.775.807 (-2<sup>63</sup> bis 2<sup>63</sup>-1) |
| object     |                                                                                               / |
| sbyte      |                                                                                    -128 bis 127 |
| short      |                                                                              -32.768 bis 32.767 |
| string     |                                                                                               / |
| uint       |                                                          0 bis 4.294.967.295 (2<sup>32</sup>-1) |
| ulong      |                                             0 bis 18.446.744.073.709.551.615 (2<sup>64</sup>-1) |
| ushort     |                                                                                    0 bis 65.535 |

## Kategorien von Datentypen

- Werttypen (speichert Daten an sich)
- Nullable-Typen (Werttypen, die au??erdem 'null' sein k??nnen)
- Verweistypen/Referenztypen (speichert Referenz auf Daten)

## Heap und Stack

### Stack

- wird verwendet bei Werttypen (lokale Variablen; Funktionsparameter)
- Daten werden oben drauf gelegt; von oben nach unten entfernt -> LIFO (Last In, First Out)
- begrenzte Gr????e des Stacks f??r jeden Thread
- beim L??schen von Werttypen wird der Stack automatisch aufger??umt/Speicher freigemacht

### Heap

- wird verwednet bei Referenztypen
- aufgebaut wie ein Baumdiagramm
- langsamer als Stack, daf??r variabler in der Gr????e
- Speicher muss explizit wieder freigegeben werden (Garbage-Collection)
- globaler Zugriff
