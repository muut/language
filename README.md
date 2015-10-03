


## Muut language files

Muut's default language is English. The English localization consists of two files:

1. en.js: the client's text content in English ('All posts', 'Online', 'Reply...' etc.)
2. en.auth.js: the authentication windows' text content in English ('log in', 'join', 'forgot password'...)

To create a new localization you need to:

1. Fork this repository
2. Copy the English localization files and rename them with the target language code: For example ru.js and ru.auth.js.
3. Open the copied files on your text editor and replace the English words with the new language
4. Send us a pull request

### Wait, forking, pull request!?!

If forking makes no sense you can just save these files

https://raw.github.com/moot/language/master/en.js

https://raw.github.com/moot/language/master/en.auth.js

on your PC and then proceed with steps 2 and 3 above. Then send the modified files to tero@muut.comm


### Updates

Muut is constantly updating and improving. Your language files will contain English placeholders on top of the files once new content is added. See for example [es.js](es.js#L7). Please update the new language by making a pull request or send the updates directly to tero@muut.com . Thank you!


### Testing

You can test your new localization by opening the [test.html](test.html) file on your browser and supplying the language code on the query string. For example:

`test.html?ru`

The client should now use your language. Note that you should serve the test.html file from a local webserver (localhost) and not directly from the file system (file:// protocol). This way the avatars are displayed correctly and you can debug the language of the authentication pieces too.


*Note* If you see badly rendered characters then the language file is not encoded in UTF-8 format. These commands fixes the issue in OSX:

``` sh
iconv -f ISO-8859-1 -t utf-8 ru.js > ru8.js && mv ru8.js ru.js
iconv -f ISO-8859-1 -t utf-8 ru.auth.js > ru.auth8.js && mv ru.auth8.js ru.auth.js
```

### Style guide

A few things to keep in mind:

1. Keep sentences short! The shorter and more precise the better.
2. Find the best way to say it in *your* language. Don't just directly translate the English words.
3. [Google Translate](http://translate.google.com/) works well for individual words but you know the precise sentences better.

Thanks! We appreciate the help.
