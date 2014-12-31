PhotoCollage
============

*Graphical tool to make photo collage posters*

PhotoCollage allows you to create photo collage posters.  It assembles the
input photographs you give it to generate a big poster.  Photos are arranged
to fill the whole poster, however you can influence the algorithm to change the
final layout.  You can also set a custom border between photos, and save the
generated image in the resolution you want.

The algorithm generates random layouts that place photos while taking advantage
of all free space.  It tries to fill all space while keeping each photo as
large as possible.

PhotoCollage does more or less the same as many commercial websites do, but
for free and with open-source code.

![screenshot](https://github.com/adrienverge/PhotoCollage/raw/v1.2.0/screenshots/photocollage-1.2-preview.png)

It provides a library to create photo layouts and posters, and a GTK graphical
user interface.  PhotoCollage is written in Python (compatible with versions 2
and 3) and requires the Python Imaging Library (PIL).

Features:
* generate random new layouts until one suits the user
* choose border color and width
* save high-resolution image
* works even with a large number of photos (> 100)
* integrates into the GNOME environment
* available in English and French

Installation
------------

* Fedora:
  ```
  sudo yum install photocollage
  ```

* Ubuntu:
  ```
  sudo add-apt-repository ppa:dhor/myway && sudo apt-get update
  sudo apt-get install photocollage
  ```

* Manual installation (for other OS):
  ```
  # Install dependencies
  sudo yum install python3-pillow python3-gobject
  sudo apt-get install python3-pil python3-gi
  sudo pacman -S python-pillow python-gobject
  # Install PhotoCollage
  git clone https://github.com/adrienverge/PhotoCollage.git
  cd PhotoCollage
  sudo python3 setup.py install
  ```

Usage
-----

After install a launcher for PhotoCollage will appear in your desktop menu.

If it doesn't, just run:
```
./photocollage
```
