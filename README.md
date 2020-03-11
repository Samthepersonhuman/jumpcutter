# jumpcutter UPDATED
Automatically edits videos. Explanation here: https://www.youtube.com/watch?v=DQ8orIurGxw
This is forked from CaryKH's Jumpcutter.
## Some heads-up:

It uses Python 3.

It works on Ubuntu 16.04 and Windows 10. (It might work on other OSs too, we just haven't tested it yet.)

This program relies HEAVILY on ffmpeg. It will start subprocesses that call ffmpeg, so be aware of that!

As the program runs, it saves every frame of the video as an image file in a
temporary folder. If your video is long, this could take a LOT of space.
Cary has processed 17-minute videos completely fine, but be wary if you're gonna go longer.

Cary wants to use pyinstaller to turn this into an executable, so non-techy people
can use it EVEN IF they don't have Python and all those libraries. Jabrils 
recommended this to him. However, His pyinstaller build did not work. :( I will attempt to do that for him.

## Building with nix!
`nix-build` to get a script with all the libraries and ffmpeg, `nix-build -A bundle` to get a single binary.
