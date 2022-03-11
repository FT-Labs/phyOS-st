### St (Simple terminal) for dwm-phyOS

 - Installation for arch users
 Check link below to append phyOS repo in your **/etc/pacman.conf**
 
 [dwm-phyOS](github.com/phytech-r0/dwm-phyOS)

 After adding the repo, install easily with:
 
    pacman -S st-phyOS fonts-phyOS
    
 - Installation for any distro
 You need to install fonts to your system first (Nerd fonts, including all glyphs etc.):
 
    	git clone github.com/phytech-r0/fonts-phyOS
	cd fonts-phyOS && sudo mv *.otf *.ttf /usr/fonts/ttf
	sudo fc-cache
 After that, install st with:
 
    	git clone github.com/phytech-r0/st-phyOS
	cd dwmblocks-phyOS && make && sudo make install

## Default keybinds

<div align="center">

Key Combination | Action
----------------- | ----------
 <kbd>Alt</kbd> + <kbd>Shift</kbd> + <kbd>j</kbd>     | Decrease font size (zoom -)
 <kbd>Alt</kbd> + <kbd>Shift</kbd> + <kbd>k</kbd>     | Increase font size (zoom +)
 <kbd>Alt</kbd> + <kbd>o</kbd>      | Copy output of command
 <kbd>Alt</kbd> + <kbd>;</kbd>      | Cycle fonts

</div>
<div>
