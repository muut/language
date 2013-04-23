
## Moot language files

Moot's default language is English and it consists of two files

1. *en.js*: the main language on the client
2. *en.auth.js*: the language on the authentication windows (log in, join, forgot password etc..)

To make a new language you need to:

1. Fork this repository
2. Copy the English files and rename them with the target language code: For example *ru.js* and *ru.auth.js*.
3. Open the copied files on your text editor and overwrite the English words with your own language
4. Send us a pull request

### Wait, forking, pull request!?!

If forking sounds weird you can just save these files

https://raw.github.com/moot/language/master/en.js
https://raw.github.com/moot/language/master/en.auth.js

on your PC and do steps 2 and 3 above. Then send the modified files to tero@moot.it


### Testing

You can test your language by opening the [index.html](index.html) file on your browser. You can supply your language on the browsers location bar by providing the language code on the query string. For example:

`index.html?ru`

The authentication file such as *ru.auth.js* and the login dialo will not work until your work is submitted to us and the file is made available to our content delivery network.


### Style guide

Two things to keep in mind

1. Keep sentences short! The shorter and more precise the better.
2. Find the best way to say it in *your* language. Don't just blindly translate the English words.
3. Moot is constantly updating and improving. We hope you can contribute later too.



