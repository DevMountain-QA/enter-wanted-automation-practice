<img src="https://devmounta.in/img/logowhiteblue.png" width="250" align="right">

# AJ's Enter Wanted Test

This project is to create a web form that will generate the text to submit to the NCIC to add a warrant.

It is assumed that if incorrect entry occurs, the proper error message will be displayed to assist the user in correcting their mistakes.

Development on the application has been focused only on completing the form and validations, stylistic concerns are not being addressed at this time.

### The requirements are as follows for each field, and the results:

alpha: any alphabetical characters, upper or lower case

numeric: numbers only, 0-9

special: these are any characters other than numbers and letters, including blank spaces ' ' - Periods '.' should not be allowed, as it will break message parsing.

* Header: Required, 9-19 characters in length, any allowed
* MKE: Required, 2-4 in length, alphabetical or special characters allowed
* Originating Agency Identifier: Required, 9 alphanumeric characters in length
* Name: Required, 1-30 characters in length, any allowed
* Sex: Required, 1 character in length, alphabet only, F (female) M (male) and U (unknown) are the only accepted entries
* Race: Required, 1 character in length, alphabet only
* Height: Required, 3 characters in length, numeric only in FII format, where F is feet and I is inches
* Weight: Required, 1-3 characters in length, numeric only in lbs, leading zeros to be entered systematically as necessary to change the length to 3 characters in the assembled query.
* Hair: Required, 3-10 characters in length, alphabetical only
* Offense: Required, 5-15 characters in length, any allowed
* Date of Warrant/Violation: Required, 8 characters in length, numeric in MMDDYYYY format (allows dates from 1900 to today +1 day, to account for time zone differences)
* Drivers License: Optional, 1-20 characters in length, any characters allowed, if included requires DL State & DL Expiration Year
* DL State: Optional, 2 characters in length, State Abbreviations only, if included requires Drivers License & DL Expiration Year
* DL Expiration Date: Required, 8 characters in length, numeric in MMDDYYYY format (allows dates from 1900 to today +1 day, to account for time zone differences)
* License Plate: Optional, 5-8 alphanumeric characters in length, if included requires License State & License Year
* License State: Optional, 2 characters in length, State Abbreviations only, if included requires License Plate and License Year
* License Year: Optional, 4 characters in length, numeric in YYYY format, if included requires License Plate and License Year

Upon successful entry, a text message will be created, which consists of each of the values entered, separated by a '.' - any optional fields left blank will still be denoted in the message by an additional '.'

* Submit Button - This will validate entries and generate either a textual message or error messages as appropriate.
* Undo Button - This will reset inputs to either blank, or to the last submitted values.

## Change Report
* Names Updated to accept as little as one character
* MKE fixed to match reqs.
* OAI fixed to match reqs.
* Updated reqs with submit and undo buttons.
* Docs updated:
  * Height and Weight field explanations updated
  * DL Expiration Year replaced by Expiration Date per customer request previously.
  * License plate requirements added (including License State and License Year)
  * Submit and Undo button descriptions added

## Planned Updates
* Race, Sex, and Offense input fields to be replaced by drop-down menus for ease of use; will still allow free-form entry for more unanticipated local requirements.
* Future Dates: Date of Warrant/Violation and Expirations are currently handled incorrectly for valid future dates.  This is a known issue and is being worked.
* Height: To be split into two fields - one for feet, one for inches.

## Project Instructions
Assume that it has been a few weeks since the bugs we found yesterday were reported.  Those have been reported as fixed, as well as several other issues uncovered by your development team through the process of debugging, corresponding updates have been made to the documentation.

* Note: Since changes were made to the docs, you may need to update or create one or more tests.

## Contributions

If you see a problem or a typo, please fork, make the necessary changes, and create a pull request so we can review your changes and merge them into the master repo and branch.

## Copyright

© DevMountain LLC, 2018. Unauthorized use and/or duplication of this material without express and written permission from DevMountain, LLC is strictly prohibited. Excerpts and links may be used, provided that full and clear credit is given to DevMountain with appropriate and specific direction to the original content.

<p align="center">
<img src="https://devmounta.in/img/logowhiteblue.png" width="250">
</p>