## About

ILLIXR is an open-source Extended Reality (XR) benchmark suite. It contains several core state-of-the-art components of the generic XR pipeline, components that are required in most, if not all, XR applications. ILLIXR is **not** an XR runtime, nor is it meant to be the world's most optimized piece of XR software. Instead, the goal of ILLIXR is to advance systems and computer architecture research for XR by incorporating key state-of-the-art components of both modern and future XR applications. You can think of ILLIXR as an XR benchmark suite by computer architects for computer architects.

We use the term _components_ and not _kernels_ or _computations_ because each component of ILLIXR is an entire application in itself, and consists of many, many kernels and computations. At the moment, ILLIXR contains the following state-of-the-art components.

1. [Simultaneous Localization and Mapping](https://github.com/ILLIXR/open_vins)
2. [Scene reconstruction](https://github.com/ILLIXR/ElasticFusion)
3. [Ambisonic encoding](https://github.com/ILLIXR/audio_pipeline)
4. [Ambisonic manipulation and binauralization](https://github.com/ILLIXR/audio_pipeline)
5. [Lens distortion correction](https://github.com/ILLIXR)
6. [Chromatic aberration correction](https://github.com/ILLIXR)
7. [Time warp](https://github.com/ILLIXR)
8. [Computational holography for adaptive multi-focal displays](https://github.com/ILLIXR/HOTlab)

Many of these components were developed by domain experts and obtained from publicly available repositories. They were modified for one or more of the following reasons: fixing compilation, adding features, or removing extraneous code or dependencies. Each component not developed by us is available as a fork for proper attribution to its authors. Detailed descriptions of each component can be found in our paper (listed below under `Publications`).

We plan on adding more components to ILLIXR in the future, including graphics.


## Publications

We ask that you cite our following paper when you use ILLIXR for a publication. We would also really appreciate it if you send us a citation once your work has been published.

- Muhammad Huzaifa, Rishi Desai, Xutao Jiang, Joseph Ravichandran, Finn Sinclair, Sarita V. Adve, [Exploring Extended Reality with XRBench: A New Playground for Architecture Research]().


## Setup

There is no centralized setup for ILLIXR. Each component of ILLIXR is packaged as its own repository for modularity. Please refer to the setup instructions of each individual component listed on the [ILLIXR github](https://github.com/ILLIXR).

## Acknowledgements

ILLIXR was developed by several members of the [RSIM research group](http://rsim.cs.illinois.edu/) at the University of Illinois at Urbana-Champaign, including Sarita V. Adve, Rishi Desai, Muhammad Huzaifa, Xutao Jiang, Joseph Ravichandran, and Finn Sinclair.

ILLIXR would not have been possible without invaluable help from Steve LaValle, Matt Horsnell, Liang Gao, Andrew Maimone, Amit Jindal, Aleksandra Faust, Eric Shaffer, Steve Lovegrove, Wei Cu, Archontis Politis, Martin Persson, and Vegard &#216;ye. The development of ILLIXR was supported by the Applications Driving Architectures (ADA) Research Center, a JUMP Center co-sponsored by SRC and DARPA. The development of ILLIXR was also aided by generous hardware and software donations from ARM and NVIDIA.


## Licensing Structure

ILLIXR is available as open-source software under the [University of Illinois/NCSA Open Source License](https://github.com/ILLIXR/illixr.github.io/blob/master/LICENSE). As mentioned above, ILLIXR largely consists of components developed by domain experts and modified for the purposes of inclusion in ILLIXR (remember, we are computer architects, not algorithm developers!). However, ILLIXR does contain software developed solely by us. **The NCSA license is limited to only this software**. The external libraries and softwares included in ILLIXR each have their own licenses and must be used according to those licenses:

- [Open-VINS](https://github.com/rpng/open_vins) - [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)
- [ElasticFusion](https://github.com/mp3guy/ElasticFusion) - [ElasticFusion license](https://github.com/mp3guy/ElasticFusion/blob/master/LICENSE.txt)
- [libspatialaudio](https://github.com/videolabs/libspatialaudio) - [GNU Lesser General Public License v2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
- [HOTlab](https://github.com/MartinPersson/HOTlab) - [GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.html)


## Get In Touch

Whether you are a computer architect, a systems person, an XR application developer, or just anyone interested in XR, we would love to hear your feedback on ILLIXR! ILLIXR is a living benchmark suite and we would like to both refine existing components and add new ones. We believe ILLIXR really has the opportunity to drive future computer architecture and systems research for XR, and can benefit from contributions from other researchers and organizations. If you would like to be a part of this effort, please contact us at illixr at illinois dot edu
