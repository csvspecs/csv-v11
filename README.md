[CSV 1.1 @ GitHub](https://github.com/csvalues)


# CSV 1.1 - Comma Separated (Named) Values, Version: 1.1

_CSV Evolved (for Humans) - Easy-to-Write, Easy-to-Read_

```
#####################
# North America

# area (in sq km), pop(ulation)

ca, Canada,          CAN,   9 984 670 km²,  34 278 406
us, United States,   USA,   9 629 091 km², 314 167 157
mx, México [Mexico], MEX,   1 972 550 km², 112 322 757
...
```

(Source: [world.db/north-america/countries.txt](https://github.com/openmundi/world.db/blob/master/north-america/countries.txt))


```
###########################
# Oh, Canada! 10 provinces and 3 territories
#
# see en.wikipedia.org/wiki/Provinces_and_territories_of_Canada
#
# note: key is two-letter canadian postal code
#
# for regions tags see
#   en.wikipedia.org/wiki/List_of_regions_of_Canada


bc, British Columbia,       Victoria,     922 509 km², en|western canada

ab, Alberta,                Edmonton,       640 082 km², en|western canada|prairies
mb, Manitoba,               Winnipeg,       552 330 km², en|western canada|prairies
sk, Saskatchewan,           Regina,         588 239 km², en|western canada|prairies

nb, New Brunswick,            Fredericton,    71 377 km², en|fr|eastern canada|atlantic canada|maritimes
ns, Nova Scotia,              Halifax,        52 939 km², en|eastern canada|atlantic canada|maritimes
pe, Prince Edward Island,     Charlottetown,   5 686 km², en|eastern canada|atlantic canada|maritimes
nl, Newfoundland and Labrador,  St. John's,   370 511 km², en|eastern canada|atlantic canada
...
```

(Source: [world.db/master/north-america/ca-canada/regions.txt](https://github.com/openmundi/world.db/blob/master/north-america/ca-canada/regions.txt))



## Design Principles

- Evolving and working with real-world datasets and code ;-). "Eat your own dog food".
- The long long view. 10 years. 20 years. 30 years. 100 years. Text is forever ;-)

**Less (typing) is better. Easy-to-write.**

- No quotes needed for values, that is, write `Halifax` and not `"Halifax"`. Requiring quotes (`"..."` or `'...'`) is a no-no.   


**Easy-to-read.** 

- Comments, comments, comments.
- Use space to format your datasets, that is, `bc, British Columbia,    Victoria` is the same as `bc,British Columbia,Victoria`.
- Blank lines.

**Human. Practical (proven) alternatives.**

- Use dual quotes e.g. `"..."` or `'...'`.
- Use here documents e.g. `<<TXT ... TXT` for multi-line values.
- Use triple quotes e.g. `"""..."""` or `'''...'''` for multi-line values or mixed quote escaping.

**Human. Options. Options. Options.**

- No fixed number of fields.
- Use single-line or multi-line records.
- Use "classic" values "by position" or named values (e.g. `city: Halifax`).

**Conventions. Let the computer help you (auto-)fill-in values.**

- Auto-generate record ids from names / titles.
- Optional "front matter" block with defaults / fallbacks (e.g. `country: Canada`).




## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The CSV 1.1 format and conventions are dedicated to the public domain.
Use it as you please with no restrictions whatsoever.

## Questions? Comments?

Send them along to the [wwwmake mailing list/forum](http://groups.google.com/group/wwwmake). Thanks
