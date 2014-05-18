# Save files when focus is lost

## UPDATE: This has been added natively to TextMate 2.0-alpha.9545 :)

See the commit message on https://github.com/textmate/textmate/commit/42888110fbc664bce8954ad2ebf3160e58db02bf

From the release notes:

> You can now set `saveOnBlur` in `.tm_properties` to make TextMate save files when focus is lost. Previously the recommended way was to create a command set to “Save Modified Files” with a semantic class of `callback.application.did-deactivate`, though incase of a save error, such command would bring up UI where saveOnBlur will ignore errors. Using `.tm_properties` also allows to easily target specific file types, for example one could use:
>
>      [ ui/**.php ]
>      saveOnBlur = true
>
> This would then only have .php files in the ui folder auto-save when focus is lost.

The rest of this README (and the code in this repo) is left here for historical reasons :)

## What's this

There's a preference, hidden somewhere deep in TextMate 1, that allows it to save all unsaved files when the application loses the focus.

I loved it for web development, and couldn't believe it was dropped from TextMate 2.

However, it has been replaced by something even more amazing: you can now hook into the "focus lost" event and do all sort of things with your files.

This command re-enables the old behaviour (save all unsaved files when focus is lost), but can be easily tweaked to have TextMate save only some types of files (you can fill the 'Scope Selector' with just the file types you want saved, i.e: text.html, source.css...)


## Installation

- Clone the git repo to  `~/Library/Application Support/TextMate/Managed/Bundles`
- Relaunch TextMate 2

## Note

You need to be using a recent build. Open Preferences » Software Update and **ALT-click the "Check Now"** button to get the most recent nightly build (this will grab a latest version than the one you get by just clicking the button).


Enjoy it!
