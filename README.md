## Good Tenants Country Library

A simple npm package to fetch location data based on the country using the useGoodTenantsCountryLibrary function.

## Installation

npm install good-tenants-country-library

## Usage

import useGoodTenantsCountryLibrary from "good-tenants-country-library";

// Example 1
const goodTenantsCountryLibrary = useGoodTenantsCountryLibrary();

//get states
const states = goodTenantsCountryLibrary.getStates(country)
console.log(states);

//get areas
const area = goodTenantsCountryLibrary.getAreasByState(state, country)
console.log(area);

//get sub areas
const subArea = goodTenantsCountryLibrary.getSubareasByArea(area, state, country)
console.log(subArea);

## Parameters
All parameters are required for all functions
-  getStates: (country: required): A string representing the country for which you want to fetch location data. Only 'nigeria', 'kenya', and 'uganda' are supported.
-  getAreasByState: (state: required, country: required): A string representing the state selected from the list of supported states, and a string representing the country for which you want to fetch location data.
-  getSubareasByAre: (area: required, state: required, country: required): A string representing the area selected from the supported list of areas, a string representing the state selected from the list of supported states and a string representing the country for which you want to fetch location data.

## Data Structure

The returned data is an array containing the subarea || area || state depending on the function used.


## License

This project is licensed under the MIT License - see the LICENSE file for details.