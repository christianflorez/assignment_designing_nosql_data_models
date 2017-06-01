## User Log-In

You're building an application that requires user login. Once logged in the user has a bunch of profile information and preference settings available to them. They will need to be able set their birthday, gender, phone number and location (city, state, country). They should be able to provide text to tell about themselves. They also should be able to enable and disable visibility of their birthday, gender, phone number and location.

Index Table for Users

User Document:
* username: string
    * Must contain only word characters
* password: string
    * Must be at least 8 characters
* email: string
    * Must contain an @ symbol
* profile: subdocument

Profile Subdocument:
* birthday: date/time
    * Must be formatted as MM/DD/YYYY
* gender: string
    * Max of 10 characters
* phone number: integer
    * Must be formatted +1 (234) 567-8901
* location: subdocument
* visibleFields: Array containing key of visible fields (e.g. [["gender"], ["phonenumber"]], etc.)

Location Subdocument:
* city: string
    * Max of 20 characters
* state: string
    * selection from separate document
* country: string
    * selection from separate document

State Document:
* stateName: string
    * Max of 25 characters
* stateAbbr: string
    * Max of 2 characters

Country Document:
*  countryName: string
    * Max of 25 characters