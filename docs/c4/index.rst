.. _c4:

第 4 章 OpenGL 1.1 灯光和材质
==============================

**OpenGL 1.1: Light and Material**

.. tab:: 中文

    计算机图形学的一个目标是物理真实性，即制作看起来像是现实世界中的照片的图像。这并不是唯一的目标。例如，对于科学可视化，目标是使用计算机图形以准确清晰的方式呈现信息。艺术家可以利用计算机图形来创造抽象而不是逼真的艺术作品。然而，真实性是计算机图形最明显的用途之一的主要目标，比如视频游戏、电影和广告。

    物理真实性的一个重要方面是光照：光影的变化、光线从不同材料反射的方式，以及透明物体通过时光线弯曲或衍射的方式。用于产生最真实图形的技术可以考虑所有这些因素以及更多。

    然而，计算机图形的另一个目标是速度。OpenGL，特别是为 **实时图形** 设计的，其中可用于渲染图像的时间是秒的一小部分。对于动画电影，如果每帧渲染花费几个小时也没关系。但是，视频游戏预期每秒渲染六十帧。即使使用现代计算机图形硬件的惊人速度，也需要进行妥协来获得这种速度。三十年前，当OpenGL还很新时，这种妥协要大得多。

    在本章中，我们将学习OpenGL 1.1中的光照和材质。您将学习如何配置光源以及如何将材质属性分配给对象。材质属性确定对象与光的相互作用方式。您还将学习如何将图像应用到表面作为纹理。在今天的标准下，OpenGL 1.1中的光、材质和纹理的支持相对简单和不完整。但是，它使用的概念仍然是现代实时图形甚至最真实的计算机图形的基础。

    .. toctree::
       :maxdepth: 1
       :caption: 第 4 章内容

       s1.rst
       s2.rst
       s3.rst
       s4.rst

.. tab:: 英文

    One of the goals of computer graphics is physical realism, that is, making images that look like they could be photographs of reality. This is not the only goal. For example, for scientific visualization, the goal is to use computer graphics to present information accurately and clearly. Artists can use computer graphics to create abstract rather than realistic art. However, realism is a major goal of some of the most visible uses of computer graphics, such as video games, movies, and advertising.

    One important aspect of physical realism is lighting: the play of light and shadow, the way that light reflects from different materials, the way it can bend or be diffracted as it passes through translucent objects. The techniques that are used to produce the most realistic graphics can take all these factors and more into account.

    However, another goal of computer graphics is speed. OpenGL, in particular, was designed for **real-time graphics**, where the time that is available for rendering an image is a fraction of a second. For an animated movie, it's OK if it takes hours to render each frame. But a video game is expected to render sixty frames every second. Even with the incredible speed of modern computer graphics hardware, compromises are necessary to get that speed. And thirty years ago, when OpenGL was still new, the compromises were a lot bigger

    In this chapter, we look at light and material in OpenGL 1.1. You will learn how to configure light sources and how to assign material properties to objects. Material properties determine how the objects interact with light. And you will learn how to apply an image to a surface as a texture. The support for light, material, and texture in OpenGL 1.1 is relatively crude and incomplete, by today's standards. But the concepts that it uses still serve as the foundation for modern real-time graphics and, to a significant extent, even for the most realistic computer graphics.
