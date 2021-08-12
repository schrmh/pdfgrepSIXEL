# pdfgrepSIXEL  

## *A tool inspired by pdfgrep that displays not text but pdf pages as results.*  

### Usage: `./pdfgrepSIXEL 'String'`  
**You need a SIXEL capable terminal for this to work!**  
*[st-flexipatch](https://github.com/bakkeby/st-flexipatch) works best with my script from my experience.  
You could also use [xterm](https://invisible-island.net/datafiles/release/xterm.tar.gz) or [mlterm](http://mlterm.sourceforge.net/) but those will most likely remove SIXELs before all the found pages are displayed.  
Also note that most terminal emulators don't support SIXEL but it is more adopted than other competitors.*    

### Preview:  
![Example image showing simple usage and output of pdfgrepSIXEL](/example.png?raw=true "Example image showing simple usage and output of pdfgrepSIXEL")  

### Possible future features:  
- (No) duplicate pages  
- Highlight text inside pages  
(- display numbers next to pages for those operations:)  
- Edit a page in an external editor (text or graphical)  
- See adjacent pages  
- Custom page size
- Auto resize pages when terminal size changes

### "Bugs":  
- Only one word is searchable (no space)  
- Page numbers could hide stuff..
- Page numbers >999 won't be visible
