## Moot language files

Moot's default language is English. The English localization consists of two files:

1. en.js: the client's text content in English ('All posts', 'Online', 'Reply...' etc.)
2. en.auth.js: the authentication windows' text content in English ('log in', 'join', 'forgot password'...)

To create a new localization you need to:

1. Fork this repository
2. Copy the English localization files and rename them with the target language code: For example ru.js and ru.auth.js.
3. Open the copied files on your text editor and replace the English words with the new language
4. Send us a pull request

## Fork from moot/language

This is a fork from moot/language. Only the French translation is updated.

### Testing

You can test your new localization by opening the [test.html](test.html) file on your browser and supplying the language code on the query string. For example:

`test.html?ru`

The client should now use your language. The authentication file (such as ru.auth.js) and the login dialog will not work until your work is submitted to us and the files are made available in our content delivery network.

*Note* If you see badly rendered characters then the language file is not encoded in UTF-8 format. These commands fixes the issue in OSX:

``` sh
iconv -f ISO-8859-1 -t utf-8 ru.js > ru8.js && mv ru8.js ru.js
iconv -f ISO-8859-1 -t utf-8 ru.auth.js > ru.auth8.js && mv ru.auth8.js ru.auth.js
```

### Style guide

A few things to keep in mind:

1. Keep sentences short! The shorter and more precise the better.
2. Find the best way to say it in *your* language. Don't just directly translate the English words. (Google Translate is not recommended here.)
3. Moot is constantly updating and improving, and new content will be added. We hope you can contribute later too.

Thanks! We appreciate the help.
