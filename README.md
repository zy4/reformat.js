Reformat.js
===========

Reformat.js is a small javascript library for format conversions.

Formats
-----

The converter covers the following formats:
__`fasta`__, __`clustal`__, __`phylip`__, __`stockholm`__, __`pir`__, __`embl`__, __`genbank`__, __`a3m`__, __`nexus`__

Usage
-----

You will need to include jQuery in order to use this library.


Methods
-------

e.g. __`fasta`:__ Returns the sequence as fasta.

```javascript
var fasta = $('#myClustal').reformat('fasta');
```

__`getGIs`:__ Returns GI numbers.

```javascript
var giArray = $('#mySequences').reformat('getgis');
```

__`consensus`:__ Returns the consensus sequence of an alignment as a string.

```javascript
var consensus = $('#myAlignment').reformat('consensus');
```


Attribution
-----------

Reformat.js was partially inspired by [Sebastian Wilzbach's clustal parser](https://github.com/biojs-io/biojs-io-clustal)
