# Matrix-Screensaver
Falling code rain screensaver inspired by The Matrix using `<canvas>`.
Created a year ago as a side project, but I dragged it out of my files and tweaked it a bit.
No need to set up anything, simply download the .html file and open it (not as a plain text file!).
Mobile platforms are not supported.
There *will* be bugs.

> [!CAUTION]
> Even though this is a screensaver, it doesn't actually lock your PC/laptop. Due to the limitations of web applications, I'm not able to implment a secure screensaver. If you use this screensaver and leave your device unattended, somebody could easily access **all of your sensitive information**. Do not blame me if you get hacked.

**This project was created as a hobby - performance was/is not a piority. To increase performance, set `improvedGlowing: false`, reduce glow, or use `fixedSpeed: true` with a low speed.**

### TO-DO
- Add real-time settings menu
- Dyamic canvas size, for example, when resizing the browser tab.

### Feature List
| Feature             | Description                                                                                   |
|---------------------|----------------------------------------------------------------------------------------------|
| 3D Projection       | Optionally enables pseudo-3D effect by varying font sizes                                    |
| Glow & Afterglow    | Adjustable glow intensity and afterglow effects                                              |
| Customizable Colors | Full control over rain, shadow, background, and glow colors                                  |
| Lightning Flashes   | Simulates brief flashes like lightning, adding atmosphere                                    |
| Density & Speed     | Fine-tune the density and fall speed of the rain                                             |
| Interactive         | Canvas reacts to clicks with bursts of colored lines                                         |
| Performance Tuning  | Switch between fixed interval and requestAnimationFrame for best performance on each device   |
| Glitch Effect       | When clicking anywhere on the screen, many colored lines will appear on the screen as a burst.|

### The `settings` object
| Property          | Type    | Description                                                                                               |
|-------------------|---------|-----------------------------------------------------------------------------------------------------------|
| three             | Boolean | Enable pseudo-3D projection (font size variation)                                                         |
| darkness          | Float   | Controls "fade out" speed (0-1, higher = faster fade)                                                     |
| glow              | Number  | Size of the glow effect in pixels                                                                         |
| size              | Number  | Base font size in pixels (ignored if `three` is true)                                                     |
| speed             | Number  | Milliseconds between frames (ignored if `fixedSpeed` is false)                                            |
| range             | Float   | Density/spread of rain (0-1, higher = less rain)                                                          |
| fixedSpeed        | Boolean | If true, uses setInterval; if false, uses requestAnimationFrame for smooth animation                      |
| improvedGlowing   | Boolean | Enables heavy afterglow/halo (resource intensive)                                                         |
| lightning         | Float   | Frequency of flashes (1 = off, lower = more flashes, 0-1)                                                 |

### The `colors` object
| Property              | Description                                       | Default      |
|-----------------------|---------------------------------------------------|--------------|
| backgroundColorRed    | Red channel for bg (0-255)                        | 0            |
| backgroundColorGreen  | Green channel for bg (0-255)                      | 0            |
| backgroundColorBlue   | Blue channel for bg (0-255)                       | 0            |
| shadowColor           | Color of the shadow/glow                          | "limegreen"  |
| matrixRain            | Color of trailing rain characters                  | "#38d914"    |
| leadingMatrixRain     | Color of lead character                            | "white"      |
| improvedBlurRed       | Afterglow red intensity (multiplier)               | 0            |
| improvedBlurGreen     | Afterglow green intensity (multiplier)             | 1            |
| improvedBlurBlue      | Afterglow blue intensity (multiplier)              | 0            |

### Screenshots
![Core](https://github.com/010ender/Matrix-Screensaver/blob/main/Core.png)
*The fastest and simplest version, Core.*


![Deep Ocean](https://github.com/010ender/Matrix-Screensaver/blob/main/Deep%20Ocean.png)
*Chilly and blue. In that dark abyss you would never know if something is watching you.*


![Default Green](https://github.com/010ender/Matrix-Screensaver/blob/main/Default%20Green.png)
*The default color preset.*


![Glitched Mainframe](https://github.com/010ender/Matrix-Screensaver/blob/main/Glitched%20Mainframe.png)
*Glitchy! Bugs everywhere.*


![Infernal Flames](https://github.com/010ender/Matrix-Screensaver/blob/main/Infernal%20Flames.png)
*Made to look like the Nether in Minecraft.*
