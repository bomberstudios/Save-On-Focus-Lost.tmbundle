# Save files when focus is lost

There's a preference, hidden somewhere deep in TextMate 1, that allows it to save all unsaved files when the application loses the focus.

I loved it for web development, and couldn't believe it was dropped from TextMate 2.

However, it has been replaced by something even more amazing: you can now hook into the "focus lost" event and do all sort of things with your files.

This command re-enables the old behaviour (save all unsaved files when focus is lost), but can be easily tweaked to have TextMate save only some types of files (you can fill the 'Scope Selector' with just the file types you want saved, i.e: text.html, source.css...)


## Installation

- Clone the git repo to  `~/Library/Application Support/Avian/Bundles/`
- Relaunch TextMate 2

## Note

You need to be using a recent build. Open Preferences » Software Update and **ALT-click the "Check Now"** button to get the most recent nightly build (this will grab a latest version than the one you get by just clicking the button).


Enjoy it!
