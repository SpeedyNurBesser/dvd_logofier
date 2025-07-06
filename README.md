#  Logofier

Simulate the DVD bounce using any image (or series of images) with any window size. Customize initial speed, vector, and position. 

## Usage

The most basic command structure is the following:

```dvd_logofier <IMAGE_FILENAME>```

Note, that dvd_logofier searches for the image in the terminal location. So, cd into the directory your image is stored in.

This will result in a 720 x 480 window appearing, where the given image bounces arround with the default speed of 1 px/frame @ 60 frames per second.

<a href="https://imgur.com/yTtNrbP.png">
  <img src="https://imgur.com/yTtNrbP.png" />
</a>

Multiple images can be specified, like so:

`dvd_logofier img1.png img2.png img3.png img4.png`

This will lead to the next image in the given order being selected any time a wall is hit.



Further options, like window size, initial position and vector, velocity, and background color, can be changed using optional parameters. Here, are some examples:

`dvd_logofier test.png --screen-width 1920 --screen-width 1080`

`dvd_logofier test.png --background-color '#ffffff'`

`dvd_logofier test.png --velocity 10`


To see an extensive list of all options, type `dvd_logofier --help`

## Installation

```pip install dvd-logofier```

In theory, this should install all dependencies. If it does not, also install `typer` and `pygame`:

```pip install pygame```

```pip install typer```
