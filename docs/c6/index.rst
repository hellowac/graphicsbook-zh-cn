.. _c6:

第 6 章 WebGL 简介
=====================

**Introduction to WebGL**

.. tab:: 中文

    在本章中，我们将转向WebGL，这是OpenGL的网络版本。在 :ref:`上一章 <c5>` 中介绍的Three.js使用WebGL进行3D图形处理。当然，直接使用WebGL会更困难，但这样做可以让你完全控制图形硬件。学习它将是了解现代图形编程的一个很好的入门。WebGL与我们在 :ref:`c3` 和 :ref:`c4` 中学习的OpenGL 1.1非常不同。尽管如此，你会发现你在前几章学到的很多东西都可以应用到WebGL上。

    我并不打算全面介绍WebGL。有许多WebGL特性我甚至都不会提及，其中许多对于更高级的计算机图形学很重要。然而，我将涵盖所需的核心特性，用于2D和3D图形，以及一些更高级的特性作为额外内容。

    WebGL有两个版本，目前都还在使用。WebGL 1.0基于OpenGL ES 2.0，这是为嵌入式系统（如智能手机和平板电脑）设计的OpenGL版本。OpenGL ES 1.0，即最初的嵌入式系统OpenGL，与OpenGL 1.1非常相似。然而，OpenGL ES的2.0版本引入了重大变化。它实际上是一个更小、更简单的API，它将更多的责任放在程序员身上。例如，用于处理变换的函数，如 *glRotatef* 和 *glPushMatrix* ，已从API中移除，使程序员负责跟踪变换。WebGL不使用glBegin/glEnd生成几何体，也不使用诸如 glColor\* 或 glNormal\*之类的函数来指定顶点的属性。WebGL 1.0几乎在每个网络浏览器中都得到支持。（在某些设备上，由于硬件限制，WebGL可能被禁用。）

    基于OpenGL ES 3.0的WebGL 2.0现在几乎在所有支持WebGL 1.0的设备上都得到支持。大多数为WebGL 1.0编写的程序在WebGL 2.0下也能工作，所以你在1.0版本中学到的几乎所有东西都可以应用到新版本上。在这本教科书中，我将专注于WebGL 1.0，但我也会介绍WebGL 2.0的一些新特性。我会尽量清楚地说明我谈论的仅适用于WebGL 2.0的特性。

    任何WebGL程序都有两个方面。程序的一部分是用JavaScript编写的，这是网络的编程语言。第二部分是用GLSL编写的，这是一种用于编写在GPU上运行的“着色器”程序的语言。WebGL 1.0使用GLSL ES 1.00（嵌入式系统的OpenGL着色器语言，版本1.00）。WebGL 2.0可以使用GLSL ES 1.00编写的着色器程序，但它也可以使用GLSL ES 3.00，后者有一些重大差异以及新特性。我会尽量清楚地说明我正在讨论的语言。

    对于这本关于WebGL的介绍性章节，我们将坚持基本的2D图形。你将了解WebGL程序的结构。你将学到API的JavaScript方面的大部分内容，你将学会如何编写和使用简单的着色器。在[下一章](../c7/index.md)中，我们将转向3D图形，你将了解更多关于GLSL的知识。

    .. toctree::
       :maxdepth: 1
       :caption: 第 6 章内容

       s1.rst
       s2.rst
       s3.rst
       s4.rst
       s5.rst

.. tab:: 英文

    In this chapter, we turn to WebGL, the version of OpenGL for the Web. Three.js, which was covered in the [previous chapter](../c5/index.md), uses WebGL for 3D graphics. Of course, it is more difficult to use WebGL directly, but doing so gives you full control over the graphics hardware. And learning it will be a good introduction to modern graphics programming. WebGL is very different from OpenGL 1.1, which we studied in [Chapter 3](../c3/index.md) and [Chapter 4](../c4/index.md). Nevertheless, it will turn out that much of what you learned in previous chapters will carry over to WebGL.

    It is not my intention to cover WebGL in its entirety. There are many WebGL features that I will not even mention, and many of those are important for more advanced computer graphics. However, I will cover the core features that are needed for 2D and 3D graphics, along with a few of the more advanced aspects, as a bonus.

    There are two versions of WebGL, both of them still in use. WebGL 1.0 is based on OpenGL ES 2.0, a version of OpenGL designed for use on embedded systems such as smart phones and tablets. OpenGL ES 1.0, the original OpenGL for embedded systems, was very similar to OpenGL 1.1. However, the 2.0 version of OpenGL ES introduced major changes. It is actually a smaller, simpler API that puts more responsibility on the programmer. For example, functions for working with transformations, such as *glRotatef* and *glPushMatrix*, were eliminated from the API, making the programmer responsible for keeping track of transformations. WebGL does not use glBegin/glEnd to generate geometry, and it doesn't use function such as glColor*or glNormal* to specify attributes of vertices. WebGL 1.0 is supported in almost every web browser. (On some devices, WebGL might be disabled because of hardware limitations.)

    WebGL 2.0, which is based on OpenGL ES 3.0, is now supported on almost all devices that suport WebGL 1.0. Most programs written for WebGL 1.0 will also work under WebGL 2.0, so almost everything that you learn about the 1.0 version will carry over to the newer version. In this textbook, I will concentrate on WebGL 1.0, but I will also cover some of the new features of WebGL 2.0. I will try to make it clear when I am talking about features that only apply to WebGL 2.0.

    There are two sides to any WebGL program. Part of the program is written in JavaScript, the programming language for the web. The second part is written in GLSL, a language for writing "shader" programs that run on the GPU. WebGL 1.0 uses GLSL ES 1.00 (the OpenGL Shader Language for Embedded Systems, version 1.00). WebGL 2.0 can use shader programs written in GLSL ES 1.00, but it can also use GLSL ES 3.00, which has some significant differences as well as new features. I will try to always be clear about which language I am discussing.

    For this introductory chapter about WebGL, we will stick to basic 2D graphics. You will learn about the structure of WebGL programs. You will learn most of the JavaScript side of the API, and you will learn how to write and use simple shaders. In the [next chapter](../c7/index.md), we will move on to 3D graphics, and you will learn a great deal more about GLSL.
