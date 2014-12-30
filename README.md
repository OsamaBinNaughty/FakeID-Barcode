FakeID-Barcode
==============

Generator for fake ID barcodes. (Currently SC only, looking to expand).

About
=====

A United States Drivers License uses more than just the human readable face of the card. The 2D barcode is a PDF417 barcode.

Troubleshooting
===============

I have found the byte that makes the ID 100% readable and valid on all readers, and it looks like: ``````

Looks invisable, huh? Well, it's just not a valid ASCII character. In Notepad++, it looks like ```[FS]```.

IF IT IS NOT THERE, THE BARCODE WILL BE INVALID IN HARDWARE READERS. If you want to see it, open it in Notepad++. GitHub/your browser does not support this byte, so I am just trying to tell you that if you run into any issues reading the barcode, it may be missing.

Disclaimer
==========

This is just experimentation of the PDF417 format and validating state IDs under a controlled and undistributed environment. Please do not use for the making of false identification. I am not responsible for legal action taken against you (the user).
