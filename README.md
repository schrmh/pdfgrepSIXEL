# pdfgrepSIXEL  

## *A tool inspired by pdfgrep that displays not text but pdf pages as results.*  

### Usage: `./pdfgrepSIXEL 'String'`  
**You need a SIXEL capable terminal for this to work!**   
*E.g. xterm. Some popular terminal emulators like xfce4-terminal don't have SIXEL support.*    

### Preview:  
![Example image showing simple usage and output of pdfgrepSIXEL](/example.png?raw=true "Example image showing simple usage and output of pdfgrepSIXEL")  

#### Making the changes to xterm  
Download [xterm](https://invisible-island.net/datafiles/release/xterm.tar.gz) and compile it with the needed options:  
```
tar -xzf xterm.tar.gz  
cd xterm-353/  
./configure --enable-dec-locator --enable-sixel-graphics --with-terminal-id=VT340  
make  
sudo make install  
sudo make install-ti  
```
Add to ~/.Xresources:
```
XTerm*allowWindowOps: true  
XTerm*decTerminalID: vt340  
XTerm*sixelScrolling: true  
XTerm*regisScreenSize: 1920x1080  
XTerm*numColorRegisters: 256  
```
Apply changes: `xrdb ~/.Xresources`

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
- Maybe not all found pdf pages will be displayed..
