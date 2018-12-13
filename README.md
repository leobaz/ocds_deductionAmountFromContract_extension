# Deduction amount from the contract

The deduction amount from the contract extension is used to express the amount deducted from the contract due to causes of prohibitions. 

There are a lot of factors that cause the prohibitions.

For example, if we are building a road from point A to point B and in the middle of that road, it's a building that prevents the road. Now in the contract, it is planned to destroy that building and if for any circumstance a new decision comes to not destroy the building but to go around it the amount from not destroying the building is the amount of deduction from the contract due to the causes of the prohibitions.

## Additional fields

The field introduced by this extension is:

* ``` contracts/deductionAmountFromContract ``` - The amount deducted from the contract

## Example

Simple example: 

```
{
    "ocid": "ocds-213czf-000-00001",
    "id": "ocds-213czf-000-00001-07-close",
    "date": "2012-01-10T09:30:00Z",
    "initiationType": "tender",
    "tag": [
      "contract"
    ],
    "parties": ["..."],
    "buyer": {
      "id": "EU-LAC-E09000003"
    },
    "awards": ["..."],
    "contracts": [
      {
        "id": "ocds-213czf-000-00001-contract-01",
        "awardID": "ocds-213czf-000-00001-award-01",
        "title": "Contract to build new cycle lanes in the centre of town.",
        "period": {
          "startDate": "2010-07-01T00:00:00Z",
          "endDate": "2012-01-01T23:59:00Z",
          "maxExtentDate": "2012-01-31T23:59:00Z"
        },
        "value": {
          "amount": 11500000,
          "currency": "EUR"
        },
        "deductionAmountFromContract": {
          "value": {
            "amount": 1455,
            "currency": "EUR"
          }
        }
      }
    ]
}
```