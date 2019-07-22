pdfgrepSIXEL
------------

A tool inspired by pdfgrep that displays not text but pdf pages as results.

Usage: `./pdfgrepSIXEL 'String'`  
**You need a SIXEL capable terminal for this to work!**   
*E.g. xterm. Some popular terminal emulators like xfce4-terminal don't have SIXEL support.*    


Possible future features:
- No duplicate pages
- Highlight text inside pages
(- display numbers next to pages for those operations:)
- Edit a page in an external editor (text or graphical)
- See adjacent pages

"Bugs":
- Only one word is searchable (no space)
- Too many pdf files won't work because of loop with uppercase letters (see code)
