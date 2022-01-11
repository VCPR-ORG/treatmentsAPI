## Style notes

id > ID
user (users) > User (see [proper nouns](proper-nouns))
  Ditto other active components e.g. Prescription??

Endpoint & Security Schema description as sentence (i.e. with stop, starts caps).
  Endpoint starts with "This endpoint ..."

Summary description as fragment (no caps/no stop)

Property description as fragment (no caps (unless [proper noun](proper-nouns))/ no stop)
  UNLESS LONG e.g., duration after last treatment during which some act is prohibited. Most often this restricts when meat or milk may be sold for food.

Error description as sentence: Success with caps as fragment (Success – token refreshed or OK)
rest as per style == no caps & fragment

## Proper nouns / Active components of system

User
Protocol
Diagnosis
Dosage
ID
Prescription
Greenbook Drug
Treatment
Eligibility / Eligibilities
Case
Promise


## Testing

[Mayhem](https://mayhem4api.forallsecure.com/docs/fuzz-your-own.html)

Warning -- construction is right BUT do not hit the production server with this!

mapi run  VCPR1 100 "https://raw.githubusercontent.com/VCPR-ORG/publicAPI/develop/src/openapi.yaml" --url "https://test.VCPR.ORG"   --interactive
