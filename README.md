


#  Orrery for macOS
## Overview
This project provides a reasonably accurate model of the 8 major planets in the solar system. The orbital mechanics for each planet were calculated based on publicly available orbital elements and the current date. A simple hud panel is provided with a slider that increases or reverses the render date, providing a rudimentary animation of the planetary orbits. 

## Usage
Scene kit provides a navigation framework for its 3d scenes. The following are the navigation methods using a trackpad:
* Two Fingers pans the XY axis
* Pinch zooms in and out
* Click pan rotates 3d model

## Installation
### General Setup
1. Clone or Download the project from github.
2. Open the Orrery.xcodeproj file.
3. Click the Orrery project file in xcode.
4. On the General tab under Signing, add your team signing credentials. (This requires an apple developer ID)
### Run from the command line
1. Follow the general setup
2. Open Terminal and navigate to the top level Orrery directory
3. Enter the command: make run
### Run from Xcode
1. Follow the general setup
2. Click build and run on the top left of xcode (or Command R).

## Requirements
* macOS 10.12 or later
* xcode 9.2 or later

## Notes & Caveats
This project has been written in a mixture of Swift, Objective C and C. The class OrbitalPositions was written in objective c because Swift still has a difficult time with simple math operations. This is still a work in progress and has not been fully tested. Specifically, Unit Tests are only included for the cartisianPositionForPlanet: method on OrbitalPositions and the scene kit render loop could be optimized further.

## Acknowledgements
* Orbital mechanics calculations and elements provided by: http://www.stjarnhimlen.se/comp/tutorial.html
* Background knowledge and a working example http://lab.la-grange.ca/en/building-jsorrery-a-javascript-webgl-solar-system
* Planet textures: http://planetpixelemporium.com/planets.html

Created by Michael Golden on 1/8/18.
Copyright © 2018 norobostudios. All rights reserved.
