# Ray Tracer

![alt text](https://github.com/konieboy/C-Ray-Tracer/blob/master/images/yours1.png)

Konrad Wisniewski 2017 

------------------------------------------------
------------------------------------------------

To compile, type:

make all

To run:

	./rayTracer --default
	The program should write an image called default.ppm in the current directory. This image should be rendition of the test scene at a resolution of 512 x 512.

	./rayTracer --yours
	The program should write an image called yours.ppm in the current directory. This image should be a rendition of your modelled scene at a resolution of 512 pixels for the shorter side.

	If no flag is given, file is saved as default.ppm
	
	RECOMMENDED USE:

	1) Create default scene, 512*512, fov of 55, Depth level of 12, 4x supersampling
		./rayTracer --default 512 512 55 12 4
		
	2) Create custom scene, 512*512, fov of 55, Depth level of 12, 4x supersampling
	
		./rayTracer --yours 512 512 55 12 4
		
------------------------------------------------
------------------------------------------------
Implemented all of the necessary features:
- Perspective Camera
- Geometric Primitives
- Local Illumination
- Recursive Ray Tracing
- Super Sampling
------------------------------------------------
------------------------------------------------

How to use all the features:

1) Custom Resolution 

	Usage: ./rayTracer --default [int]width [int]height

	ex) ./rayTracer --default 512 512

	default values are 512X512

------------------------------------------------
2) Custom FOV (Perspective Camera)

	Usage: ./rayTracer --default [int]width [int]height [int]FOV

	ex) ./rayTracer --default 512 512 55

	default value is 55
------------------------------------------------

3) Adjustable levels of SuperSampling and Depth 

Usage: ./rayTracer --default [int]width [int]height [int]FOV [int]Depth [int]SuperSampling

ex) ./rayTracer --default 512 512 55 14 4

------------------------------------------------
------------------------------------------------

Images

- yours.ppm and yours1.ppm show off triangles and spheres, reflections, super sampling, custom resolutions.

- yours2.ppm shows of custom FOV

- yoursLowQuality.ppm shows low supersampling and reflective depth
