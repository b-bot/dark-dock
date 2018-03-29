An ongoing project to create grayscale versions of the most commonly used Mac apps. Inspired by the lack of a dark theme for macOS.

### Before

![Screen Shot 2018-03-29 at 18.54.37.png](https://github.com/byronpolley/dark-dock/blob/master/resources/C21F101BB1CD207F0F36474DAA1ECF30.png)

### After

![Screen Shot 2018-03-29 at 18.58.16.png](https://github.com/byronpolley/dark-dock/blob/master/resources/C824210A7F95993F2F735DE60FD71D2C.png)

## Installation

1. Download the repository.
2. Download and install [Image2Icon](http://www.img2icnsapp.com).
3. The `grayscale` folder contains all of the icons in black and white.
4. Drag the `.icns` file of the desired app over the colour version within the LiteIcon panel.
5. Click **Apply Changes**.
6. Open/Close and Reopen the app to see changes.

### Changing icons with System Integrity Protection (SIP) enabled

The majority of system applications cannot be changed using LiteIcon due to a macOS security feature called SIP. LiteIcon warns you the first time opening it of this with the following prompt.

![Screen Shot 2018-03-29 at 18.15.46.png](https://github.com/byronpolley/dark-dock/blob/master/resources/4856009127EFDCA0371491CFE34BDC53.png)

You will have to disable SIP temporarily with the following steps:
1. Restart your Mac.
2. Before OS X starts up, hold down Command-R and keep it held down until you see an Apple icon and a progress bar. Release. This boots you into Recovery.
3. From the Utilities menu, select Terminal.
4. At the prompt type exactly the following and then press Return: `csrutil disable`
5. Terminal should display a message that SIP was disabled.
6. From the  menu, select Restart.
7. All of the disabled icons will now appear in the LiteIcon interface.
8. Make sure to re-anable SIP once done using the same steps except `csrutil enable`. This is important for security.

## Contribution / Modification

There is an `icons.sketch` file included for users who wish to contribute or modify the existing icons for their own usage.

* Open the `icons.sketch`
* Go to `Applications/**Example.app**/`
* Right-click and `Show Package Contents`
* The original icon is always in `Content/Resources`.
* Copy the icon and rename accordingly and place in the `original` folder.
* With Sketch open copy into `icons.sketch` as a layer.
* There is only one panel you need to use to get the image grayscale. With the icon selected tick `Color Adjust` in the right-hand sidepanel.
* Adjust **Saturation** to 0. Using a combination of **Brightness** and **Contrast**, adjust settings until there is a strong white/black contrast that should flatten the image. Ensure not to omit critical details for aesthetical reasons. I have found flat icons work better than detailed ones.
* Export the layer @2x PNG.
* Download the [Image2Icon](http://www.img2icnsapp.com) app and import `.png` and export `.icns` for use.
* If contributing commit ONLY the `.icns` files for the original and grayscale, NOT the `icons.sketch` file.

## Help / Get In Touch

Instagram: [@b_b0t](https://instagram.com/b_b0t)
Twitter: [@b_b0t](https://instagram.com/b_b0t)
