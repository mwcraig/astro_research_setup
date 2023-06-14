# Information and settings for Andor/Apogee Alta CG16M

## Camera parameters

+ Name: `Apogee Alta CG16M`
+ Gain: `1.45 electron/ADU`
+ read noise: `9` electrons
+ dark current: `0.01 electron/pixel/sec` typical, but there are hot pixels
+ linearity limit: `35000 ADU`
+ Pixel size: 9 micron
+ Number of pixels: 4096 x 4109 (includes overscan)


## Reduction settings

### All images

+ Do not use the overscan
+ Trim to all of first axis, 4096 on second axis

### Reducing bias images

+ Only need to trim

### Combining bias

+ Choose sigma clipping, upper and lower bounds of 5.
+ Combine using mean/average

### Reducing darks

IF THE DARK EXPOSURE TIME DOESN'T MATCH ANY OF The OTHER IMAGES:

+ Trim
+ Subtract bias

### Combining darks

+ Choose sigma clipping, upper and lower bounds of 5.
+ Combine using mean/average
+ Group by exposure time

## Reducing flats

+ Trim
+ Subtract bias
+ Subtract dark
    - Scale by exposure time

## Combining flats

+ Choose sigma clipping, upper and lower bounds of 5.
+ Combine using mean/average first, BUT if there are stars in the combined darks then use median instead.
+ Scale before combining
    - by median
+ Group by filter

## Reducing science (light) images

+ Trim
+ Subtract bias
+ Subtract dark
    - Scale by exposure time
+ Flat correct
