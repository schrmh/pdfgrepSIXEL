# pdfgrepSIXEL  

## *A tool inspired by pdfgrep that displays not text but pdf pages as results.*  

### Usage: `./pdfgrepSIXEL 'String'`  
**You need a SIXEL capable terminal for this to work!** (See https://www.arewesixelyet.com/)  
*[Konsole](https://konsole.kde.org/) works best with my script from my experience (but you might want to increase its [Scrollback](https://docs.kde.org/stable5/en/konsole/konsole/scrollback.html) buffer size).  
You could also use [xterm](https://invisible-island.net/datafiles/release/xterm.tar.gz) or [mlterm](http://mlterm.sourceforge.net/) but those will most likely remove SIXELs before all the found pages are displayed.  
Also note that most terminal emulators don't support SIXEL but it is more adopted than other competitors.*    

### Preview:  
![Example image showing simple usage and output of pdfgrepSIXEL. User searched for text Quanten and got displayed a few PDF pages from two pdf documents within a terminal emulator.](/example.png?raw=true "Example image showing simple usage !and !output of pdfgrepSIXEL")

### Features:
- Orange results per page number (hide with `--no-result-numbers`)
- Scale (all sides of) pages to size in pixel by using `--scale-to`  
Parameter order doesn't matter but the search string has to come last.

### Possible future features:  
- Further passing of parameters to pdfgrep
- Search of individual files
- Recursive search
- (No) duplicate pages  
- Highlight text inside pages (very hard with shell script utilities alone...)  
Optionally wrap the thing to allow the following operations (shortcuts next to pages):
- Edit a page in an external editor (text or graphical)  
- See adjacent pages  
- Resize (single/all) pages after output  
- Auto resize pages when terminal size changes
