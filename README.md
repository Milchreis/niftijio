niftijio
========

[![Release](https://jitpack.io/v/Milchreis/niftijio.svg)](https://jitpack.io/#Milchreis/niftijio)

This project is a Java library for reading and writing NIfTI image volumes.
This includes support for header metadata, various datatypes, and multichannel
volumes.  When a volume is read from a file, the image intensities are stored
in a four-dimensional double array.  The array indices match the order in the
'dim' array of the header.

A jar can be built using Maven by executing 'mvn package'.

The file format specification can be found here:

http://nifti.nimh.nih.gov/nifti-1

The code for reading the header was derived from the following implementation:

http://niftilib.sourceforge.net

The code for little-endian streams is provided by Roedy Green:

http://mindprod.com/jgloss/endian.html

This is released under the MIT license.  Any comments can be directed to Ryan
Cabeen at cabeen@gmail.com

## Include to project
### Maven
If you want to use `niftijio` than add the following to your pom.xml.
```xml
<repository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
</repository>
```
```xml
<dependency>
    <groupId>com.github.milchreis</groupId>
    <artifactId>niftijio</artifactId>
    <version>1.0.0</version>
</dependency>
```
