.. _c3:

第 3 章 OpenGL 1.1 几何
======================

**OpenGL 1.1: Geometry**

.. tab:: 中文

    现在是时候转向三维计算机图形了，尽管我们真正涉足三维的部分要到本章的第2节才开始。你会发现，许多二维图形的概念都可以延续到三维，但进入第三维度带来了一些新的特性，需要一段时间来适应。

    我们的重点将放在 **OpenGL** 上，这是一个图形API，于1992年推出，自那以后经历了许多版本和许多变化。OpenGL是一个低级别的图形API，类似于我们所涵盖的二维API。在某些方面甚至更加原始，但当然由于支持三维，它变得更加复杂。OpenGL是Web上三维应用程序的当前标准WebGL的基础，在 :ref:`c6` 和 :ref:`c7` 中有所介绍。有许多竞争的低级三维图形框架，包括微软的Direct3D、苹果的Metal和Vulkan，后者是由OpenGL的创建者设计的，作为一种更现代化、高效的替代品。

    在接下来的两章中，我们将讨论OpenGL 1.1。OpenGL 1.1是一个庞大的API，我们只会涵盖其中的一部分。我们的目标是介绍三维图形的概念，而不是完全涵盖API。我们在这里涵盖的部分在最现代化的OpenGL版本，包括WebGL中已被删除。然而，更现代的图形API有一个非常陡峭的初始学习曲线，对于初次接触三维图形的人来说，并不是最好的起点。需要一些额外的支持——如果不是OpenGL 1.1，那么就是类似的框架。由于OpenGL 1.1至少在所有桌面OpenGL实现中仍然受到支持，因此它是学习三维图形的一个合理的起点。

    本章集中讨论三维图形的几何方面，如定义和变换对象以及将三维场景投影到二维图像中。我们生成的图像看起来会非常不真实。在下一章中，我们将看到如何通过模拟光照效果和表面材质属性来增加一些真实感。

    .. toctree::
       :maxdepth: 1
       :caption: 第 3 章内容

       s1.rst
       s2.rst
       s3.rst
       s4.rst
       s5.rst
       s6.rst

.. tab:: 英文

    It is time to move on to computer graphics in three dimensions, although it won't be until Section 2 of this chapter that we really get into 3D. You will find that many concepts from 2D graphics carry over to 3D, but the move into the third dimension brings with it some new features that take a while to get used to.

    Our focus will be **OpenGL**, a graphics API that was introduced in 1992 and has gone through many versions and many changes since then. OpenGL is a low-level graphics API, similar to the 2D APIs we have covered. It is even more primitive in some ways, but of course it is complicated by the fact that it supports 3D. OpenGL is the basis for WebGL, the current standard for 3D applications on the Web that is covered in :ref:`Chapter 6 <c6>` and :ref:`Chapter 7 <c7>`. There are many competing frameworks for low-level 3D graphics, including Microsoft's Direct3D, Apple's Metal, and Vulkan, which was designed by the creators of OpenGL as a more modern and efficient replacement.

    For the next two chapters, the discussion is limited to OpenGL 1.1. OpenGL 1.1 is a large API, and we will only cover a part of it. The goal is to introduce 3D graphics concepts, not to fully cover the API. A significant part of what we cover here has been removed from the most modern versions of OpenGL, including WebGL. However, more modern graphics APIs have a very steep initial learning curve, and they are not really the best starting place for someone who is encountering 3D graphics for the first time. Some additional support is needed—if not OpenGL 1.1 then some similar framework. Since OpenGL 1.1 is still supported, at least by all desktop implementations of OpenGL, it's a reasonable place to start learning about 3D graphics.

    This chapter concentrates on the geometric aspects of 3D graphics, such as defining and transforming objects and projecting 3D scenes into 2D images. The images that we produce will look very unrealistic. In the next chapter, we will see how to add some realism by simulating the effects of lighting and of the material properties of surfaces.
