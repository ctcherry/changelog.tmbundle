Changelog Bundle
================

A TextMate bundle that helps create changelog entires. The hope is by making it easier to add items to a changelog people will update it more regularly.

The changelog entry format created by this bundle looks like this:

    2009-01-08 - Chris Cherry (ctcherry@gmail.com)
    	* Description of change number 1
    	* Description of another change

Installation
------------

    mkdir -p /Library/Application\ Support/TextMate/Bundles
    cd /Library/Application\ Support/TextMate/Bundles
    git clone git://github.com/ctcherry/changelog.tmbundle.git

Usage
-----

Changelogs are automatically recognized if they have the header format specified above as their first line.

Set the `TM_CHANGELOG_NAME` variable to the string you want to appear in the changelog entry header. Some combination of your name, username or email, is most common.

Make sure the file language is set to "Changelog text" (use the menu at the bottom of the TextMate window)

Typing 'ch' and hitting tab will insert the header with the correct date and name variable you entered above, put you on a newline with an asterisk and you are ready to type your first description line. Hitting enter will line break and indent you properly to insert another item.