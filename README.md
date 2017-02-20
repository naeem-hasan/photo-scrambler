# photo-scrambler
A photo scrambler that can jumble up photos according to user input horizontal and vertical chunks!

## Requirements:
* [Python 2](https://www.python.org/downloads/release/python-2713/). You probably already have it installed in your machine.
* [Pillow](https://python-pillow.org/). Install it by: `sudo pip install Pillow`.

## Usage:
So you have the necessary requirements?! :relaxed:

You scramble a photo using this command: `photo-scramble filename.jpg`. A scrambled image file will be generated in the current directory.
But you can specify the horizontal AND/OR vertical cuts. If only horizontal number of cuts is defined, the vertical cut number is calculated automatically so that each chunk becomes closest to a square. See the examples.

### Example usage:
* `photo-scramble myphoto.png`
* `photo-scramble myphoto.jpg 5`
* `photo-scramble photo.jpg 3 6`

### Note:
The script breaks the photo into chunks, loads them in the memory and then places them randomly. Hence, it can be slow and memory consuming when dealing with large images or large number of cuts.
