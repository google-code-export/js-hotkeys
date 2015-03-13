Anonymous at 09 Dec, 2007 11:49
Hello. First of all, please, sorry my poor english.

I have certain little problem with shorcut.js in the case of assign "t" key and not F5 key. In this case, when you press the F5 key shorcut.js trigger the event assigned to the "t" key.

The same issue with the "s" and F keys, and for the "u" and F6 keys. You can obtain information about this issue in this link of the jQuery hotkeys plugin page.

I dont now if is the better way, but, the above issue can fixed adding this lines of code before the line forty six of shortcut.js:


// The user press "s" key and not only the F4 key
if( (code == 115) && (character == 's') ) character = '';
// The user press "t" key and not only the F5 key
if( (code == 116) && (character == 't') ) character = '';
// The user press "u" key and not only the F6 key
if( (code == 117) && (character == 'u') ) character = '';


Hope be usefull for anyone. Thanks a lot for your shortcut.js library :)