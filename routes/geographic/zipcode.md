# Zipcode Recognizer

This route will match if and only if the user enters a valid 5 digit zipcode as their input.  If matching, a variety of values will be stored in the Conversation State as described in the table below.


| Conversation State Key                 | Description                                        |
|----------------------------------------|----------------------------------------------------|
| `routes.geo.last_zipcode`              | The valid 5 digit zipcode                          |
| `routes.geo.last_zipcode_type`         | STANDARD, PO BOX, MILITARY, or UNIQUE              |
| `routes.geo.last_city`                 | Primary city of the zipcode                        |
| `routes.geo.last_state`                | State of the zipcode                               |
| `routes.geo.last_latitude`             | Approximate centroid latitude (if available)       |
| `routes.geo.last_longitude`            | Approximate centroid longitude (if available)      |
| `routes.geo.last_country`              | Country, typically US but can be other values for territories and military zipcodes |
| `routes.geo.last_estimated_population` | Estimated population of the zipcode (if available) |
