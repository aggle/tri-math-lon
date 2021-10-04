# tri-math-lon
Exploring triathlon results data

## Usage
Results typically have the following columns: place, bib #, name, gender, swim time, t1, bike time, t2, run time, overall time, and overall place. They may also have additional columns like city,	state, country, paces for swim, bike and run, places for swim, bike and run, age, division, and division place. 

Each output format will need a different parsing utility to clean the data for ingestion into the main processing pipeline. Values that can be derived will be re-derived instead of read, so for each race you will need to provide the distances for each leg. If distances are not provided, then I guess fields that depend on distance will be set to NaN.
