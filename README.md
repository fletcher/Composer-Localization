Composer-Localization
=====================

String files for localizing the MultiMarkdown Composer application


FYI, the `master` branch is the default English localization.


## What is this? ##

MultiMarkdown Composer is a commercial application, but it's not so
big that I can afford to hire translators to localize the app into
countless languages.  People across the world have asked me about
this, so I decided that I would at least make the necessary files
available to help crowdsource the localization if anyone is
interested.  This way, there is at least the possibility of localizing
to other languages if there is enough interest and support.  I'll do
what I can to help.

Basically, you use the files as a template to translate to your
desired language.  Once complete (or complete-"ish") I can use these
to generate the necessary files for the app to be localized.



## What are these files?


The files, listed in rough order of priority, are:

* MainMenu.strings -- strings for the menu bar and other general UI elements

* FTPSmartTextView.strings -- strings for the HUD panels

* Localizable.strings -- General strings

* Preferences.strings -- strings for the preference dialog

* Composer.strings -- strings for the app itself



## Create a new language localization ##

You will need to clone the repo, and then create a new branch.

Use the lowercase two-letter code as the branch title (e.g. `en`,
`de`, etc.)  This branch title will be used as the localization
directory name (e.g. `en.lproj`, `de.lproj`, etc.).


## Update translations ##

Working in the files above, you will need to modify the string to fit
the desired language.  For example:


	/* Metadata HUD title */
	"Metadata" = "Metadata";

The first line is a description of what we are talking about.

The second line contains the `key` (don't change this), followed by
`=`, and then the text to be used.  It's this *second* word or phrase
that you should change.  For example:

	/* Metadata HUD title */
	"Metadata" = "Something new";

This would cause the HUD name to be "Something new" instead of "Metadata".


## Sharing your changes ##

You'll need to send me a pull request for your changes.  That's
outside the scope of this how-to.

If you're good at translating, but not so good at git/github, then
contact me and we can work something out -- you can send me the files
and I'll upload them.


## Quality control ##

I need to be careful that the translations are accurate, which means
I'll need to get them vetted somehow before releasing them.  I'll be
relying on Twitter/website announcements for help.

I'll probably start by incorporating these into the Non-Sandboxed
version before trying to get them into the App Store version.
