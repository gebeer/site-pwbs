# pwbs
*bootstrap-sass-official fontawesome blank site profile for ProcessWire*

This blank site profile for ProcessWire CMS/CMF features:
- bootstrap-sass-official
- font-awesome SASS version
- jquery
- modernizr
- render functions for:
  - BS3 dropdown menu
  - BS3 accordion from PageArray
  - BS3 carousel from PW images array

##Prerequisites
- [compass](http://compass-style.org/install/)
- [bower](http://bower.io/#install-bower)

##How to install
**from zip:**
1. download the [zip](https://github.com/gebeer/pwbs/archive/master.zip)
2. extract the folder "site-pwbs" into a clean [ProcessWire](https://github.com/ryancramerdesign/ProcessWire) install's root folder
3. during install of ProcessWire choose the profile "bootstrap-sass-official fontawesome blank profile" 

**git clone:**
1. copy [ProcessWire](https://github.com/ryancramerdesign/ProcessWire) to your projects root folder
2. open a terminal in that root folder and execute `git clone https://github.com/gebeer/site-pwbs.git`
3. during install of ProcessWire choose the profile "bootstrap-sass-official fontawesome blank profile" 

##After installation
The last step after installing the profile is to install all assets with bower:
- open a terminal in site/templates and execute `bower install`

##How it works
The profile is based on the blank site profile that comes with PW 2.5 and uses the delegate template approach. It comes with a top navbar, a main container and a footer section. Rest is up to you.
 
###CSS
gets compiled through compass. You can easily override BS variables and exclude BS components that you don't need. I intentionally did not add structure to the sass folder so you can structure your partials yourself as you please. There is only one folder "generic" with _mixins.scss whith a very lean and flexible breakpoint mixin that I discovered here.
 
###JS
Since I only use the BS javascript plugins I really need, I usually copy them over to my plugins.js file.

###Why bower? 
I use bower to install bootstrap-sass-original and fontawesome because it gives more flexibility than requiring them through ruby gems. This way you can tweak the BS and FA partials to your liking  (of course only if you don't intend to do "bower update" further down the road)

[PW Forum thread](https://processwire.com/talk/topic/9584-bootstrap-3-sass-fontawesome-blank-site-profile/) 

Enjoy!
