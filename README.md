# docker-stuffz

## Adafruit container for building ESP32 

https://www.youtube.com/watch?v=f6ZhVPpiNzM

Ladyada will be talking about using Docker for kernel compiles on ESP32S3 to overcome issues with other methods; they created a Docker container, simpler and smaller than VirtualBox. And we're discussing on adding a 2x5 0.05" JTAG/SWD connector to ESP32-S3 boards, highlighting options for easy debugging.

This week at the Desk of Ladyada we're playing around with @jcmvbkbc 's linux-for-ESP32S3 script (https://gist.github.com/jcmvbkbc/316e.... We tried compiling a few different ways: MSYS2, WSL, VirtualBox and Mac OS, but bumped into different issues each time - not major issues but still kinda annoying stuff. if we want others to be able to reproduce this we did what any REAL engineer does when they have a big toolchain to massage: make a Docker container! (https://www.hanselman.com/blog/docker...) - much simpler and smaller than virtualbox because it has only the bare essentials. no cruft to deal with from python versions or operating system setups. we'll chat about how to make a Dockerfile, how to port over a shell script, and then how to terminal in once running. the Dockerfile is herehttps://github.com/adafruit/Adafruit_... and if you want to just download the container image post-compilation check it out at https://hub.docker.com/repository/doc...

The Great Search - 2x5 0.05" JTAG / SWD connector and cable
https://www.digikey.com/short/rcmjwc81
