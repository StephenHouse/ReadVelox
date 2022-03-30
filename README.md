# ReadVelox

A MATLAB function for importing ThermoFisher Scientific's Velox .emd image and diffraction files into MATLAB, because the built-in HDF5 functions don't play nicely with Velox files.

Version 01.01

## Installation
Place into whatever directory you are using to hold your MATLAB scripts/programs.

## Input
The input is the filename of the .emd file.
The output is a structure with the following fields:
- OutputData.RawImage    <-- The image intensities
- OutputData.RawMetadata <-- The raw metadata string
- OutputData.ImageMode   <-- 'TEM','STEM', or 'DP'
- OutputData.ImageWidth  <-- Width of the image, in pixels
- OutputData.ImageHeight <-- Height of the image, in pixels
- OutputData.PixelScale  <-- Pixel size, in PixelUnits
- OutputData.PixelUnit   <-- The units of PixelScale

## Roadmap
It currently does not read in spectrum, spectral image, or multi-image series files. Only TEM and STEM images and diffraction files. I'll update this as this functionality is added, or do let me know if you've improved and/or expanded it on your own. I'd be thrilled.

## Boring legal text
Copyright (c) 2019, Stephen D. House
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
- Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
- Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
