# Css3.DB

A simple database that uses css as the storage format.

## Installation

```bash
npm install css3.db
```

## Usage

```javascript
const CSS3DB = require('css3.db');

// Create a new html database
const cssDB = new CSS3DB(__dirname+'/db1.css');

// Set key/value pair
cssDB.set('foo', 'boo') // -> true

// Get length (or size)
cssDB.length // -> 1
cssDB.size // -> 1

// Get key
cssDB.get('foo') // -> 'boo'

// Has key
cssDB.has('foo') // -> true

// Delete key
cssDB.delete('foo') // -> true

// Get entries
cssDB.entries() // -> [{"key": "foo", "value": "boo"}]

// Get keys
cssDB.keys() // -> ["foo"]

// Get values
cssDB.values() // -> ["boo"]

// Clear all entries
cssDB.clear() // -> true
```
