![Action Shot](/images/Pepper_thumb_1.jpg)

[![YouTube Channel Views](https://img.shields.io/youtube/channel/views/UCz5BOU9J9pB_O0B8-rDjCWQ?style=flat&logo=youtube&logoColor=red&labelColor=white&color=ffed53)](https://www.youtube.com/channel/UCz5BOU9J9pB_O0B8-rDjCWQ) [![Instagram](https://img.shields.io/github/stars/veebch?style=flat&logo=github&logoColor=black&labelColor=white&color=ffed53)](https://www.instagram.com/v_e_e_b/)

# Pepper Pi

How to build the floating transparent display for a Raspberry Pi 5 described in the build video.

## Build Video

[here](https://www.veeb.ch/projects/the-valley-beneath-the-pepper-dome)

The video contains (at least) one error. The reflector angle for a dome that is on a desk is should be *more* than 45 degrees, not less. So the cut angle that is used in the shape calculator should be 60, not 30 degrees.


## Components
- Raspberry Pi 5 (any model of the 5 should work)
- Round DSI LED screen (3.4inch (86mm) Waveshare)
- Glass dome (the one used in the video is 90mm diameter, internal diameter is ~87mm)
- Acrylic Reflector
- 3d Printed Enclosure



## OS commands
To flip the display for reflection:
```
wlr-randr --output DSI-2 --transform flipped-180
```
alias for the ```dome``` command (depends on [mpv](https://github.com/mpv-player/mpv))

```
alias dome='mpv  --fs --fs-screen=1'
```
Videos that are sent to the screen should be 800x800 videos. 

For music visualisation, use [cava](https://github.com/karlstav/cava) on a terminal that has been maximised on the display.

## Enclosure 

The files for the 3d printed enclosure are in the directory [3d](./3d)

## Reflector Shape Calculator

Depending on the diameter of the dome and the typical view angle, the shape of your reflector will change. To save you some work, we've made a calculator that will give you a template for the shape reflector that you need to use. The calculator is [here](https://www.veeb.ch/projects/the-valley-beneath-the-pepper-dome)






