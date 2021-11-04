

# API details

The below GET request API can be used to check whether an entity is in the sanctions list or not

    https://api.finhunt.org/sanction_lookup?q=

 
# Steps to look up an entity using the Free Sanctions Lookup API

To look up any entity, Provide a query string (q) with details about the entity . Each string should be separated by a space.

You may test the below queries by copying and pasting the sample links given below to a new browser window

For eg :

To look up if a person with the passport no “AB269600” is available in the sanctions list, use the below query

    https://api.finhunt.org/sanction_lookup?q=AB269600

To look up if a person named “Alex” with passport no “AB269600” is available in the sanctions list, use the below query

    https://api.finhunt.org/sanction_lookup?q=Alex AB269600

To look up if a person named “Alex” with passport no “AB269600” from “Belarus” is available in the sanctions list, use the below query

    https://api.finhunt.org/sanction_lookup?q=Alex AB269600 Belarus 


# The response to the request would look as below

[
  {
    "first_name": "Alex Nain",
    "last_name": "SAAB MORAN",
    "document": [
      {
        "type": "Cedula No.",
        "number": "72180017",
        "issuing_country": "Colombia"
      },
      {
        "type": "Passport",
        "number": "PE085897",
        "issuing_country": "Colombia"
      },
      {
        "type": "Passport",
        "number": "085635076",
        "issuing_country": "Venezuela"
      },
      {
        "type": "Passport",
        "number": "D010302",
        "issuing_country": "Antigua and Barbuda"
      },
      {
        "type": "Gender",
        "number": "Male"
      }
    ],
    "alias": [
      {
        "name": "Alex SAAB"
      },
      {
        "name": "Alex SAAB MORAN"
      }
    ],
    "sanction_list_name": "US OFAC CDN",
    "original_data": "uid:\n  _text: \"26995\"\nfirstName:\n  _text: \"Alex Nain\"\nlastName:\n  _text: \"SAAB MORAN\"\nsdnType:\n  _text: \"Individual\"\nprogramList:\n  program:\n    _text: \"VENEZUELA-EO13850\"\nidList:\n  id:\n    - uid:\n        _text: \"17691\"\n      idType:\n        _text: \"Cedula No.\"\n      idNumber:\n        _text: \"72180017\"\n      idCountry:\n        _text: \"Colombia\"\n    - uid:\n        _text: \"17692\"\n      idType:\n        _text: \"Passport\"\n      idNumber:\n        _text: \"PE085897\"\n      idCountry:\n        _text: \"Colombia\"\n    - uid:\n        _text: \"17693\"\n      idType:\n        _text: \"Passport\"\n      idNumber:\n        _text: \"085635076\"\n      idCountry:\n        _text: \"Venezuela\"\n    - uid:\n        _text: \"17694\"\n      idType:\n        _text: \"Passport\"\n      idNumber:\n        _text: \"D010302\"\n      idCountry:\n        _text: \"Antigua and Barbuda\"\n    - uid:\n        _text: \"132029\"\n      idType:\n        _text: \"Gender\"\n      idNumber:\n        _text: \"Male\"\nakaList:\n  aka:\n    - uid:\n        _text: \"42861\"\n      type:\n        _text: \"a.k.a.\"\n      category:\n        _text: \"strong\"\n      lastName:\n        _text: \"SAAB\"\n      firstName:\n        _text: \"Alex\"\n    - uid:\n        _text: \"42862\"\n      type:\n        _text: \"a.k.a.\"\n      category:\n        _text: \"strong\"\n      lastName:\n        _text: \"SAAB MORAN\"\n      firstName:\n        _text: \"Alex\"\ndateOfBirthList:\n  dateOfBirthItem:\n    uid:\n      _text: \"31881\"\n    dateOfBirth:\n      _text: \"21 Dec 1971\"\n    mainEntry:\n      _text: \"true\"\n",
    "score": 12.228511810302734
  }]



# Limits

The public API given above has a per IP limit of 100 API calls per day for security reasons .

To get access to the free API key ( which allows you to make 20,000 free sanctions lookup per month  ), Please reach out to us via email at solutions@finhunt.org
