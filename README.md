# Digger
A client with which to access _gopherspace_.

## Gopher
[_Gopher_](https://en.wikipedia.org/wiki/Gopher_(protocol)) is a communications protocol that, in the early 90s, competed (briefly) with what became the world wide web. _Gopher_ serves up files and text based menus. As such, it is much lighter weight than HTML documents and the like served over http. Due to its text based nature it also has the benefit of being reliable in its visual output and style, and for being relatively accessible. 

## Digger
The following is a list of current and future Digger features:

- Tk based GUI
    - Back button, move backwards in session history
    - Forward button, move forward in session history
    - Refresh button, will be replaced by a favorite button _(non-functional)_
    - Home, shows favorites and is a start page _(non-functinoal)_
    - An address bar, on __ENTER__ submits a request for a _gopher_ page
    - Settings button _(non-functional)_
    - A display area for the requested information
    - Scroll bar, scrolling works, but no bar is present _(non-functional)_
    - A status bar to display various information
- Links to menus and files
    - On hover, link destination shows in status bar
    - On hover, link is underlined
    - Links are colored differently from regular text _(configurable)_
    - Link type appears next to link in noticeable coloring _(configurable)_
    - On primary click, destination is loaded and new location replaces old location in address bar
    - On primary click, link background changes to visually confirm click _(configurable)_
    - Cursor is a pointer over links, while regular text is an I-beam cursor.
- Menus Pages and files
    - Menus display correctly and quickly
    - Text files display correctly and quickly
    - Images files _(non-functional)_
    - Sound files _(non-functional)_
    - Binary files _(non-functional)_
    - HTML files, will open in default browser _(non-functional)_
    - Interactive pages/search _(non-functional)_
- History
    - Session based history for backward and forward navigation
    - Persistent favorites _(non-functional)_
    - Suggestions on URL entry based on persistent history _(non-functional)_
- Application settings and menus
    - Settings menu _(non-functional)_
        - Color themes
        - Icon themes
        - History settings
        - Files/download settings
    - Secondary click context menus for text manipulation & file saving _(non-functional)_
    - Page saving for offline viewing _(non-functional)_
    - Hotkey to view raw page source for menus _(non-functional)_
- Errors
    - Error warnings to user _(non-functional)_
    - Error page on bad/malformed request _(non-functional)_
    - Error display for type 3 server response _(non-functional)_


## Installation

Digger requires python3 to be installed on the system prior to running.
    # can be prefixed with python3
    # but not required if you have python3 installed
    /path/to/digger.py
On some linux distributions an additional package for tkinter may be required.
If you get a console error complaining about tkinter try the following (or equivalent for your package manager):
    sudo apt-get python3-tk
Once up an running you should be good to go.


## Distribution

Digger's primary system target is linux. Once a version 1.0 is reached the plan is to distribute primarily through [Snapcraft](https://snapcraft.io/) packages. 

Some version of windows executable may come along as well, depending on configurability of build tools (py2exe, freeze, etc) for windows executables and time.
