# es6-namespace
[![Build Status](https://travis-ci.org/xuanhoa88/es6-namespace.svg?branch=master)](https://travis-ci.org/xuanhoa88/es6-namespace) [![npm version](https://badge.fury.io/xuanhoa88/es6-namespace.svg)](https://badge.fury.io/xuanhoa88/es6-namespace) [![Bower version](https://badge.fury.io/xuanhoa88/es6-namespace.svg)](http://badge.fury.io/xuanhoa88/es6-namespace) [![dependencies Status](https://david-dm.org/xuanhoa88/es6-namespace/status.svg)](https://david-dm.org/xuanhoa88/es6-namespace)

es6-namespace is a lightweight javascript helper checking for or creating namespace objects.
Is compatible with all new and old browsers like IE6.

## Usage

You can create a object chain with

```javascript
Namespace.create('be.awesome').Magic = function() {
  // your magic code
};
```

Check if a namespace exists

```javascript
Namespace.has('be.awesome');
```

Check if namespace on a local object exists

```javascript
var localObj = { be: { awesome: 'bam' } };
if (Namespace.has(localObj, 'be.awesome')) {
  Namespace.create('be.awesome');
}
```
