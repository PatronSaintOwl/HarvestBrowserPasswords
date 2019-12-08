# HarvestBrowserPasswords
A Windows tool for extracting credentials locally stored by Google Chrome and Mozilla Firefox web browsers

Decrypts Google Chrome passwords for the currently logged-on user by locating "Login Data" database files and using DPAPI to decrypt passwords

Decrypts Mozilla Firefox passwords for all available profiles by locating 'key4.db' databases and 'logins.json' files for 3DES decryption. Supports decryption using a master password using the `-p` option if master password is known.

## Usage
`HarvestBrowserPasswords.exe <options>`

## Command Line Options
  -c, --chrome      Locate and decrypt Google Chrome logins

  -f, --firefox     Locate and decrypt Mozilla Firefox logins

  -a, --all         Locate and decrypt Google Chrome and Mozilla Firefox logins

  -p, --password    (Optional) Master password for Mozilla Firefox Logins

  -o, --outfile     Write output to csv

  --help            Display help message
