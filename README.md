# ubuntu-maintenance-scripts

This repository contains my personal debian ubuntu desktop maintenance scripts To use simply create a bin folder in /home/{user} folder and place them there and add the new bin folder to PATH. to do this open .bashrc file in your home directory with gedit, nano etc... and add the next line to it (without the quotes)

"export PATH:~/bin:${PATH}"

then save the file.

Feel free to fork or download these scripts and use them as-is or edit them for your own use, I have added the GPL3 licence to comply with sharing requirements and do not claim copyright as most of the information gathered to enable writing them was found on the web.

once the PATH variable is set correctly

I hope everyone finds these scripts useful and maybe educational too.


the scripts included are as follows...
	
	abu	->  apt-build update
	ac	->  apt-clean
	adb-bootloader ->  reboot android to bootloader (assumes android-debug-bridge {adb} installed)
	ah	->  list all apt packages on hold
	ali ->  lists all installed apt packages in terminal and makes an apt-installed-list file
	        in current working directory
	arem ->  apt autoremove
	aria2files -> wrapper script for aria2c download tool (assumes aria2 installed)
	auto-dkms -> reloads dkms  (assumes debian kernel module support {dkms} installed)
	bb ->  basic build (performs a standard configure, build and install with gcc)
	bdeb ->  build debian package script (dpkg-buildpackage assumes fakeroot,time and dpkg-dev
	         installed)
	cpd  ->  copy apt downloaded packages to current directory and clean apt-cache
	dcfg  ->  reconfigure installed packages with dpkg
	dup  ->  do a distribution update/upgrade and clean apt-cache
	fbi  -> fix broken and missing debian packages
	fix  ->  fix it script to repair problems with apt not working correctly
	font-fix  ->  reloads font-cache after new font install
	genb ->  general build and install script
	gencmake ->  build and install program with cmake
	genmes  ->  build and install program with mesonbuild
	gt  ->  google search engine in terminal
	htr  -> cleans hidden trash files from /home/{user} directory
	i ->  intelligent install script (only updates or installs missing packages, won't downgrade
	      anything) use from folder containing .deb packages
	ipy  ->  python3 setup.py install script (download package from Pypi, unpack and run)
	isorun  ->  boot an .iso with qemu
	kp  ->  make debian kernel package script (using make-kpkg) assumes fakeroot, make-kpg installed
	kpc  ->  cleans source directory after failed build with kp above (useful for editing source code)
	kps  ->  rebuild kernel after running above script without reconfiguring (as done by kp script)
	ldcon  ->  ldconfig script (update system info after new build/install of binaries)
	lrem  ->  removes apt locks that prevent installing packages with apt
	pb ->  build debian package from .dsc file with pbuilder and copy result to 
	       wherever terminal was opened
	pbcl  -> pbuilder clean script
	pbcr  ->  creates a base.tgz for pbuilder using hirsute hippo as base
	pbu  ->  updates a base.tgz build with pbuilder
	r2d  ->  convert .rpm to .deb script with alien (assumes alien installed)
	rr  -> remove recursive script...
           (careful when using this it WILL remove EVERYTHING from current directory!!)
    rsp  ->  refresh all snap packages
    swap4g  ->  delete current /swapfile and create new 4G one
    ui  ->  update-initramfs and grub (all kernels)

