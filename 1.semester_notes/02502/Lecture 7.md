The different image and video processing and analysis methods are often grouped into the categories listed below

- Image Compression

> This is probably the most well-defined categories and contain the group of methods used for compressing image and video data

- Image Manipulation

> This category covers methods used to edit an image. For ex., when rotating or scaling an image, but also when improving the quality by for ex. changing the contrast

- Image Processing

> Image processing originates form the more general field of _signal processing_ and covers methods used to _segment_ the object of interest. Segmentation here refers to methods which in some way enhance the object while suppressing the rest of the image (for example, the edges in an image)

- Image Analysis

> Here the goal is to analyze the image with the purpose of first finding and second extrating some parameters of the object in the image. For example, finding an object’s position and size

- Machine Vision

> When applying image processing or image analysis in production industries it is normally referreed to as _machine vision_ or simply _vision_

- Computer Vision

> When talking about computer vision we normally mean advanced algorithms similar to those a human can perform, e.g., face recognition. Normally computer cision also covers all methods where more than one camera is applied

General frameworks

- Image Acquisition

> Everything to do with the camera and setup of your system is covered, e.g., camera type, camera settings, optics and light sources

- Preprocessing

> This block does something to your image before the actual processing commences, e.g. convert the image from color to gray-scale or crop the most interesting part of the image

- Segmentation

> This is where the information of interest is extracted from the image. Often this block is the “heart” of a system. In the example given in the figure, the information is the fingers.

- Representation

> The objects extracted in the segmentation block are represented in a concise manner, e.g. using a few representative numbers as illustrated in the figure

- Recognition

> This block examines the information produces by the previous block and classifies each object as being an object of interest or not. In the example in given the figure, this block determines that three finger objects are present and hence output this

_BLOB analysis_ a block that’s equals to the last two blocks

_Reconstruction_ is a 3d volume image that is created by using a st of algorithms

---

Image Acquisition - Capter 2

An image must be capture by a camera and converted into a manageable entity before any image processing can commence, which is known as _image acquisition_

## Image acquisition consist of three steps:

- energy
- optical system
- sensor

---

Image processeing er når man redigerer billedet uden at lære fra det ift image analysis

seperate objects to differents segments

Image Types

- colour

RGB, often we want to convert it tho

converting colours to the grey scale

v= 0.5**R+0.5_G_+0.5*B

- binary

black or white (on or off)

- label

each label represent some kind of information

Ex. gray = background, blue = soft tissue, green = hard bone, red = spongy bone

It is often seen as a processeing step

- 16-bit

the pixel value isn’t only for displaying

0 for water

-1000 for air

-120 fat

400+ bone

- floating point

for scaling and changes of pixels

multispectral system