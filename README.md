# Language OCL [![Build Status](https://travis-ci.org/OpenFn/language-ocl.svg?branch=main)](https://travis-ci.org/OpenFn/language-ocl)

Language Pack for building expressions and operations for working with
the [OCL API](http://ocl.github.io/ocl-docs/master/en/developer/html/ocl_developer_manual.html).

## Documentation

View the [docs site](https://openfn.github.io/language-ocl/) for full
technical documentation. Below, find a samples of the most commonly used helper
functions.

## Sample State

```json
{
  "configuration": {
    "username": "#####",
    "password": "#####",
    "hostUrl": "https://api.openconceptlab.org/"
  },
  "data": {
    "a": 1,
    "b": 2
  }
}
```

## Mapping source concepts to destination API


#### Recieve form data from source application and convert data element keys to destination application.

```js
map(  "data": {
    "a": 1,
    "b": 2},
  {users:"haftamuk", sources: "eCHIS-CODES", concepts: "fp_new_at_10_to_14" }
  );
```



## Development

Clone the repo, run `npm install`.

Run tests using `npm run test` or `npm run test:watch`

Build the project using `make`.
