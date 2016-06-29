# Awesome Light Fields [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome light field resources.

## Introductory material
* [Light Fields and Computational Imaging](https://graphics.stanford.edu/papers/lfphoto/levoy-lfphoto-ieee06.pdf) - Marc Levoy


## Foundations
* [Light Field Rendering](https://graphics.stanford.edu/papers/light/light-lores-corrected.pdf) - Marc Levoy, Pat Hanrahan.
* [The Lumigraph](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/Gortler-SG96.pdf) - Steven J. Gortler, Radek Grzeszczuk, Richard Szeliski, Michael F. Cohen.
* [The Plenoptic Function and the Elements of Early Vision](https://people.eecs.berkeley.edu/~efros/courses/AP06/Papers/adelson-elements-91.pdf) - Edward H. Adelson, James R. Bergen. 


## Acquisition

### Live Scenes

#### Moving Camera
* [Standford Spherical Gantry](https://graphics.stanford.edu/projects/gantry/) - Used in the Digital Michelangelo project.
* [OTOY's Motorized Pan/Tilt Head and Offset Camera](https://www.youtube.com/watch?v=pyJUg-ja0cg) - Captures a spherical light field.

#### Array of Cameras
* [High Performance Imaging Using Arrays Of Inexpensive Cameras](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.363.5542&rep=rep1&type=pdf) - Bennett Wilburn. Describes the 100-camera reconfigurable array built at Stanford. 
* [The Panoptic Camera](http://lsm.epfl.ch/page-52820-en.html) - Hemispherical array from EPFL.
* [Design and Implementation of Multi-camera Systems Distributed over a Spherical Geometry](http://lsm.epfl.ch/files/content/sites/lsm/files/shared/Research%20Posters/diagrams2012_poster.pdf) - Summary poster of the EPFL hemispherical array.

#### Array of Lenses
* [Light Field Photography with a Hand-held Plenoptic Camera](https://classes.soe.ucsc.edu/cmps290b/Fall05/readings/lfcamera-150dpi.pdf) - Ren Ng, Marc Levoy, Mathieux Brédif, Gene Duval, Mark Horowitz, Pat Hanrahan.
* [The Standard Plenoptic Camera](http://www.plenoptic.info/) - Theoretical background on plenoptic cameras. 
* [Lytro](https://www.lytro.com/) - A manufacturer of plenoptic cameras.
* [Raytrix](https://www.raytrix.de/) - A manufacturer of plenoptic cameras focused on industrial applications.  


### Synthetic Scenes
* - 

## Parameterization

### Two-Plane
* Please refer to the [seminal papers](##fountations) for the classic two-plane parameterization.

### Spherical
* [Uniformly Sampled Light Fields](https://s3.amazonaws.com/academia.edu.documents/40263545/Uniformly_Sampled_Light_Fields20151122-28611-18fit5e.pdf?AWSAccessKeyId=AKIAJ56TQJRTWSMTNPEA&Expires=1466986432&Signature=BNSQFvjmX7iwT%2F1REsjSu%2BO0aF0%3D&response-content-disposition=inline%3B%20filename%3DUniformly_Sampled_Light_Fields.pdf) - Emilio Camahort, Apostolos Lerios, Don Fussell. This paper introduces the Two-Sphere Parameterization (2SP), the Sphere-Plane Parameterization (SPP) and associated data structures for storage and retrieval.
* [Rendering of Spherical Light Field](https://www.semanticscholar.org/paper/Rendering-of-spherical-light-fields-Ihm-Park/d93b91a371befc20a073a4971d07053e26e52c27/pdf) - Insung Ihm, Sanghoon Park, Rae Kyoung Lee. This paper introduces the Sphere-Sphere Parameterization: one positional sphere and many small directional spheres.

### Unstructured
* [Unstructured Lumigraph Rendering](https://dash.harvard.edu/bitstream/handle/1/2641679/Gortler_UnstructuredLumigraph.pdf) - Chris Buehler, Michael Bosse Leonard McMillan, Steven Gortler, Michael Cohen. This paper presents the basic challenges of unstructured light field rendering and describes a strategy for real time rendering.
* [Unstructured Light Fields](https://people.csail.mit.edu/abedavis/ULF/DavisEG2012.pdf) - Abe Davis, Marc Levoy, Fredo Durand. This paper presents an approach to capturing a light field using a hand-held video camera, estimating camera poses using fiducial markers or scene features.   

### Using geometry or depth
* [Fast (Spherical) Light Field Rendering & Per-Pixel Depth](http://www.cg.informatik.uni-siegen.de/data/www.cg.informatik.uni-siegen.de/data/Publications/2007/tr1107_LightField.pdf) - Severin Todt, Christof Rezk-Salama, Andreas Kolb. This paper describes per-pixel depth correction of rays.
* [Surface Camera Light Field Rendering](http://www.csbio.unc.edu/mcmillan/pubs/IJIG04_Yu.pdf) - Jingyi Yu, Leonard McMillan, Steven Gortler.  

### Sampling
* [Plenoptic Sampling](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.387.2222&rep=rep1&type=pdf) - Jin-Xiang Chai, Xin Tong Shing-Chow Chan, Heung-Yeung Shum.
* [On the Number of Samples Needed in Light Field Rendering With Constant-depth Assumption](http://www.cis.pku.edu.cn/faculty/vision/zlin/Publications/2000-CVPR-Light_Field_Sampling.pdf) - Whouchen Lin, Heung-Yeung Shum.
* [Spatio-Angular Resolution Tradeoff in Integral Photography](http://www.tgeorgiev.net/Spatioangular.pdf) - Todor Georgeiv, Ke Colin Zheng, Brian Curless, David Salesin, Shree Nayar, Chintan Intwala.



## Storage
### Data structures
* [Rendering Gigaray Light Fields](http://www.jku.at/cg/content/e152197/e189819/RGRLF.pdf) - C. Birklbauer, S. Opelt, O. Bimber. Presents a caching framework. 

### Compression
* [Data Compression for Light-Field Rendering](https://trac.csse.rose-hulman.edu/LIDCOM/export/41/GeneralResources/DataCompressionLFR.pdf)


## Rendering
* [Dynamically reparameterized light fields](http://www.cs.harvard.edu/~sjg/papers/drlf.pdf) - Aaron Isaksen, Leonard McMillan, Steven J. Gortler. This paper uses a planar proxy geometry to refocus the rays, and describes a related rendering algorithm to accelerate the synthesis of new views. 
* 1997 - Gortler - Time Critical Lumigraph Rendering


## Displays
### Light Field Displays
### VR Headsets

## Modification
* Lightshop - Interactive Light Field Manipulation and Rendering
* How Do People Edit Light Fields?

