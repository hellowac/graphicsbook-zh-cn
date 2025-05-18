.. _c7:

第 7 章： 使用 WebGL 进行 3D 图形
===============================

**3D Graphics with WebGL**

.. tab:: 中文

    上一章我们讨论了WebGL，但仅限于二维图形的上下文。随着我们进入三维领域，我们将不得不处理更复杂的变换。为此，我们将主要依赖一个开源的JavaScript库来进行向量和矩阵数学运算。我们还需要实现光照和材质，这将在GLSL中直接完成。

    我们将通过复制[第3章](../c3/index.md)和[第4章](../c4/index.md)中介绍的OpenGL 1.1的大部分功能来开始本章。但很快，我们将通过添加聚光灯、Phong着色和环境映射等功能超越这些。

.. tab:: 英文

    The previous chapter covered WebGL, but only in the context of two-dimensional graphics. As we move into 3D, we will have to work with more complex transformations. For that, we will rely mainly on an open-source JavaScript library for vector and matrix math. We will also need to implement lighting and material, which we will do directly in GLSL.

    We begin the chapter by duplicating most of the capabilities of OpenGL 1.1 that were covered in [Chapter 3](../c3/index.md) and [Chapter 4](../c4/index.md). But we will soon move beyond that by adding features such as spotlights, Phong shading, and environment mapping.
