# flatiron-ceo-lab

"Cars for sale"

As a new car sales startup, we need to build out the first version of our platform. Our users need to be able to see a list of the cars available, and search by model name, type (pickup truck, sedan, etc...), or newness.

## deliverables

1. The app must display a scrollable list of cars.
2. Cars in list must be implemented re-usably, and simply.
<!-- 3. You must query a database for the list of cars. It doesn't need to be an active public API right now, just use seed data. -->
3. You must query the NHTSA vehicle query API for a list of models. To keep it simple, we don't care about model year. Also just query for Honda. See below.
<!-- 4. The user must be able to submit cars to the database through a controlled form. -->
5. The user must be able to search the list (responsively) with a controlled searchbox.

## NHTSA api

This url will return a JSON response with honda cars: `https://vpic.nhtsa.dot.gov/api/vehicles/getmodelsformake/honda?format=json`

Example code here: https://vpic.nhtsa.dot.gov/api/Home/Index/LanguageExamples

In theory we could do more with this path, but not important right now: https://vpic.nhtsa.dot.gov/api/vehicles/GetMakesForManufacturerAndYear/mer?year=2019&format=json

More info: https://vpic.nhtsa.dot.gov/api/


## Bonus

1. Ideally, the user can filter by model name, type, or newness, but it's not required for MVP.
2. Conditionally render an address form for the user to input their delivery address. It doesn't need to actually submit to a database yet.

## testing

No tests are required, but they'd be nice.
