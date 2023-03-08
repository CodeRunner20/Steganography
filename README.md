# Steganography
This Project Describes the use of LSB Steganography.

Installation

Use the package manager 

pip to install 'opencv,pillow and numpy'


pip install opencv-python
pip install pillow
pip install numpy

usage

step-1. clonning--> git clone repo. or download zip file

step-2. run 'python imgstegno.py'

step-3. give respective inputes and get outputs

STEGANOGRAPHY comes from the Greek Words: STEGANOS – “Covered”, GRAPHIE – “Writing”. The sender hides his/her message within an image/audio/video.Since the algorithm uses the lease significant bit to hide the secret message the change is undectable by a naked eye.
The various types of steganography include:


Image Steganography

Audio Steganography

Video Steganography

Text files Steganography


Types of Images:

Black and white

Geryscale

RGB

In a gray scale image each pixel is represented in 8 bits. The last bit in a pixel is called as Least Significant bit as its value will affect the pixel value only by “1”. So, this property is used to hide the data in the image. If anyone have considered last two bits as LSB bits as they will affect the pixel value only by “3”

The LSB embedding approach has become the basis of many techniques that hide messages within multimedia carrier data. LSB embedding may even be applied in particular data domains – for example, embedding a hidden message into the color values of RGB bitmap data

Let's study the application of LSB on a Greyscale Image
In a Greyscale image, each pixel is represented by 8 bits, while in a RGB it is 24 bits

Suppose the following are some of the bits in a Grayscale image


11110011

11011011

10110110

11011100

11011111

11010111

00100110

01000011

You wish to hide "A" in it. The ascii value of "A" is 10000001.
The algorithm simply replaces the last bit of the bytes with the consecutive bits of the letter "A", Giving us


11110011

11011010

10110110

11011100

11011110

11010110

00100110

01000011


Steganalysis
Steganalysis is the study of detecting messages hidden using steganography

LSB Steganography can be detected by looking at the histograms of the files

Also lossy compression technique can render LSB Steganography useless to an extent, so lossless compression techniques should be used


