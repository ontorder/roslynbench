shitty not-that-much realistic compiling speed test  
if i ever get time and force of will i could think of making something more useful

```
.net 10.0.2 release  
-------------------------  
test            time            out size        src size        description
100kclassdeco   95.2 sec        10.104 KB       22.3 MB         class name{[attrib]ctor [attrib]tostring}
100kclass       23.3 sec        5.404 KB        2.3 MB          class name;
100kclass       6.3 sec         5.404 KB        2.3 MB          🤷🏻
100krec         146.5 sec       84.755 KB       2.4 MB          record name;
100ksrec        145.0 sec       84.755 KB       3.1 MB          sealed record name;
1megarec        too long        31.0 MB                         sealed record name;
100kif          16.0 sec        1.403 KB        5.18 MB         if (n == ###) return true;
100kclaff       45.1 sec        5.293 KB        100K files      file: class name;
100klambda      88.4 sec        16.759 KB       6.48 MB         M(v[]) => v.Any(_=>_==###);
100kslambda     89.1 sec        16.759 KB       7.18 MB         M(v[]) => v.Any(static _=>_==###);
100kxmldoc      26.3 sec        4.192 KB        20.47 MB        /// <summary> <param> <return>
100kclassmin    47.1 sec        10.104 KB       16.1 MB         classdeco, no spaces \n \r
50Kclass        6.0 sec         2.604 KB        1.15 MB         class name;
200kclass       11.9 sec        10.904 KB       4.7 MB          class name;
```
