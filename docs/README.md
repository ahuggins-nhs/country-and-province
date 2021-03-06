country-and-province / [Exports](modules.md)

# Province and Country

A library for ISO Country and Province data, wrapping two npm modules in an easy-to-use API.

This library currently uses `country-list` and `provinces` libraries as the data back-end. The main motivation for this library was to build out useful searching and resolving of country and province names and codes with an easy-to-understand API.

## Usage

Install from NPM and import it.

```javascript
const { Countries, Provinces, Country, Province } = require('./index.js')

console.log(Countries.byName('United States')) // Expected output: Country class with data for United States of America
console.log(new Country('CA')) // Expected output: Country class with data for Canada

console.log(Provinces.byCode('QC')) // Province class for Quebec, Canada
console.log(new Province('CA')) // Province class for California, United States
console.log(new Province('Newfoundland')) // Province class for Newfoundland, Canada

console.log(new Country('Spain').provinceByCode('CA')) // Province class for Cádiz, Spain

```

## API

Self-documented within [this repository](./docs/modules.md).
