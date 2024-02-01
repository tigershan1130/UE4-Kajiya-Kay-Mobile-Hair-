# UE4-Kajiya-Kay-Mobile-Hair-
Based on Kajiya-Kay Implementing ATI based into Mobile Pipeline in UE4

![image](https://github.com/tigershan1130/UE4-Kajiya-Kay-Mobile-Hair-/assets/39791762/385caebc-2190-4308-82ed-f56607d1b5e1)

Left uses regular BRDF shading
Right uses kayjiya-kay implementation of the hair cards.

Note:
- This rendering requires custom rendering pipeline instead of feeding highlight into diffuse(which makes it look totally wrong). 
The highlight would look more realistic with the surroundings using this custom kayjiya-kay implementation of the hair with skylight, etc.
- This project need to enable mobile support for Opengl ES3.1 and uses custom modification on UE4 4.26.2, which you can find here:
https://github.com/tigershan1130/UnrealEngine-1/commit/f50307f95b2a4cbfb6a675dcc3bbf393f0b0ffdf


TODO:
- Add approximation for diffuse transmission
- Add second offset mesh based for transparency smoothing edges.

Reference:

http://developer.amd.com/wordpress/media/2012/10/Scheuermann_HairSketchSlides.pdf
https://web.engr.oregonstate.edu/~mjb/cs519/Projects/Papers/HairRendering.pdf
