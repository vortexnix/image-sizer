## Introduction

sizer_image.py code resizes the images as per user input and and organizes them in separate folders. Features include: 
- User can add as many category folders as needed (minimum 1 folder at least)
- The script will automatically create the desired folders namely images1x, images2x etc if they don't exist. 
- Script also displays new and original dimensions

## Dependencies

Code is written in python3. The only dependency is external imaging library pillow

## Installation on MacOS

1. Install python3 and pillow:
	
	$ brew update
	
	$ brew install python3
	
	$ brew install libtiff libjpeg webp little-cms2
	
	$ pip3 install pillow

## Usage
- To specify custom configuration, make changes to class initial_config:
	- "self.sdir" contains location where images for processing are stored
	- "self.extension": png and jpg extensions are supported
	- "self.cdir":
		- User can add as many category folders as needed (minimum 1 folder at least)
		- category folder should be named precisely as images*x/ in the initial_config class
		- Corresponding dpi are specified in front of category folder name

- Desired width will be prompted when code is running.

- Lets say "images" folder contains images to be analyzed. Place the code file in the same directory that contains "images" folder 

- Run the script from terminal:
	$ python3 sizer_image.py

## Contributors

Developed by Beautifulbird, March 2017.

## License

The source files are available under open-source MIT license. Please give proper credt to the contributors.
