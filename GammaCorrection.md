# Gamma Correction of lab monitors

Two monitors (Need specs) were used. 

A (Dimentions) patch was displayed in the center of each monitor and was used to take luminance recordings. 
16 luminance levels of the patch were recorded with RGB values starting at -1 and increased to 1 in steps of 0.125.
Luminance output of the monitors were quite comparable at each level, only differing by ~10 cd/m<sup>2</sup>.
The min and max values were 0.78 cd/m<sup>2</sup> and 186.4 cd/m<sup>2</sup> for the left monitor and 0.93 cd/m<sup>2</sup> and 197.4 cd/m<sup>2</sup> for the right monitor.
The patches were presented on a mean grey background with random dot noise around the patch (Size,rate of movemnet etc)

Both monitors were gamma corrected manually using a (luminance meter name) and then validated againt a PR655 luminance meter running automatically.
The manual readings were



The gamma from this was reasonably comparable for the left monitor (2.3853 cd/m2) but the right monitor gave a completely different reading which did not look right at all (4.7618 cd/m2). I ran it 3 times, but it was quite inconsistent. It seemed to take far longer to run than the left monitor so maybe it was having issues taking recordings that said, I didn't change anything between recording each monitor so I'm not sure why it would? I’ve kept my manual recording as it is in a more reasonable range when compared to the gamma calibration previously on the monitor (1.666 cd/m2).

## Notes from obsidian

Calibrated both manually and automatically (w/ the 655)

Automatic calibration-
Left monitor gamma = 2.3853
Right monitor gamma = 4.7618 (?????)


Manual calibration-
Recorded 16 equally spaced luminance values from 1-255 (skipped 0 as Paul recommended avoiding extreme values)

Left monitor gamma = 2.05741


![[Pasted image 20250313163806.png]]
![[Pasted image 20250313163825.png]]
![[Pasted image 20250313164248.png]]



Right monitor gamma = 1.83718
![[Pasted image 20250313164140.png]]
![[Pasted image 20250313164153.png]]
![[Pasted image 20250313164219.png]]


Left monitor raw recordings=
0.78,1.24,3.14,6.53,12.05,19.41,28.21,39.7,50.37,64.59,80.49,98.74,117.7,140.2,162.5,186.4

Right monitor raw recordings=
0.93,1.72,4.46,9.17,16.01,24.77,35.33,48.60,60.66,76.41,94.67,112.8,132.7,155.0,177.2,197.4
