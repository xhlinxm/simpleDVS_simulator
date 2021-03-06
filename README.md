# Simple simulator for DVS data 

This package implements a simple method for creating event-based camera data (DVS data) from images and groundtruth motion 

## Getting Started

Clone or download the project. This repository contains Matlab M-files and some sequences stored with Git LFS.
After this, you will have a copy of the project for testing.

## Running the tests

Just run
```
simulateEvents(/path/to/file, filename, factor)
```
	* `/path/to/file` is the pathname to the mat file with the inputs (see the examples in the sequences.zip)  
	* `filename` is the mat file with the inputs (see the examples in the sequences.zip): II (vector of images), O_t (2D groundtruth: x speed, y speed)
	* `factor` modulates the number of frames, or the minimum latency (check code)   

## Pre-requisites

This code was initially created to translate [Middlebury dataset](http://vision.middlebury.edu/flow/data/) for motion estimation into event raw data, in order to compare event-based and conventional frame-based methods. In order to do that, we include some of the Middlebury sequences to try our code. Since the file is too large to be included in github, we used `git-lfs`. Take a look here to install it: https://github.com/git-lfs/git-lfs/wiki/Tutorial

In order to clone, just do it in the normal way for github after installing `git-lfs`. After cloning, a file called sequences.zip will appear in your local repository. Just uncompress it and run the Matlab code with its files.

## Publications

If you use this work in an academic context, please cite the following publication:

* Barranco, Francisco, Cornelia Fermüller, and Yiannis Aloimonos. "Contour motion estimation for asynchronous event-driven cameras." Proceedings of the IEEE 102, no. 10 (2014): 1537-1556. ([PDF](https://ieeexplore.ieee.org/abstract/document/6895239))

## Authors

* **Francisco Barranco** - *University of Granada*
Please report problems, bugs, or suggestions to fbarranco_at_ugr_dot_es (Replace _at_ by @ and _dot_ by .).

## Acknowledgments

* This work was supported by the European Union (EU) under the grant Poeticon++ in the Cognitive Systems program, and by the National Science Foundation under an INSPIRE grant in the Science of Learning Activities program. The work of F. Barranco was supported by an EU Marie Curie fellowship (FP7-PEOPLE-2012-IOF-33208), and the CEI-GENIL Granada (PYR-2014-4).

## License

Copyright (C) 2018 Francisco Barranco, 28/01/2019, University of Granada.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details. 

You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.


