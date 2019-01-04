# Google Contacts Filter

Purpose: Creates a Gmail filter to exclude (whitelist) contacts from a Google contacts CSV file

Author: Matthew Renze

Usage: python.exe CreateFilter.py input-file
  - input-file - the Google Contacts CSV file to filter

Instructions:
1.  Go to https://www.google.com/contacts
2.  Select the contact to be included in the filter
3.  In the "More" dropdown list, select "Export"
4.  Select the Outlook CSV format *(NOT Google CSV format)*
5.  Click Export
6.  Run the script on the CSV file (as described above)
7.  Copy the output to your clipboard
8.  Go to https://mail.google.com/mail/u/1/#settings/filters
9.  Create a new filter
10. Paste the filter string into the "Doesn't have" field
11. Finish creating the filter

Now the selected email addresses will be excluded from the filter

Notes: 
 - Works only with Outlook CSV format export from Google Contacts. Unfortunately, the Google CSV format files had a weird encoding and couldn't be read as CSV
 - Google imposes a maximum size limit to the filter strings, so if you have too many contacts, this won't work. Try deselecting contacts until it does.
