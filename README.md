# Atom Ctags Package [![stable](http://badges.github.io/stability-badges/dist/stable.svg)](http://github.com/badges/stability-badges) [![Make a donation via Paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=lx1988cyk%40gmail%2ecom&lc=US&no_note=0&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHostedGuest)


This package uses：
[ctags](http://ctags.sourceforge.net),
[autocomplete-plus](https://github.com/saschagehlich/autocomplete-plus)
and fork from [symbols-view](https://github.com/atom/symbols-view)

#Features
* **AutoComplete with ctags**
* **Auto Update the file's tags data when saved**
* go-to-declaration and return-from-declaration
* toggle-file-symbols
* toggle-project-symbols
* "Rebuild Ctags" in context-menu
* "Auto Build Tags When Active" setting, default: false
* 'extraTagFiles' setting, add specified tagFiles.(Make sure you tag file generate with --fields=+KSn)
* 'cmdArgs' setting, add specified ctag command args like: --exclude=lib --exclude=*.js
* 'buildTimeout' setting, specified ctag command execute timeout

![atom-ctags](https://cloud.githubusercontent.com/assets/704762/3483867/e0bac2ee-0397-11e4-89c1-70689f6b8ff3.gif)

#Install
**You can install atom-ctags using the Preferences pane.**
And please Make sure that [autocomplete-plus](https://github.com/saschagehlich/autocomplete-plus) already installed.


#TODO
* Merge [symbols-tree-view](https://atom.io/packages/symbols-tree-view)
* ~~Submit to atom package center~~
* ~~Modify package name~~
* Performance optimization
* Disk file cache
* Release memory when deactivate
* Appearance improve
* Writing Tests
* Auto check package of autocomplete-plus installed
* ~~Auto disable package of symbols-view~~
* ~~use Activation Events to speed up load time~~
* ~~use ctags command args -R~~


#Changelog
* go-to-declaration support column
* Optimization for duplicate results [#3](https://github.com/yongkangchen/atom-ctags/issues/3)
* [speed tag parse by use ctag command param to parse line number instead of fs-plus](https://github.com/yongkangchen/atom-ctags/commit/784160320309212d0acf865092133ba55980c605)
* [`use -R instead of (fs-plus).traverseTreeSync` and `search tag limit max`](https://github.com/yongkangchen/atom-ctags/commit/4e4df478c2a00b83143e1887a8b6fd6c5067ce95)
