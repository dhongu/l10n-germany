Loads the German localities (Orte) with their postal code and region, and fills in the
city and the region of German addresses from the postal code.

- Ships the list of German localities with their postal code, linked to the regions of Germany. The data
  comes from [GeoNames](https://www.geonames.org) (Creative Commons Attribution 4.0).
- Germany is set to *enforce cities*: the city of a German address is chosen from the list.
- On the contact form, typing the postal code (Postleitzahl) of a German address sets the city and the
  region. A postal code shared by several localities sets only the region; the city name, when it matches
  one of them (without accents and case), picks the locality.
- The action *Germany: set city from ZIP* on contacts links the German contacts to the city of their postal
  code and fills in the region.
- At install, the German contacts are linked: directly on a small database, by the scheduled action
  *Germany: link contacts to the city of their ZIP* in batches on a large one (it deactivates itself when done).
- Every form that runs the postal code rules of the contact (for example the delivery details of an AWB)
  gets the region filled in, so the shipment can be sent to Germany without looking it up by hand.
