# PIcFrame

Hobby project to create a simple Photo Frame using a Raspberry Pi.

Uses the pi3d (http://pi3d.github.io/) project and is heavily based on the PictureFrame app from https://github.com/pi3d/pi3d_demos. The goal is to create a lightweight and easy to install Picture Frame package for a Raspberry Pi.


Installation instructions:

Install Raspberry Pi OS with Desktop. You probably want to disable screensaver and enable SSH. Maybe also boot to CLI.

If you have a Raspberry Pi 4 copy and paste this in the Terminal:

sudo raspi-config nonint do_boot_behaviour B2 && sudo raspi-config nonint do_memory_split 256 && sudo raspi-config

In the raspi-config module, go to 7 Advanced Options > A8 GL Driver > Choose G2 GL Fake KMS.

For the Raspberry Pi 2 and 3:

sudo raspi-config nonint do_boot_behaviour B4 && sudo raspi-config nonint do_memory_split 128 && sudo raspi-config 

In the raspi-config module, go to 7 Advanced Options > A8 GL Driver > Choose G1 (Legacy)

After that it is time to install pi3d:
sudo pip3 install pi3d

Download PIcFrame, unzip and run with supplied script.

Options available and con figurable in PIcFrame_config.py.



