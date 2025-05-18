.. _c5:

第 5 章： Three.js：3D 场景图 API
==================================


**Three.js: A 3D Scene Graph API**

.. tab:: 中文

    [第3章](../c3/index.md)和[第4章](../c4/index.md)介绍了使用OpenGL 1.1的3D图形。这些章节中涵盖的大部分理念在现代计算机图形学中仍然相关，但自从OpenGL早期以来，已经发生了许多变化和改进。在[第6章](../c6/index.md)和[第7章](../c7/index.md)中，我们将使用WebGL，这是一个用于在网页上创建3D图形内容的现代OpenGL版本。而[第9章](../c9/index.md)介绍了WebGPU，这是一个更新的Web图形API。

    WebGL是一种低级语言——甚至比OpenGL 1.1还要低级，因为WebGL程序必须处理许多在OpenGL原始版本中内部处理的低级实现细节。这使得WebGL更加灵活，但也更难使用。我们很快将直接使用WebGL。然而，在我们这么做之前，我们将看看一个构建在WebGL之上的更高级的API，用于3D Web图形：**three.js**。从这个高级开始有几个原因。它将允许你看到一些你已经学到的东西是如何在现代面向对象图形包中使用的。它将允许我介绍一些新特性，如阴影和环境映射。它将让你使用一个你可能在真实Web应用程序中使用的图形库。并且在我们继续深入更底层之前，它将让我们从我们一直在处理的低级细节中解脱出来。

    你很可能可以在不了解JavaScript的情况下跟随本章的大部分讨论。然而，如果你想使用three.js（或WebGL或WebGPU）进行任何编程，你需要知道JavaScript。语言的基础知识在[附录A](../a1/index.md)的[A.3节](../a1/s3.md)中介绍。

.. tab:: 英文

    [Chapter 3](../c3/index.md) and [Chapter 4](../c4/index.md) introduced 3D graphics using OpenGL 1.1. Most of the ideas covered in those chapters remain relevant to modern computer graphics, but there have been many changes and improvements since the early days of OpenGL. In [Chapter 6](../c6/index.md) and [Chapter 7](../c7/index.md), we will be using WebGL, a modern version of OpenGL that is used to create 3D graphics content for web pages. And [Chapter 9](../c9/index.md) introduces WebGPU, a newer graphics API for the Web.

    WebGL is a low level language—even more so than OpenGL 1.1, since a WebGL program has to handle a lot of the low-level implementation details that were handled internally in the original version of OpenGL. This makes WebGL much more flexible, but more difficult to use. We will soon turn to working directly with WebGL. However, before we do that, we will look at a higher-level API for 3D web graphics that is built on top of WegGL: **three.js**. There are several reasons for starting at this high level. It will allow you to see how some of the things that you have learned are used in a modern object-oriented graphics package. It will allow me to introduce some new features such as shadows and environment mapping. It will let you work with a graphics library that you might use in real web applications. And it will be a break from the low-level detail we have been dealing with, before we move on to an even lower level.

    You can probably follow much of the discussion in this chapter without knowing JavaScript. However, if you want to do any programming with three.js (or with WebGL or WebGPU), you need to know JavaScript. The basics of the language are covered in [Section A.3](../a1/s3.md) in [Appendix A](../a1/index.md).
