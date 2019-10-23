Vampyre Imaging Library
===================================

<img style="float: right" src="https://raw.githubusercontent.com/galfar/imaginglib/master/Doc/Common/logo.png">

Object Pascal image loading, saving, and manipulation library.

<https://github.com/galfar/imaginglib>  
<https://bitbucket.org/galfar/imaginglib>  

Homepage: <http://imaginglib.sf.net>  
Forum: <https://galfar.vevb.net/imaging/smf>

Overview
--------------------------

In the beginning, the goal of the library was to provide cross-platform native Object Pascal support for loading images in various file formats, do some basic operations like resizing and pixel format conversions, and save back - and all this without needing external dependencies both build time and run time.

Later, more features were added on top for convenience but the following still applies:

- core library depends only on Delphi/FPC RTL (common subset nowadays)
- keep the image in the original pixel format (for all operations or as long as possible)
- if a feature needs some external library or platform specific stuff it's an optional extension
- drawing and painting is not a main use of the library -> there are better and faster options for this

Features
--------------------------

Loading and saving of these image file formats:

- PNG/APNG, MNG, JNG
- JPEG
- GIF
- DDS
- TGA, BMP
- HDR, PCX, XPM, PNM
- TIFF, JPEG2000 (not native Pascal, depends on platform)
- and more

Supported platforms are:

- Delphi: Windows, macOS
- FPC: Windows, Linux x86/ARMv7, Android, macOS

Many internal image data formats and conversions:

- 8, 16, 24, 32, 48 and 64 bit RGB and ARGB formats
- indexed formats
- grayscale formats
- floating point formats (IEEE754 and half precision)
- compressed formats like DXT1/3/5, 3Dc, and BTC

Basic image manipulation functions working for all supported data formats and conversions between them (bilinear/bicubic resizing, rotation by any angle, color reduction, mipmap generation, ...).

Image drawing with blending, linear and nonlinear filters, point transforms, binary morphology, drawing lines, ellipses, rectangles, etc.

Low level library interface (accessible by other programming languages) and high level OOP one.

Extensions for creating OpenGL, Direct3D, and SDL textures/surfaces.

VCL, LCL, and FMX graphic classes and functions.

Support multi-images, direct access to image data,
user-specified file formats, overriding default read and write functions,
and more.

License & Credits
------------------

Imaging comes with two open source licenses from which you can choose the one which fits your needs best:

- MPL - Mozilla Public License
- LGPL - GNU Lesser General Public License

 Developed by Marek Mauder.

Status
-----------

Imaging started almost 20 years ago and since 2009 it is more or less in maintenance mode without big new features being added.
Anyway, it is still alive, updated to work with current compilers and platforms, and here and there a new feature gets in. Documentation can be pretty outdated though.
