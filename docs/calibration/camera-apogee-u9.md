# Camera parameters

+ Name: `Apogee Alta U9`
+ Gain: `1.5 electron/ADU`
+ read noise: `30` electrons
+ dark current: `0.1 electron/pixel/sec`
+ linearity limit: `35000 ADU`
+ Pixel size: 9 micron
+ Number of pixels: 2048 x 3073
+ Filters: `BVRcIc`

## Reduction settings

### All images

+ Do not use the overscan
+ Trim to all of first axis, 3073 on second axis

### Reducing bias images

+ Only need to trim

### Combining bias

+ Choose sigma clipping, upper and lower bounds of 5.
+ Combine using mean/average

### Reducing darks

IF THE DARK EXPOSURE TIME DOESN'T MATCH ANY OF THE OTHER IMAGES:

+ Trim
+ Subtract bias

IF THERE ARE DARK EXPOSURES THAT MATCH EVERY EXPOSURE IN THE SET:

+ Trim, but do NOT subtract bias

### Combining darks

+ Choose sigma clipping, upper and lower bounds of 5.
+ Combine using mean/average
+ Group by exposure time

## Reducing flats

+ Trim
+ Subtract bias (maybe)
+ Subtract dark
    - Do not Scale by exposure time

## Combining flats

+ Choose sigma clipping, upper and lower bounds of 5.
+ Combine using mean/average first, BUT if there are stars in the combined darks then use median instead.
+ Scale before combining
    - by median
+ Group by filter

## Reducing science (light) images

+ Trim
+ Subtract bias (maybe)
+ Subtract dark
    - Do not Scale by exposure time
+ Flat correct
