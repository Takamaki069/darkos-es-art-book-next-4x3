# darkos-es-art-book-next-4x3

Before to begin, thanks to; 

> previous version: https://github.com/mute-key/arkos-es-art-book-next-4x3

## Introduction

The original theme by mute-key this is based on was awesome but I found it started to lack systems under dArkOS and the original repo was locked, so I opted to fork it and push some updates as I do them on my own fork! I will continue to update this page and the theme when I get time but cc licence and credits are already in place as per the source I forked from!

## Preview 

I do not own a capture card so i couldn't take the screenshot so this is the best i can do. i was working through ssh and was hoping to be able to take screenshots but scrot would not work because the frontend is not x-window ofc. 

you can see there is an transparent layer between system logo and carousel. the default contrast between the selected systems was not enough for my likings. the extra layer really made the selected system image to stand out than the others and more interesting to slide it through. you can remove the contrast layer, set bezels or change the opacity of the layer in the theme options. 

<img src=".showcase/systemview.jpg" width="520" height="299">
<br>
<img src=".showcase/overlay.gif" width="520" height="299">

## Changes from previous theme

I added and modified few things here and there. some of the changes are as follow;

* Added new transparent layer in system-multi view for better contrast and option to select the contrast ratio in `Theme Configuration -> Overlay Transparency`;
    - Medium (default) 
    - Light
    - Very Light
    - Dark 
    - Very Dark
* The bezel options you can choose in `Theme Configuration -> System select Overlay`; 
    - Side bezel
    - All-side bezel
    - No bezel 
    - No overlay
* Moved clock to top left and adjusted cordinate
* Moved battery indiciator to top right and adjusted cordinate
* Changed battery indiciator to frontend default and added spacing between icon and text
* Added option to select system images between default and custom in `THEME CONFIGURATION -> SYSTEM VIEW: IMAGE`. You can change theme also.
    - Added custom system images;
        - __nes__: *mega man 3*
        - __gb__: *pokemon yellow*
        - __gbc__: *pokemon trading card game*
        - __gba__: *final fantasy tactics advance*
        - __neogeo__: *kof98*
        - __satern__: *castleveina symphony of the night*
        - __nds__: *professor layton curious village*
        - __psx__: *valkyrie profile*
        - __psp__: *monster hunter portable 3rd*
        - __mame__: *arcade pixel art from [Link](https://www.reddit.com/r/readyplayerone/comments/116gill/i_drew_this_pixel_art_of_an_old_arcade_and_called/)*
        - __last-played__: *bookshelf pixel art from [Link](https://www.reddit.com/r/PixelArt/comments/11m1fcp/bookshelf/)*
* Added option to select the font size `THEME CONFIGURATION -> SYSTEM VIEW: FONT SIZE`. To change the font size, the font size values are in **./__inc/lang/font-size-*.xml**.
    - Default (1x)
    - Medium (1.1x)
    - Large (1.2x)
    - Very Large (1.3x)
    - Max (1.4x)
* Added option to select how many systems to display on system view on `Theme Configuration -> SYSTEM VIEW: DISPLAY `
    - 5 Systems
    - 3 Systems (this seems to be the visual setting for a lot of 1x1 screen aspect ratio devices)

    
## Sidenote (Disclaimer)
<!-- https://stackoverflow.com/questions/1027179/displaying-svg-in-opengl-without-intermediate-raster -->
<!-- systemctl restart emulationstation -->
<!-- /sys/class/power_supply/battery/capacity -->
<!-- https://github.com/hardkernel?tab=stars -->

You do not need to read this unless you want to edit the theme for yourself but here is the list of my findings for the future just in case if i want to come back and add more stuff.

 -  WiFi Indicator could not be displayed on the versions of the frontend of my device. The only way to check the WiFi connection was through the main menu. I do not own devices other than rg353m so i could not check. 

-  variable elements can't be re-assigend with other value once it is assigned. 

-  variable elements can't be concatinated with other variable elements itself

-  game count on screen is hardcoded, had to find a workaround [Link](https://retropie.org.uk/forum/topic/23252/emulationstation-theme-systeminfo). the version of the EmulationStation does not allow condition checks such as `IfSubset`.

-  `batteryIndiciator` element would not work with alignment. therefore the element will render based on coordinate of left corner of the element. this ends up making 'icon with text' near impoosible to position it perfectly on top-right on the screen as the width of percentage text increases or decreases per remaining battery. the soluttion was to pushing out the batteryIndiciator text out of the screen.  


## **Acknowledgments**
* Previous version from: https://github.com/mute-key/arkos-es-art-book-next-4x3
* Original theme : https://github.com/anthonycaccese/art-book-next-jelos
* Referenced Theme :  https://github.com/nkahoang/es-theme-art-book-next-arkos
* Referenced Theme :  https://github.com/Jetup13/es-theme-sagaartbook
* Most system logos were sourced and modified from the excellent work done by Dan Patrick [here](https://archive.org/details/console-logos-professionally-redrawn-plus-official-versions).  I modified each to be compatible with EmulationStation's current SVG support.
* ChangaOne font is by [Eduardo Tunni](https://www.fontsquirrel.com/fonts/changa)
* Oxygen font is by [Vernon Adams](https://www.fontsquirrel.com/fonts/oxygen)
* Auto-Collection Genre background art created by [@nautipuss](https://github.com/nautipuss)
* Metadata Icons sourced from [FontAwesome](https://fontawesome.com/search?o=r&m=free)

## **License**
(Attribution back to the OG repo by `anthonycaccese`: https://github.com/anthonycaccese/art-book-next-es)
Creative Commons CC-BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/2.0/
You are free to share and adapt this theme as long as you provide attribution back to me (and the above credits) as well share any updates you make under the same licence terms.
