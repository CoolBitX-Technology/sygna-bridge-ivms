## Business example 1
```
{
  "ivms": {
    "originator": {
      "person_type": "NaturalPerson",
      "name_identifier": {
        "primary_identifier": "Smith",
        "secondary_identifier": "Dr Alice",
        "identifier_type": "LEGL"
      },
      "date_and_place_of_birth": {
        "date_of_birth": "1990-11-19",
        "place_of_birth": "US"
      },
      "account_number": "1BvBMSEYstWetqTFn5Au4m4GFg7xJaNVN2"
    },
    "beneficiary": [
      {
        "person_type": "NaturalPerson",
        "name_identifier": {
          "primary_identifier": "Barnes",
          "secondary_identifier": "Robert",
          "identifier_type": "LEGL"
        },
        "date_and_place_of_birth": {
          "date_of_birth": "1990-11-19",
          "place_of_birth": "TZ"
        },
        "account_number": "1BVMFfPXJy2TY1x6wm8gow3N5Amw4Etm5h"
      }
    ],
    "originator_vasp": {
      "person_type": "LegalPerson",
      "name_identifier": {
        "legal_name": "VASP A",
        "name_type_code": "LEGL"
      },
      "national_identification": {
        "nation_identifier": "3M5E1GQKGL17HI8CPN20",
        "identifier_type": "LEIX"
      }
    },
    "payload_metadata": {
      "transliteration_method": "armn"
    }
  }
}
```
* **transliterationMethod:** The method used to map from a national system of writing to Latin script.

## Business example 2
```
{
  "ivms": {
    "originator": {
      "person_type": "NaturalPerson",
      "name_identifier": {
        "primary_identifier": "Wu",
        "secondary_identifier": "Xinli",
        "identifier_type": "LEGL"
      },
      "local_name_identifier": {
        "primary_identifier": "吳",
        "secondary_identifier": "信利",
        "identifier_type": "LEGL"
      },
      "national_identification": {
        "nation_identifier": "446005",
        "identifier_type": "RAID",
        "registration_authority": "RA000553"
      },
      "country_of_residence": "TZ",
      "account_number": ""
    },
    "beneficiary": [
      {
        "person_type": "LegalPerson",
        "name_identifier": {
          "legal_name": "ABC Limited",
          "name_type_code": "LEGL"
        }
      },
      {
        "person_type": "LegalPerson",
        "name_identifier": {
          "legal_name": "CBA Trading",
          "name_type_code": "TRAD"
        }
      }
    ],
    "payload_metadata": {
      "transliteration_method": "hani"
    },
    "transfer_path": {
      "person_type": "LegalPerson",
      "name_identifier": {
        "legal_name": "VASP E",
        "name_type_code": "LEGL"
      },
      "sequence": 0
    }
  }
}
```
* **sequence:** The sequence in a serial chain at which the corresponding intermediary VASP participates in the transfer.
