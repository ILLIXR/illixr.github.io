---
layout: front
---

<a href="https://youtu.be/GVcCW8WgEDY"><img alt="ILLIXR Simple Demo" src="https://img.youtube.com/vi/GVcCW8WgEDY/0.jpg" style="width: 320px" class="center"></a>

Illinois Extended Reality testbed or ILLIXR (pronounced like elixir) is the first fully open-source Extended Reality (XR) system and testbed. The modular, extensible, and [OpenXR](https://www.khronos.org/openxr)-compatible ILLIXR runtime integrates state-of-the-art XR components into a complete XR system. The testbed is part of the broader [ILLIXR consortium](http://illixr.org), an industry-supported community effort to democratize XR systems research, development, and benchmarking.

You can find the complete ILLIXR system [here](https://github.com/ILLIXR/ILLIXR).

ILLIXR also provides its components in standalone configurations to enable architects and system designers to research each component in isolation. The standalone components are packaged together in the [v1-latest release](https://github.com/ILLIXR/ILLIXR/releases/tag/v1-latest) of ILLIXR. 

ILLIXR's modular and extensible runtime allows adding new components and swapping different implementations of a given component. ILLIXR currently contains the following components: 

1. Visual Inertial Odometry: [OpenVINS](https://github.com/ILLIXR/open_vins), [Kimera-VIO](https://github.com/ILLIXR/Kimera-VIO)
2. Scene reconstruction: [ElasticFusion](https://github.com/ILLIXR/ElasticFusion), [KinectFusion](https://github.com/ILLIXR/KinectFusionApp/tree/illixr-integration)
3. [Eye tracking](https://github.com/ILLIXR/RITnet)
4. [Ambisonic encoding](https://github.com/ILLIXR/audio_pipeline)
5. [Ambisonic manipulation and binauralization](https://github.com/ILLIXR/audio_pipeline)
6. [Lens distortion correction](https://github.com/ILLIXR/visual_postprocessing)
7. [Chromatic aberration correction](https://github.com/ILLIXR/visual_postprocessing)
8. [Asynchronous reprojection (Time warp)](https://github.com/ILLIXR/visual_postprocessing)
9. [Computational holography for adaptive multi-focal displays](https://github.com/ILLIXR/HOTlab)

We continue to add more components (new components and new implementations). 

Many of the current components of ILLIXR were developed by domain experts and obtained from publicly available repositories. They were modified for one or more of the following reasons: fixing compilation, adding features, or removing extraneous code or dependencies. Each component not developed by us is available as a forked github repository for proper attribution to its authors.

# Papers, talks, demos, consortium

A [paper](https://arxiv.org/abs/2004.04643) with details on ILLIXR, including its components, runtime, telemetry support, and a comprehensive analysis of performance, power, and quality on desktop and embedded systems.

A [talk presented at NVIDIA GTC'21](https://www.nvidia.com/en-us/gtc/catalog/?search.primarytopic=option_1564595704881&search.sessiontype=option_1614028602338&search.primaryindustrysegment=option_1563402697134&search=An%20Open-Source%20Testbed#/) describing ILLIXR and announcing the ILLIXR consortium: [Video](https://youtu.be/ZY98lWksnpM). [Slides](https://ws.engr.illinois.edu/sitemanager/getfile.asp?id=2971). 

A [demo](https://youtu.be/GVcCW8WgEDY) of an OpenXR application running with ILLIXR.

The [ILLIXR consortium](http://illixr.org) is an industry-supported community effort to democratize XR systems research, development, and benchmarking. Visit our [web site](http://illixr.org) for more information.

# Citation

We request that you cite our following [paper](https://arxiv.org/abs/2004.04643) (new version coming soon) when you use ILLIXR for a publication. We would also appreciate it if you send us a citation once your work has been published.

```
@misc{HuzaifaDesai2020,
    title={Exploring Extended Reality with ILLIXR: A new Playground for Architecture Research},
    author={Muhammad Huzaifa and Rishi Desai and Samuel Grayson and Xutao Jiang and Ying Jing and Jae Lee and Fang Lu and Yihan Pang and Joseph Ravichandran and Finn Sinclair and Boyuan Tian and Hengzhi Yuan and Jeffrey Zhang and Sarita V. Adve},
    year={2021},
    eprint={2004.04643},
    primaryClass={cs.DC}
}
```

# Getting Started and Documentation

For more information, see our [getting started page](https://illixr.github.io/ILLIXR/getting_started/).

# Acknowledgements

The ILLIXR project started in [Sarita Adve’s research group](http://rsim.cs.illinois.edu/), co-led by PhD candidate Muhammad Huzaifa, at the University of Illinois at Urbana-Champaign. Other major contributors include Rishi Desai, Samuel Grayson, Xutao Jiang, Ying Jing, Jae Lee, Fang Lu, Yihan Pang, Joseph Ravichandran, Giordano Salvador, Finn Sinclair, Boyuan Tian, Henghzhi Yuan, and Jeffrey Zhang.

ILLIXR came together after many consultations with researchers and practitioners in many domains: audio, graphics, optics, robotics, signal processing, and extended reality systems. We are deeply grateful for all of these discussions and specifically to the following: Wei Cui, Aleksandra Faust, Liang Gao, Matt Horsnell, Amit Jindal, Steve LaValle, Steve Lovegrove, Andrew Maimone, Vegard &#216;ye, Martin Persson, Archontis Politis, Eric Shaffer, Paris Smaragdis, Sachin Talathi, and Chris Widdowson.

Our OpenXR implementation uses [Monado](https://monado.dev). We are particularly thankful to Jakob Bornecrantz and Ryan Pavlik.

The development of ILLIXR was supported by the Applications Driving Architectures (ADA) Research Center, a JUMP Center co-sponsored by SRC and DARPA, the Center for Future Architectures Research (C-FAR), one of the six centers of STARnet, a Semiconductor Research Corporation program sponsored by MARCO and DARPA, the National Science Foundation under grant CCF 16-19245, DARPA, and by a Google Faculty Research Award. The development of ILLIXR was also aided by generous hardware and software donations from ARM and NVIDIA. Facebook Reality Labs provided the [OpenEDS Semantic Segmentation Dataset](https://research.fb.com/programs/openeds-challenge/).

Wesley Darvin came up with the name for ILLIXR. Abdulrahman Mahmoud helped with the design of this website.

# Licensing Structure

ILLIXR is available as open-source software under the [University of Illinois/NCSA Open Source License](https://github.com/ILLIXR/illixr.github.io/blob/master/LICENSE). As mentioned above, ILLIXR largely consists of components developed by domain experts and modified for the purposes of inclusion in ILLIXR. However, ILLIXR does contain software developed solely by us. **The NCSA license is limited to only this software**. The external libraries and softwares included in ILLIXR each have their own licenses and must be used according to those licenses:

- [ElasticFusion](https://github.com/mp3guy/ElasticFusion) \ [ElasticFusion license](https://github.com/mp3guy/ElasticFusion/blob/master/LICENSE.txt)
- [GTSAM](https://github.com/ILLIXR/gtsam) \ [Simplified BSD License](https://github.com/borglab/gtsam/blob/develop/LICENSE.BSD)
- [HOTlab](https://github.com/MartinPersson/HOTlab) \ [GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.html)
- [Kimera-VIO](https://github.com/ILLIXR/Kimera-VIO) \ [Simplified BSD License](https://github.com/MIT-SPARK/Kimera-VIO/blob/master/LICENSE.BSD)
- [libspatialaudio](https://github.com/videolabs/libspatialaudio) \ [GNU Lesser General Public License v2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
- [Monado](https://gitlab.freedesktop.org/monado/monado) \ [Boost Software License 1.0](https://choosealicense.com/licenses/bsl-1.0)
- [moodycamel::ConcurrentQueue](https://github.com/cameron314/concurrentqueue) \ [Simplified BSD License](https://github.com/cameron314/concurrentqueue/blob/master/LICENSE.md)
- [Open-VINS](https://github.com/rpng/open_vins) \ [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)
- [RITnet](https://github.com/ILLIXR/RITnet) \ [MIT License](https://github.com/AayushKrChaudhary/RITnet/blob/master/License.md)

# Get In Touch

Whether you are a computer architect, a compiler writer, a systems person, work on XR related algorithms or applications, or just anyone interested in XR research, development, or products, we would love to hear from you and hope you will contribute! You can join the [ILLIXR consortium](http://illixr.org), [discord](https://discord.gg/upkvy7x3W4), mailing list, send us an [email](mailto:illixr@cs.illinois.edu), or just send us a pull request!
