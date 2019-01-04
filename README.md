Reformat.js
===========

Reformat.js is a small javascript library for format conversions.

## Community

### Adopters

Are you using reformat.js? Please consider opening a pull request to list your organization here:

* [MPI Bioinformatics Toolkit](https://toolkit.tuebingen.mpg.de/)
* [DNAVisualization.org](https://dnavisualization.org/)

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

__`alignment`:__ Validates if input is alignment
```javascript
$('#mySequences').reformat('alignment');
```

__`type`:__ validates type of input sequence, either DNA, RNA, Protein or undefined
```javascript
$('#mySequences').reformat('type');
```

__`detect`:__ Returns the format of an input as a string.

```javascript
var format = $('#mySequences').reformat('detect');
```

__`validate`:__ Validates an input format.

```javascript
$('#mySequences').validate('fasta'); // returns either true or false
```

__`alphabet`:__ Returns the alphabet of an input.

```javascript
$('#mySequences').reformat('alphabet'); // returns the characters which occur in a sequence or an alignment in alphabetical order
```

__`freq`:__ Returns the relative frequencies of amino acids compared to literature values.

```javascript
$('#mySequences').reformat('freq'); // returns the relative frequencies of amino acids compared to literature values
```

Attribution
-----------

Reformat.js was partially inspired by [Sebastian Wilzbach's clustal parser](https://github.com/biojs-io/biojs-io-clustal)
