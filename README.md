A wallpaper template for mjswensen/themer.

## Installation & usage

Install this module wherever you have `themer` installed:

    yarn add themer-wallpaper-block-wave

Then pass `themer-vim` as a `-t` (`--template`) arg to `themer`:

    themer -c my-colors.js -t themer-wallpaper-block-wave -o gen

`themer-wallpaper-block-wave` will generate SVG and PNG wallpapers to the output directory (`gen/` in this example).

### Default resolutions

By default, `themer-wallpaper-block-wave` will output wallpapers at the following sizes:

* 2880 by 1800 (desktop)
* 750 by 1334 (device)

### Custom resolutions

`themer-wallpaper-block-wave` adds the following argument to `themer`:

    --themer-wallpaper-block-wave-size

to which you would pass `<width>x<height>`. For example, to forego the default resolutions and generate two wallpapers, one 1024 by 768 and one 320 by 960:

    themer -c my-colors.js -t themer-wallpaper-block-wave --themer-wallpaper-block-wave-size 1024x768 --themer-wallpaper-block-wave-size 320x960 -o gen

## Previews

The following are rendered using themer's default color set (mjswensen/themer-colors-default):

![dark desktop](/assets/desktop-dark.png)
![light desktop](/assets/desktop-light.png)
![dark device](/assets/device-dark.png)
![light device](/assets/device-light.png)