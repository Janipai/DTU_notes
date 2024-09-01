The different image and video processing and analysis methods are often grouped into the categories listed below

- Image Compression

> This is probably the most well-defined categories and contain the group of methods used for compressing image and video data

- Image Manipulation

> This category covers methods used to edit an image. For ex., when rotating or scaling an image, but also when improving the quality by for ex. changing the contrast

- Image Processing

> Changing the information in images – but not necessarily getting any knowledge
> 
> - Deeper explanation
>     
>     Image processing originates form the more general field of _signal processing_ and covers methods used to _segment_ the object of interest. Segmentation here refers to methods which in some way enhance the object while suppressing the rest of the image
>     
> - Example
>     
>     The edges in an image.
>     
>     - Photoshopping
>     - Changing the visual appearance of photos
>     - Cropping / rotating
>     - Filters / effects

- Image Analysis

> Automatic extraction of information from images
> 
> - Deeper explanation
>     
>     Herethe goal is to analyze the image with the purpose of first finding and second extrating some parameters of the object in the image
>     
> - Example
>     
>     Finding an object’s position and size
>     

- Machine Vision

> Combination of:

- Very fast cameras
- Fast classification algorithms
- Robotics

> - Deeper explanation
>     
>     When applying image processing or image analysis in production industries it is normally referreed to as _machine vision_ or simply _vision_
>     
> - Example
>     
>     Tomato sorting
>     

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

> RGB, often we want to convert it tho converting colours to the grey scale
> 
> v= 0.5**R+0.5_G_+0.5*B

- binary

> black or white (on or off)
> 
> - Why
>     - Separating objects from background
>     - Count the number of the objects
>     - Measure the size and shape of objects
>     - Advanced 3D visualisations

- label

> each label represent some kind of information
> 
> - Example
>     
>     gray = background, blue = soft tissue, green = hard bone, red = spongy bone
>     
> 
> It is often seen as a processeing step

- 16-bit

> the pixel value isn’t only for displaying
> 
> - 0 for water
> - -1000 for air
> - -120 fat
> - 400+ bone

- floating point

> For scaling and changes of pixels

multispectral system

- There are more visual information than what can be seen with the human eye

For processing a pixel is often transformed to a float

![[Pasted image 20240901144803.png]]

Image Resolution

- Determines how much the image fills in the memory and on the hard disk
- Spatial resolution
- Gray level resolution

Spatial

- relating to the position, area and size of things
- Example: This task is designed to test the child's spatial awareness

---

![[Pasted image 20240901144926.png]]

- F = Focal Point
- O = Optical center
- g = the distance between the object and the lens
- b = the distance from the lens to where the rays intersect

f and b is typical [1mm,100mm]

_**the thin lens equation**_

$$ 1/g+1/b=1/f $$

_**The optical zoom**_ is when the size of the object in the image, B, increases as f increased.

- G is the real height

![[Pasted image 20240901145038.png]]

$Depht Of Field = g_r+g_l$

![[Pasted image 20240901145016.png]]

aperture controlls the amount of light in the lens