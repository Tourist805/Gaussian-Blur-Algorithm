# Gaussian-Blur-Algorithm
Gaussian Blur algorithm on AVX and Sobel algorithm working on C++ assembly

In image processing, a Gaussian blur (also known as Gaussian smoothing) is the result of blurring 
an image by a Gaussian function (named after mathematician and scientist Carl Friedrich Gauss).

It is a widely used effect in graphics software, typically to reduce image noise and reduce detail. 
The visual effect of this blurring technique is a smooth blur resembling that of viewing the image through a translucent screen, distinctly different from 
the bokeh effect produced by an out-of-focus lens or the shadow of an object under usual illumination.

Well, how it works, at first we neef to create Gaussian Blur mask, from which we will multiply our cell values.
const unsigned short int gaussianMask[5][5] = {
	{2,4,5,4,2} ,
	{4,9,12,9,4},
	{5,12,15,12,5},
	{4,9,12,9,4},
	{2,4,5,4,2}
};
