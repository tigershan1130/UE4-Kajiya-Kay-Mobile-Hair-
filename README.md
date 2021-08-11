# UE4-Kajiya-Kay-Mobile-Hair-
Based on Kajiya-Kay Implementing ATI based into Mobile Pipeline in UE4

![alt text](https://github.com/tigershan1130/UE4-Kajiya-Kay-Mobile-Hair-/blob/main/Screenshots/Windows/HighresScreenshot00000.png)
![alt text](https://github.com/tigershan1130/UE4-Kajiya-Kay-Mobile-Hair-/blob/main/Screenshots/Windows/HighresScreenshot00001.png)

Left uses regular BRDF shading
Right uses kayjiya-kay implementation of the hair cards.

Note:
- This rendering requires custom rendering pipeline instead of feeding highlight into diffuse(which makes it look totally wrong). 
The highlight would look more realistic with the surroundings using this custom kayjiya-kay implementation of the hair with skylight, etc.
- This project need to enable mobile support for Opengl ES3.1 and uses custom modification on UE4 4.26.2, which you can find here:
https://github.com/tigershan1130/UnrealEngine-1/commit/11cdd35a9c3d73900d3ea71f018175a0e223e2dd


TODO:
- Add approximation for diffuse transmission
- Add second offset mesh based for transparency smoothing edges.

Reference:

http://developer.amd.com/wordpress/media/2012/10/Scheuermann_HairSketchSlides.pdf
https://web.engr.oregonstate.edu/~mjb/cs519/Projects/Papers/HairRendering.pdf
