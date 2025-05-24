.. _a4:

附录 D 示例程序和源代码
====================

**Source Code and Demos**

.. tab:: 中文

    这本书的网页版下载中，源代码示例可以在名为“source”的文件夹中找到。此页面还包含了书中使用的所有“实时演示”的链接列表；它们可以在名为“demos”的文件夹中找到。

    （注意：HTML canvas 图形、three.js、WebGL 和 WebGPU 的示例和演示是 HTML 文件，可以在网络浏览器中打开。要查看源代码，你可以在纯文本编辑器中打开文件，或者在网络浏览器中打开它并使用浏览器的“查看源代码”命令。许多 HTML 程序会加载图形模型和其他文件。在大多数浏览器中，使用这些资源的程序在从本地硬盘加载 HTML 文件时将无法工作。也就是说，当从这本书的网页版下载的源代码或演示文件夹中运行时，它们在那些网络浏览器中会失败。当通过网络服务器加载时，程序应该可以正常工作。可以在当地运行网络服务器。可能可以配置你的网络浏览器以使用本地文件的资源，但通常不建议使用该设置浏览网络。）

.. tab:: 英文

    This page contains links to source code for the programs that are used as examples in this book. In the web site download of the book, the source code examples can be found in the folder named source. This page also contains a list of links to all of the "live demos" that are used in the book; they can be found in the folder named demos.

    (Note: Examples and demos for HTML canvas graphics, three.js, WebGL, and WebGPU are html files, which can be opened in a web browser. To see the source code, you can open the file in a plain text editor, or you can open it in a Web browser and use the browser's "View Source" command. Many of the html programs load graphical models and other files. In most browsers, the programs that use such resources will not work when the html files are loaded from a local hard drive. That is, they will fail in those web browsers when run from the source or demo folder in the web site download of this book. The programs should work OK when loaded through a web server. It is possible to run a web server locally. It might be possible to configure your web browser to use resources from local files, but it is generally not recommended to browse the web with that setting.)

1. Java Graphics2D 示例
------------------------

**1. Java Graphics2D Examples**

.. tab:: 中文

    在这本书的 :ref:`c2.4` 和 :ref:`c2.5` 中，有一些示例使用了 Java Swing GUI 工具包中包含的 2D 图形 API。在网站下载的版本中，这些示例的源代码可以在源文件夹内的 `java2d </../en/en/source/java2d/>`_ 文件夹中找到。每个示例都是一个单独的文件，可以编译生成应用程序；不需要额外的 Java 文件。

    - `HierarchicalModeling2D.java </../en/source/java2d/HierarchicalModeling2D.java>`_ — 展示了一个简单的动画场景，包括移动的手推车和旋转的风车，它使用了分层建模。在这个程序版本中，层次结构是通过过程式实现的，使用子程序来绘制场景中的对象。
    - `SceneGraphAPI2D.java </../en/source/java2d/SceneGraphAPI2D.java>`_ — 展示了与前一个示例相同的场景，但这次使用场景图数据结构实现。场景图是使用主类中的静态嵌套类实现的。
    - `GraphicsStarter.java </../en/source/java2d/GraphicsStarter.java>`_ 和 `AnimationStarter.java </../en/source/java2d/AnimationStarter.java>`_ 分别绘制简单的静态和动画场景，旨在作为使用 Java 图形的实验框架。 `EventsStarter.java </../en/source/java2d/EventsStarter.java>`_ 是一个类似的框架，用于在图形程序中处理鼠标和键盘事件。
    - `PaintDemo.java </../en/source/java2d/PaintDemo.java>`_ 绘制了一个可以填充渐变或纹理图像的多边形，并允许你调整它们的性质。这只是 Java 绘画的演示。图像文件 `QueenOfHearts.png </../en/source/java2d/QueenOfHearts.png>`_ 和 `TinySmiley.png </../en/source/java2d/TinySmiley.png>`_ 是这个程序的一部分，当程序运行时，它们必须与编译的 Java 类文件在同一位置。
    - `JavaPixelManipulation.java </../en/source/java2d/JavaPixelManipulation.java>`_ 是一个演示，它在 BufferedImage 中操作单个像素的颜色。用户可以绘制一个简单的图片或从文件加载图片。"涂抹"工具将像素颜色涂抹开来，过滤器通过对图像中的像素颜色执行平均操作来修改图像。

.. tab:: 英文

    There are a few examples in :ref:`Section 2.4 <c2.4>` and :ref:`Section 2.5 <c2.5>` that uses the 2D graphics API that is part of Java's Swing GUI toolkit. In the web site download, the source code for these examples can be found in the folder named `java2d </../en/en/source/java2d/>`_ inside the source folder. Each example is a single file that can be compiled to produce an application; no additional Java files are needed.

    - `HierarchicalModeling2D.java </../en/source/java2d/HierarchicalModeling2D.java>`_ — shows a simple animated scene, with a moving cart and rotating windmills, that uses hierarchical modeling. In this version of the program, the hierarchy is implemented procedurally, using subroutines to draw the objects in the scene.
    - `SceneGraphAPI2D.java </../en/source/java2d/SceneGraphAPI2D.java>`_ — shows the same scene as the previous example, but this time implemented using a scene graph data structure. The scene graph is implemented using static nested classes in the main class.
    - `GraphicsStarter.java </../en/source/java2d/GraphicsStarter.java>`_ and `AnimationStarter.java </../en/source/java2d/AnimationStarter.java>`_ draw simple static and animated scenes, respectively, and are meant to be used as a framework for experimenting with Java graphics. `EventsStarter.java </../en/source/java2d/EventsStarter.java>`_ is a similar framework for working with mouse and key events in a graphics program.
    - `PaintDemo.java </../en/source/java2d/PaintDemo.java>`_ draws a polygon that can be filled with either a gradient or a texture image, and lets you adjust their properties. This is just a demo of Java paints. The image files `QueenOfHearts.png </../en/source/java2d/QueenOfHearts.png>`_ and `TinySmiley.png </../en/source/java2d/TinySmiley.png>`_ are part of this program and must be in the same location as the compiled Java class files when the program is run.
    - `JavaPixelManipulation.java </../en/source/java2d/JavaPixelManipulation.java>`_ is a demo that manipulates colors of individual pixels in a BufferedImage. The user can draw a simple picture or load an image from a file. A "Smudge" tool smears out pixel colors, and filters modify the image by performing averaging operations on the pixel colors in the image.

2. HTML Canvas 2D 示例
------------------------

**2. HTML Canvas 2D Examples**

.. tab:: 中文

    在 :ref:`c2.6` 中讨论了 2D 画布 API，并且在那一节中提到了几个示例。画布示例被编写为网页，你可以在浏览器中查看网页来了解它的功能。然而，你也应当阅读源代码。前四个示例旨在作为你自己实验的基础。（注意， :ref:`c2` 中的所有实时演示都使用了画布 API，但你不一定需要理解演示的源代码。）在这本书的网站下载中，你可以在源文件夹内的 `canvas2d </../en/source/canvas2d/>`_ 文件夹中找到这些示例。

    - `GraphicsStarter.html </../en/source/canvas2d/GraphicsStarter.html>`_ 是一个在 HTML 画布上绘图的最小框架。它包括绘制文本和各种形状的示例。
    - `GraphicsPlusStarter.html </../en/source/canvas2d/GraphicsPlusStarter.html>`_ 在前一个示例中增加了一些便利函数，包括一个在画布上设置坐标系的函数，以及一些基本 API 中未包含的绘制线条和椭圆形等形状的函数。它包括使用变换的示例。
    - `AnimationStarter.html </../en/source/canvas2d/AnimationStarter.html>`_ 在前一个示例中增加了动画，并包括了一个使用分层建模的简单示例。
    - `EventsStarter.html </../en/source/canvas2d/EventsStarter.html>`_ 是一个使用键盘和鼠标事件与画布交互的最小框架，其中一些基本事件处理的示例。
    - `SimplePaintProgram.html </../en/source/canvas2d/SimplePaintProgram.html>`_ 允许用户使用简单形状进行绘图。还有一个“涂抹”工具，允许用户像在湿漆上绘画一样涂抹图画；这是 HTML 画布 API 中像素操作的一个示例。程序展示了如何使用“离屏画布”。演示程序 `c2/SimplePaintDemo.html </../en/demos/c2/SimplePaintDemo.html>`_ 是这个程序的一个版本，它使用“叠加画布”而不是离屏画布。

.. tab:: 英文

    The 2D canvas API is discussed in :ref:`Section 2.6 <c2.6>`, and several examples are mentioned in that section. Canvas examples are written as web pages, and you can look at the web page in a browser to see what it does. However, you are also meant to read the source code. And the first four examples are meant to be used as a basis for your own experimentation. (Note that all of the live demos in :ref:`Chapter 2 <c2>` use the canvas API, but you are not necessarily meant to understand the source code of the demos.) In the web site download of this book, you can find these examples in the `canvas2d </../en/source/canvas2d/>`_ folder inside the source folder.

    - `GraphicsStarter.html </../en/source/canvas2d/GraphicsStarter.html>`_ is a minimal framework for drawing on an HTML canvas. It includes examples of drawing text and various shapes.
    - `GraphicsPlusStarter.html </../en/source/canvas2d/GraphicsPlusStarter.html>`_ adds a few convenience functions to the previous example, including a function for setting up a coordinate system on the canvas and functions to draw shapes such as lines and ovals that are not included in the basic API. It includes examples of using transforms
    - `AnimationStarter.html </../en/source/canvas2d/AnimationStarter.html>`_ adds animation to the previous example and includes a simple example using hierarchical modeling.
    - `EventsStarter.html </../en/source/canvas2d/EventsStarter.html>`_ is a minimal framework for using keyboard and mouse events with a canvas, with some examples of basic event handling.
    - `SimplePaintProgram.html </../en/source/canvas2d/SimplePaintProgram.html>`_ lets the user draw using simple shapes. There is also a "smudge" tool that lets the user smudge the drawing as if it is drawn in wet paint; this is an example of pixel manipulation in the HTML canvas API. The program shows how to use an "off-screen canvas." The demo program `c2/SimplePaintDemo.html </../en/demos/c2/SimplePaintDemo.html>`_ is a version of this program that uses an "overlay canvas" instead of an off-screen canvas.

3. SVG 示例
------------------------

**3. Scalable Vector Graphics Examples**

.. tab:: 中文

    [第 2.7 节](../c2/s7.md) 讨论了 SVG，这是一种用于二维矢量图形的场景描述语言。在那一节中讨论了几个示例。这些示例可以在网络浏览器中打开，以查看它们产生的图像。查看网页的源代码，了解生成图像的程序。你也可以在文本编辑器中打开文件，阅读源代码。一些示例产生了动画图像。SVG 图像应该在几乎所有现代网络浏览器中都能工作。这些示例可以在源文件夹内的 svg 文件夹中找到。

    - `first-svg-example.svg </../en/source/svg/first-svg-example.svg>`_ 是一个非常简单的示例，只绘制了一些基本形状。
    - `svg-starter.svg </../en/source/svg/svg-starter.svg>`_ 展示了 SVG 图像的基本文档结构，包括大多数基本形状的示例，并有许多注释来解释发生了什么。
    - `svg-face.svg </../en/source/svg/svg-face.svg>`_ 是一个非常简单的分组示例。
    - `svg-hierarchy.svg </../en/source/svg/svg-hierarchy.svg>`_ 是一个分层建模的示例，它制作了一个车轮模型和一个使用两个车轮作为组件的手推车模型。图像显示了一个车轮和四辆手推车的副本。车轮和手推车模型也用于列表末尾的风车动画。
    - `first-svg-animation.svg </../en/source/svg/first-svg-animation.svg>`_ 包含了简单动画、关键帧动画和变换动画的示例。
    - `hierarchical-animation.svg </../en/source/svg/hierarchical-animation.svg>`_ 展示了一个简单的分层动画模型。
    - `cart-and-windmill.svg </../en/source/svg/cart-and-windmills.svg>`_ 是 SVG 中分层建模的一个更复杂的示例。场景是一个动画，显示一个“手推车”在风车转动的背景下沿着道路移动。这个动画与 Java 示例 `java2d/HierarchicalModeling2D.java </../en/source/java2d/HierarchicalModeling2D.java>`_ 和 JavaScript 演示 `c2/cart-and-windmills.html </../en/demos/c2/cart-and-windmills.html>`_ 中实现的动画相同。


.. tab:: 英文

    [Section 2.7](../c2/s7.md) discusses SVG, a scene description language for 2D vector graphics. Several examples were discussed in that section. These examples can be opened in a web browser to see the images they produce. View the source code for the web page to see the program that produces the image. You can also open the files in a text editor to read the source. Some of the examples produce animated images. SVG images should work in almost all modern web browsers. These examples can be found in the svg folder inside the source folder.

    - `first-svg-example.svg </../en/source/svg/first-svg-example.svg>`_ is a very short first example that just draws a few basic shapes.
    - `svg-starter.svg </../en/source/svg/svg-starter.svg>`_ shows the basic document structure for an SVG image, includes examples of most of the basic shapes, and has a lot of comments to explain what is going on.
    - `svg-face.svg </../en/source/svg/svg-face.svg>`_ is a very simple first example of grouping.
    - `svg-hierarchy.svg </../en/source/svg/svg-hierarchy.svg>`_ is an example of hierarchical modeling that makes a model of a wheel and a model of a cart that uses two wheels as components. The image shows a wheel and four copies of the cart. The wheel and cart models are also used in the cart-and-windmill animation at the end of this list.
    - `first-svg-animation.svg </../en/source/svg/first-svg-animation.svg>`_ contains examples of simple animation, keyframe animation, and transform animation.
    - `hierarchical-animation.svg </../en/source/svg/hierarchical-animation.svg>`_ shows a simple animated hierarchical model.
    - `cart-and-windmill.svg </../en/source/svg/cart-and-windmills.svg>`_ is a more complex example of hierarchical modeling in SVG. The scene is an animation that shows a "cart" moving down a road as windmills turn in the background. The animation is the same as the one implemented in the Java example `java2d/HierarchicalModeling2D.java </../en/source/java2d/HierarchicalModeling2D.java>`_ and in the JavaScript demo `c2/cart-and-windmills.html </../en/demos/c2/cart-and-windmills.html>`_.


4. OpenGL 1.1 示例
------------------------

**4. OpenGL 1.1 Examples**

.. tab:: 中文

    OpenGL 1.1 是 :ref:`c3` 和 :ref:`c4` 的主题。这些章节中的示例主要使用 OpenGL 的 C API。然而，也讨论了 Java API，JOGL。大多数程序示例都可以在 C 和 Java API 中找到。JOGL 版本可以在源目录中的 `jogl </../en/en/source/jogl/>`_ 目录中找到。使用 GLUT 库创建和管理 OpenGL 窗口的 C 版本可以在源目录中的 `glut </../en/source/glut/>`_ 目录中找到（这些程序中的许多都使用在 `jogl/Camera.java </../en/source/jogl/Camera.java>`_ 中为 Java 定义的“摄像机”API，在 `glut/camera.c </../en/source/glut/camera.c>`_ 和 `glut/camera.h </../en/source/glut/camera.h>`_ 中为 C 定义）。

    书中的 OpenGL 演示是用 glsim.js 编写的，这是一个 JavaScript 库，它在 WebGL 1.0 上实现了 OpenGL 1.1 的一小部分 C API。关于 glsim 的信息可以在 `glsim/glsim-doc.html </../en/source/glsim/glsim-doc.html>`_ 中找到。一些程序示例也有使用 glsim 库的 HTML 版本。它们可以在源目录中的 `glsim </../en/source/glsim/>`_ 目录中找到。

    - `glut/first-triangle.c </../en/source/glut/first-triangle.c>`_ 、 `jogl/FirstTriangle.java </../en/source/jogl/FirstTriangle.java>`_ 和 `glsim/first-triangle.html </../en/source/glsim/first-triangle.html>`_ 分别是 C、Java 和 JavaScript 版本的非常基础的 OpenGL 示例：一个顶点分别被分配红色、绿色和蓝色颜色的三角形。你可以使用这个示例作为尝试一些基本 2D 绘图命令的起点。来自 :ref:`c3.1` 。
    - `glut/unlit-cube.c </../en/source/glut/unlit-cube.c>`_、 `jogl/UnlitCube.java </../en/source/jogl/UnlitCube.java>`_ 和 `glsim/unlit-cube.html </../en/source/glsim/unlit-cube.html>`_ 分别是 C、Java 和 JavaScript 版本的程序，该程序使用应用于正方形的建模变换绘制立方体。这个程序中没有照明，并且它使用基本的正交投影，所以图像不是真实的。来自 :ref:`c3.2` 。
    - `glut/opengl-cart-and-windmill-2d.c </../en/source/glut/opengl-cart-and-windmill-2d.c>`_ （C 语言）、 `jogl/CartAndWindmillJogl2D.java </../en/source/jogl/CartAndWindmillJogl2D.java>`_ （Java）和 `glsim/opengl-cart-and-windmill.html </../en/source/glsim/opengl-cart-and-windmill.html>`_ （JavaScript）是 OpenGL 1.1 中二维分层建模和动画的示例版本。它说明了 OpenGL 中的 2D 图形以及使用 glPushMatrix 和 glPopMatrix 进行分层建模的使用。动画与 Java Graphics2D 示例 `java2d/HierarchicalModeling2D.java </../en/source/java2d/HierarchicalModeling2D.java>`_ 和 HTML 画布图形演示 `c2/cart-and-windmills.html </../en/demos/c2/cart-and-windmills.html>`_ 中实现的动画几乎相同。来自 :ref:`c3.2` 。
    - `glut/camera.c </../en/source/glut/camera.c>`_ 和相应的头文件 `glut/camera.h </../en/source/glut/camera.h>`_ 对于 C，或 `jogl/Camera.java </../en/source/jogl/Camera.java>`_ 对于 JOGL，实现了与 OpenGL 1.1 一起使用的“摄像机”API。这是一个库，用于其他程序，本身不是一个完整的程序。JavaScript 的相应 API 是我的 GLSim 库的一部分， `glsim/glsim.js </../en/source/glsim/glsim.js>`_ 。大多数以下示例中都使用了摄像机。在 :ref:`c3.3` 中讨论。
    - `glut/ifs-polyhedron-viewer.c </../en/source/glut/ifs-polyhedron-viewer.c>`_ 和 `jogl/IFSPolyhedronViewer.java </../en/source/jogl/IFSPolyhedronViewer.java>`_ 分别是 C 和 Java 版本的程序，允许用户查看定义为索引面集的多面体。多面体模型在 `jogl/Polyhedron.java </../en/source/jogl/Polyhedron.java>`_ 中为 Java 定义，在 `glut/polyhedron.c </../en/source/glut/polyhedron.c>`_ 和 `glut/polyhedron.h </../en/source/glut/polyhedron.h>`_ 中为 C 定义。这个程序还要求使用前一项中讨论的摄像机 API。来自 :ref:`c3.4` 。
    - `glut/cubes-with-vertex-arrays.c </../en/source/glut/color-cube-of-spheres.c>`_ 、 `jogl/CubesWithVertexArrays.java </../en/source/jogl/ColorCubeOfSpheres.java>`_ 和 JavaScript 版本 glsim/cubes-with-vertex-arrays.html 演示了使用 glDrawArrays 和 glDrawElements 进行绘制。来自 :ref:`c3.4`。
    - `glut/color-cube-of-spheres.c </../en/source/glut/glut-starter.c>`_ 和 `jogl/ColorCubeOfSpheres.java </../en/source/jogl/JoglStarter.java>`_ 绘制了大量球体，使用了各种渲染方法，并显示了渲染图像所需的时间。重点是比较不同渲染方法的渲染时间，包括显示列表、glDrawArrays 和顶点缓冲对象。读者不需要理解这个程序中的所有代码。来自 :ref:`c3.4`。
    - `glut/glut-starter.c </../en/source/glut/color-cube-of-spheres.c>`_ 、 `jogl/JoglStarter.java </../en/source/jogl/JoglStarter.java>`_ 和 `glsim/glsim-starter.html </../en/source/glsim/glsim-starter.html>`_ 是使用 C、Java 和我的 JavaScript OpenGL 模拟器编写 OpenGL 1.1 应用程序的“启动”文件。这些程序不绘制任何内容，但它们具有用于绘制以及鼠标和键盘交互以及动画的函数/方法桩。在 :ref:`c3.6` 中讨论。
    - `glut/four-lights.c </../en/source/glut/four-lights.c>`_ 和 `jogl/FourLights.java </../en/source/jogl/FourLights.java>`_ 是使用光源和材质属性的示例。程序演示了多个移动光源，并允许用户打开和关闭灯光以查看效果。演示 `glsim/fout-lights-demo.html </../en/demos/glsim/fout-lights-demo.html>`_ 是同一个程序的 JavaScript 版本。来自 :ref:`c4.3` 。
    - `glut/texture-demo.c </../en/source/glut/texture-demo.c>`_ 是一个 C 程序，展示了各种对象上的多种纹理。它依赖于文件 `glut/textured-shapes.c </../en/source/glut/textured-shapes.c>`_ 和 `glut/textured-shapes.h </../en/source/glut/textured-shapes.h>`_ ，以及包含程序


.. tab:: 英文

    OpenGL 1.1 is the topic of :ref:`Chapter 3 <c3>` and :ref:`Chapter 4 <c4>`. Examples in those chapters primarily use the C API for OpenGL. However, the Java API, JOGL, is also discussed. Most program examples are available in both the C and the Java APIs. The JOGL versions can be found in the directory named `jogl </../en/en/source/jogl/>`_ inside the source directory. The C versions, which use the GLUT library to create and manage OpenGL windows, can be found in the directory named `glut </../en/source/glut/>`_ inside source. (Many of these programs use a "camera" API defined in `jogl/Camera.java </../en/source/jogl/Camera.java>`_ for Java and in `glut/camera.c </../en/source/glut/camera.c>`_ and `glut/camera.h </../en/source/glut/camera.h>`_ for C.)

    The OpenGL demos in the book are written using glsim.js, a JavaScript library that implements a small subset of the C API for OpenGL 1.1 on top of WebGL 1.0. Information about glsim can be found in `glsim/glsim-doc.html </../en/source/glsim/glsim-doc.html>`_. Some of the program examples are available in HTML versions that use the glsim library. They can be found in the `glsim </../en/source/glsim/>`_ directory inside the source directory.

    - `glut/first-triangle.c </../en/source/glut/first-triangle.c>`_ ,  `jogl/FirstTriangle.java </../en/source/jogl/FirstTriangle.java>`_ and `glsim/first-triangle.html </../en/source/glsim/first-triangle.html>`_ are C, Java, and JavaScript versions of the very first OpenGL example: a triangle whose vertices are assigned the colors red, green, and blue. You can use this example as a starting point for trying out some basic 2D drawing commands. From :ref:`Section 3.1 <c3.1>`.
    - `glut/unlit-cube.c </../en/source/glut/unlit-cube.c>`_,  `jogl/UnlitCube.java </../en/source/jogl/UnlitCube.java>`_, and  `glsim/unlit-cube.html </../en/source/glsim/unlit-cube.html>`_ are C, Java, and JavaScript versions of a program that draws a cube using modeling transformations applied to a square. There is no lighting in this program, and it uses a basic orthographic projection, so the image is not realistic. From :ref:`Section 3.2 <c3.2>`.
    - `glut/opengl-cart-and-windmill-2d.c </../en/source/glut/opengl-cart-and-windmill-2d.c>`_ (for C), `jogl/CartAndWindmillJogl2D.java </../en/source/jogl/CartAndWindmillJogl2D.java>`_  (for Java), and `glsim/opengl-cart-and-windmill.html </../en/source/glsim/opengl-cart-and-windmill.html>`_ (for JavaScript) are versions of an example of hierarchical modeling and animation in two dimensions with OpenGL 1.1. It illustrates 2D graphics in OpenGL as well as the use of glPushMatrix and glPopMatrix for hierarchical modeling. The animation is almost the same as the one implemented in the Java Graphics2D example `java2d/HierarchicalModeling2D.java </../en/source/java2d/HierarchicalModeling2D.java>`_ and in the HTML canvas graphics demo `c2/cart-and-windmills.html </../en/demos/c2/cart-and-windmills.html>`_ . From :ref:`Section 3.2 <c3.2>`.
    - `glut/camera.c </../en/source/glut/camera.c>`_ and the corresponding header file `glut/camera.h </../en/source/glut/camera.h>`_ for C, or `jogl/Camera.java </../en/source/jogl/Camera.java>`_ for JOGL, implement a "camera" API for use with OpenGL 1.1. This is a library for use in other programs, not itself a complete program. The corresponding API for JavaScript is part of my GLSim library, `glsim/glsim.js </../en/source/glsim/glsim.js>`_ . A camera is used in most of the following examples. Discussed in :ref:`Section 3.3 <c3.3>` .
    - `glut/ifs-polyhedron-viewer.c </../en/source/glut/ifs-polyhedron-viewer.c>`_ and `jogl/IFSPolyhedronViewer.java </../en/source/jogl/IFSPolyhedronViewer.java>`_ are C and Java versions of a program that lets the user view polyhedra that are defined as indexed face sets. The polyhedra models are defined in `jogl/Polyhedron.java </../en/source/jogl/Polyhedron.java>`_ for Java and in `glut/polyhedron.c </../en/source/glut/polyhedron.c>`_ and `glut/polyhedron.h </../en/source/glut/polyhedron.h>`_ for C. This program also requires the camera API discussed in the previous item. From :ref:`Section 3.4 <c3.4>`.
    - `glut/cubes-with-vertex-arrays.c </../en/source/glut/color-cube-of-spheres.c>`_,  `jogl/CubesWithVertexArrays.java </../en/source/jogl/ColorCubeOfSpheres.java>`_, and the JavaScript version glsim/cubes-with-vertex-arrays.html demonstrate drawing using glDrawArrays and glDrawElements. From :ref:`Section 3.4 <c3.4>`.
    - `glut/color-cube-of-spheres.c </../en/source/glut/glut-starter.c>`_ and `jogl/ColorCubeOfSpheres.java </../en/source/jogl/JoglStarter.java>`_ draw a large number of spheres using a variety of rendering methods, and show the time that it takes to render the image. The point is to compare render times for different rendering methods, including display lists, glDrawArrays, and vertex buffer objects. The reader is not expected to understand all of the code in this program. From :ref:`Section 3.4 <c3.4>`.
    - `glut/glut-starter.c </../en/source/glut/color-cube-of-spheres.c>`_,  `jogl/JoglStarter.java </../en/source/jogl/JoglStarter.java>`_, and `glsim/glsim-starter.html </../en/source/glsim/glsim-starter.html>`_ are "starter" files for writing OpenGL 1.1 applications using C, Java, and my JavaScript OpenGL simulator. These programs don't draw anything, but they have function/method stubs for drawing as well as for mouse and keyboard interaction and animation. Discussed in :ref:`Section 3.6 <c3.6>`
    - `glut/four-lights.c </../en/source/glut/four-lights.c>`_ and `jogl/FourLights.java </../en/source/jogl/FourLights.java>`_ are an example of using light sources and material properties. The program demonstrates multiple, moving light sources and lets the user turn the lights on and off to see the effect. The demo `glsim/fout-lights-demo.html </../en/demos/glsim/fout-lights-demo.html>`_ is a JavaScript version of the same program. From :ref:`Section 4.2 <c4.2>`.
    - `glut/texture-demo.c </../en/source/glut/texture-demo.c>`_ is a C program that shows a variety of textures on a variety of objects. It depends on the files `glut/textured-shapes.c </../en/source/glut/textured-shapes.c>`_ and `glut/textured-shapes.h </../en/source/glut/textured-shapes.h>`_, and on the folder `glut/textures </../en/source/glut/textures>`_ that contains the texture images used by the program. The Java version is `jogl/TextureDemo.java </../en/source/jogl/TextureDemo.java>`_, and it requires `jogl/TexturedShapes.java </../en/source/jogl/TexturedShapes.java>`_, as well as the image folder `jogl/textures </../en/source/jogl/textures>`_. From :ref:`Section 4.3 <c4.3>`.
    - `glut/texture-from-color-buffer.c </../en/source/glut/texture-from-color-buffer.c>`_ and `jogl/TextureFromColorBuffer.java </../en/source/jogl/TextureFromColorBuffer.java>`_ demonstrate the technique of copying an image from the color buffer using the function glCopyTexImage2D(). Draws an animated 2D scene and then uses it as a texture on various objects. Requires the same textured shape libraries mentioned in the previous item. From :ref:`Section 4.3 <c4.3>`.
    - `glut/texture-objects.c </../en/source/glut/texture-objects.c>`_ is a small program to demonstrate the use of texture objects to handle multiple textures. It is available for C only. From :ref:`Section 4.3 <c4.3>`.

5. Three.js 示例
------------------------

**5. Three.js Examples**

.. tab:: 中文

    Three.js 是一个用于网页上 3D 图形的 JavaScript 库，使用 WebGL 和 HTML 画布。它在 :ref:`c5` 中进行了讨论。示例可以在网站下载的源文件夹中找到，位于名为 `threejs </../en/source/threejs>`_ 的文件夹内。所有示例都使用 JavaScript 文件 `three.module.min.js </../en/source/threejs/script/three.module.min.js>`_，这是库的“压缩”版本，不适合人类阅读。也有一个适合人类阅读的版本， `three.module.js </../en/source/threejs/script/three.module.js>`_ 。示例还使用其他 three.js 脚本，可以在 threejs 文件夹内的 `script </../en/source/threejs/script/>`_ 文件夹中找到。版本是 three.js 版本 154。Three.js 是一个开源项目。它可以从 `threejs.org <http://threejs.org/>`_ 下载。

    - `threejs/full-window.html </../en/source/threejs/full-window.html>`_ — Three.js 通常用于编写填充浏览器窗口并持续运行动画的程序。这个示例展示了如何做到这一点，但我的其他示例没有遵循相同的模式。动画显示了有颜色的球在半透明盒子里弹跳。用户可以用鼠标旋转场景。来自 :ref:`c5.1`
    - `threejs/modeling-starter.html </../en/source/threejs/modeling-starter.html>`_ — 一个起始程序，用于尝试使用 three.js 构建和动画化场景图模型。用户可以使用键盘旋转模型。它包括一个简单的示例。来自 :ref:`c5.1`
    - `threejs/diskworld-1.html </../en/source/threejs/diskworld-1.html>`_ — 展示了一个简单的“汽车”在圆盘边缘上行驶的动画模型，以及由圆柱体和圆锥体制成的“树木”。基于之前的示例程序。来自 :ref:`c5.1`
    - `threejs/vertex-groups.html </../en/source/threejs/vertex-groups.html>`_ — 展示了如何在一个手工构建几何体的立方体和金字塔上使用材料数组。这使用了 **THREE.BufferedGeometry** 的“顶点组”特性。还有一个版本 `threejs/vertex-groups-indexed.html </../en/source/threejs/vertex-groups-indexed.html>`_ 使用索引面集模式表示金字塔。来自 :ref:`c5.2`
    - `threejs/textured-pyramid.html </../en/source/threejs/textured-pyramid.html>`_ — 展示了与前一个示例相同的金字塔，带有纹理。展示了如何为 three.js 几何体定义纹理坐标。来自 :ref:`c5.2`
    - `threejs/curves-and-surfaces.html </../en/source/threejs/curves-and-surfaces.html>`_ — 使用参数化表面、管状几何体、旋转和拉伸创建了几个表面。来自 :ref:`c5.2`
    - `threejs/model-viewer.html </../en/source/threejs/model-viewer.html>`_ — 显示使用 three.js 加载器从各种格式的文件加载的模型。模型来自 three.js 下载。（请参阅演示 `c5/mesh-animation.html </../en/demos/c5/mesh-animation.html>`_ 以查看两个模型的动画版本。）来自 :ref:`c5.2`
    - `threejs/instanced-mesh.html </../en/source/threejs/instanced-mesh.html>`_ — 使用 THREE.InstancedMesh 对象的一个小示例，可以绘制大量相同基本几何体的实例，每个副本具有不同的变换，并且可以为每种颜色选择不同的颜色。来自 :ref:`c5.3`
    - `threejs/skybox.html </../en/source/threejs/skybox.html>`_ — 演示使用立方体贴图制作天空盒。来自 :ref:`c5.3`
    - `threejs/reflection.html </../en/source/threejs/reflection.html>`_ — 使用环境贴图模拟对象反射其环境的演示。环境是一个天空盒。来自 :ref:`c5.3`
    - `threejs/refraction.html </../en/source/threejs/refraction.html>`_ — 模拟折射的演示。这个示例几乎与前一个示例相同，只是使用折射而不是反射。来自 :ref:`c5.3`


.. tab:: 英文

    Three.js is a JavaScript library for 3D graphics on Web pages, using WebGL and the HTML canvas. It is discussed in :ref:`Chapter 5 <c5>`. The examples can be found in the folder named `threejs </../en/source/threejs>`_, inside the source folder of the web site download. All of the examples use the JavaScript file `three.module.min.js </../en/source/threejs/script/three.module.min.js>`_, which is a "minified" version of the library, not meant for human readers. A human-readable version, `three.module.js </../en/source/threejs/script/three.module.js>`_ is also available. The examples also use other three.js scripts, which can be found in the `script </../en/source/threejs/script/>`_ folder inside the threejs folder. The version is three.js Release 154. Three.js is an open-source project. It can be downloaded from `threejs.org <http://threejs.org/>`_.

    - `threejs/full-window.html </../en/source/threejs/full-window.html>`_ — Three.js is typically used to write programs that fill the browser window and continually run an animation. This example shows how to do that, but my other examples do not follow the same pattern. The animation shows colored balls bouncing around inside a translucent box. The user can rotate the scene with the mouse. From :ref:`Section 5.1 <c5.1>`
    - `threejs/modeling-starter.html </../en/source/threejs/modeling-starter.html>`_ — A starter program for experimenting with building and animating a scene graph model with three.js. The user can rotate the model using the keyboard. It includes a simple example. From :ref:`Section 5.1 <c5.1>`
    - `threejs/diskworld-1.html </../en/source/threejs/diskworld-1.html>`_ — Shows an animated model of a simple "car" driving around the edge of a disk, with "trees" made from a cylinder and a cone. Based on the previous sample program. From :ref:`Section 5.1 <c5.1>`
    - `threejs/vertex-groups.html </../en/source/threejs/vertex-groups.html>`_ — Shows how to use an array of materials on a cube and on a pyramid whose geometry is constructed by hand. This uses the "vertex group" feature of **THREE.BufferedGeometry**. This is also a version `threejs/vertex-groups-indexed.html </../en/source/threejs/vertex-groups-indexed.html>`_ that represents the pyramid using the indexed face set pattern. From :ref:`Section 5.2 <c5.2>`
    - `threejs/textured-pyramid.html </../en/source/threejs/textured-pyramid.html>`_ — Shows the same pyramid as the previous example, with a texture. Shows how to define texture coordinates for a three.js geometry. From :ref:`Section 5.2 <c5.2>`
    - `threejs/curves-and-surfaces.html </../en/source/threejs/curves-and-surfaces.html>`_ — Creates several surfaces using a parametric surface, tube geometry, lathing, and extrusion. From :ref:`Section 5.2 <c5.2>`
    - `threejs/model-viewer.html </../en/source/threejs/model-viewer.html>`_ — Displays models that are loaded from files various formats, using three.js loaders. Models are from the three.js download. (See the demo `c5/mesh-animation.html </../en/demos/c5/mesh-animation.html>`_ to see animated versions of two of the models. From :ref:`Section 5.2 <c5.2>`
    - `threejs/instanced-mesh.html </../en/source/threejs/instanced-mesh.html>`_ — A small example of using a THREE.InstancedMesh object, which makes it possible to draw a large numbers of instances of the same basic geometry, with different transformations and, optionally, different colors for each copy. From :ref:`Section 5.3 <c5.3>`
    - `threejs/skybox.html </../en/source/threejs/skybox.html>`_ — Demonstrates using a cubemap texture to make a skybox. From :ref:`Section 5.3 <c5.3>`
    - `threejs/reflection.html </../en/source/three js/reflection.html>`_ — A demonstration of using an environment map to simulate the reflection by an object of its environment. The environment is a skybox. From :ref:`Section 5.3 <c5.3>`
    - `threejs/refraction.html </../en/source/threejs/refraction.html>`_ — A demonstration of simulated refraction. This example is almost identical to the previous example, except for using refraction rather than reflection. From :ref:`Section 5.3 <c5.3>`

6. WebGL 示例
------------------------

**6. WebGL Examples**

.. tab:: 中文

    WebGL 是用于网页上的 OpenGL 版本。它在 :ref:`c6` 和 :ref:`c7` 中进行了讨论。示例程序可以在名为 `webgl </../en/en/source/webgl>`_ 的文件夹中找到，该文件夹位于网站下载的*source*文件夹内。WebGL的示例程序是HTML文件。通过在Web浏览器中打开它们来运行程序。可以在文本编辑器中查看源代码，或者使用Web浏览器中的“查看源代码”命令。WebGL程序的一部分是用JavaScript编写的。另一部分由顶点着色器和片段着色器组成，这些着色器是用GLSL编写的。许多这些示例依赖于同一 `webgl </../en/en/source/webgl>`_ 目录中的脚本。特别是，3D示例使用了glMatrix库( :ref:`c7.1.1` )。这些程序中的大多数使用WebGL 1.0，但有一些需要WebGL 2.0，如文中所述。

    - `webgl/VAO-test-webgl2.html </../en/source/webgl/VAO-test-webgl2.html>`_ — 演示了顶点数组对象的使用。在 :ref:`c6.1.7` 中提到，但它使用了许多稍后在教科书中介绍的技术。这个程序需要WebGL 2.0。
    - `webgl/instancing-test-webgl2.html </../en/source/webgl/instancing-test-webgl2.html>`_ — 演示了使用gl.drawArraysInstanced()进行实例化绘制的使用。在 :ref:`c6.1.8` 中提到，但它使用的技术将在教科书的后面部分介绍。这个程序需要WebGL 2.0。
    - `webgl/webgl-rgb-triangle.html </../en/source/webgl/webgl-rgb-triangle.html>`_ — 使用WebGL渲染的标准OpenGL示例：一个顶点为红色、绿色和蓝色的三角形，内部像素的颜色通过插值顶点颜色来计算。演示了属性和变化变量的使用。来自 :ref:`c6.2` 。
    - `webgl/shape-stamper.html </../en/source/webgl/shape-stamper.html>`_ — 用户通过使用鼠标点击画布来“盖章”形状。形状的属性由一组弹出菜单确定。演示了统一变量的使用，WebGL上下文中的preserveDrawingBuffer选项，以及顶点着色器中的简单坐标变换。来自 :ref:`c6.2` 。
    - `webgl/moving-points.html </../en/source/webgl/moving-points.html>`_ — 一组圆形在画布中移动，碰到边缘时反弹。展示了如何在WebGL中使用POINTS原语，并介绍了片段着色器中的discard语句。来自 :ref:`c6.2` 。
    - `webgl/simple-texture.html </../en/source/webgl/simple-texture.html>`_ — 一个非常简单的纹理示例。它只是将纹理图像应用到一个三角形上。来自 :ref:`c6.4` 。
    - `webgl/texture-from-pixels.html </../en/source/webgl/texture-from-pixels.html>`_ — 展示了如何从一个数组中加载纹理，该数组包含纹理的像素颜色分量值。（还演示了gl.LINEAR和gl.NEAREST放大过滤器之间的区别。）来自 :ref:`c6.4` 。
    - `webgl/cubemap-fisheye.html </../en/source/webgl/cubemap-fisheye.html>`_ — 加载一个立方体贴图，但在2D上下文中使用它来模仿用鱼眼镜头拍摄的照片。2D纹理坐标首先映射到一个球体上，以获取用于采样立方贴图的方向向量。来自 :ref:`c6.4` 。
    - `webgl/webgl-game-of-life.html </../en/source/webgl/webgl-game-of-life.html>`_ — John H. Conway的“生命游戏”在WebGL中的实现，作为一个基本示例，展示了如何使用GPU执行计算任务。来自 :ref:`c6.4`。
    - `webgl/texelFetch-MonaLisa-webgl2.html </../en/source/webgl/texelFetch-MonaLisa-webgl2.html>`_ — 一个相当愚蠢的演示程序，使用GLSL ES 3.00函数texelFetch()从纹理图像中获取颜色。这个程序需要WebGL 2.0。来自 :ref:`c6.4` 。
    - `webgl/simple-hierarchy2D.html </../en/source/webgl/simple-hierarchy2D.html>`_ — 演示了在WebGL和GLSL中使用2D建模变换，以及一些简单的动画层次对象。变换在JavaScript中实现为**AffineTransform2D**类型的对象，定义在文件webgl/AffineTransform2D.js中。来自 :ref:`c6.5` 。
    - `webgl/glmatrix-cube-unlit.html </../en/source/webgl/glmatrix-cube-unlit.html>`_ — 第一个直接在WebGL中进行3D图形处理的示例，没有照明。来自 :ref:`c7.1`。
    - `webgl/cube-with-simple-rotator.html </../en/source/webgl/cube-with-trackball-rotator.html>`_ — 演示了使用 **SimpleRotator** （在 `webgl/simple-rotator.js </../en/source/webgl/simple-rotator.js>`_ 中定义）进行鼠标旋转的使用。来自 :ref:`c7.1` 。
    - `webgl/cube-with-trackball-rotator.html </../en/source/webgl/cube-with-trackball-rotator.html>`_ — 演示了使用 **TrackballRotator** （在 `webgl/trackball-rotator.js </../en/source/webgl/trackball-rotator.js>`_ 中定义）进行鼠标旋转的使用。这几乎与前一个示例相同。来自 :ref:`c7.1` 。
    - `webgl/cube-with-basic-lighting.html </../en/source/webgl/cube-with-basic-lighting.html>`_ — 第一个在WebGL中直接实现照明的示例。为 `webgl/glmatrix-cube-unlit.html </../en/source/webgl/glmatrix-cube-unlit.html>`_ 添加了照明。在这种情况下，照明仅使用漫反射颜色和来自观察者方向的方向光。来自 :ref:`c7.2`。
    - `webgl/basic-specular-lighting.html </../en/source/webgl/basic-specular-lighting.html>`_ — 第一个实现镜面反射的示例。来自 :ref:`c7.2` 。
    - `webgl/basic-specular-lighting-Phong.html </../en/source/webgl/basic-specular-lighting-Phong.html>`_ — 使用Phong着色（在片段着色器中进行照明计算）的第二个镜面反射实现。除了将计算移动到片段着色器外，这个示例与前一个示例相同。来自 :ref:`c7.2` 。还有一个移植到WebGL 2.0和GLSL ES 3.00的版本： `webgl/basic-specular-lighting-Phong-webgl2.html </../en/source/webgl/basic-specular-lighting-Phong-webgl2.html>`_ 。所需的更改非常少。
    - `webgl/parametric-function-grapher.html </../en/source/webgl/parametric-function-grapher.html>`_ — 允许用户根据用户输入的方程x(u,v)，y(u,v)和z(u,v)绘制参数曲面。这是一个相对复杂的程序，它展示了GLSL数据结构、双面照明和多边形偏移。来自 :ref:`c7.2`。
    - `webgl/spotlights.html </../en/source/webgl/spotlights.html>`_ — 聚光灯的演示，有三个彩色聚光灯。用户可以更改截止角度和聚光指数。来自 :ref:`c7.2`。
    - `webgl/diskworld-2.html </../en/source/webgl/diskworld-2.html>`_ — 一个相对复杂的程序，具有层次建模和几种类型的照明，包括移动灯、聚光灯和光衰减。这与three.js示例 `threejs/diskworld-1.html </../en/source/threejs/diskworld-1.html>`_ 相同，增加了照明特性。来自 :ref:`c7.2`。
    - `webgl/texture-transform.html </../en/source/webgl/texture-transform.html>`_ — 使用glMatrix实现纹理变换的动画纹理图像。来自 :ref:`c7.3`


.. tab:: 英文

    WebGL is the version of OpenGL for use on Web pages. It is discussed in `Chapter 6 <c6>` and `Chapter 7 <c7>`. The sample programs can be found in a folder named `webgl </../en/en/source/webgl>`_, inside the *source* folder of the web site download. The sample programs for WebGL are HTML files. Run the programs by opening them in a Web browser. View the source code in a text editor or using a "View Source" command in a web browser. Part of a WebGL program is written in JavaScript. The other part consists of a vertex shader and a fragment shader written in GLSL. Many of these examples rely on scripts that are in the same `webgl </../en/en/source/webgl>`_ directory. In particular, the 3D examples use the glMatrix library ( :ref:`Subsection 7.1.1 <c7.1.1>` ). Most of these programs work with WebGL 1.0, but a few require WebGL 2.0, as noted.

    - `webgl/VAO-test-webgl2.html </../en/source/webgl/VAO-test-webgl2.html>`_ — Demonstrates the use of Vertex Array Objects. Mentioned in `Subsection 6.1.7 <c6.1.7>`, but it uses many techniques that will be covered later in the textbook. This program requires WebGL 2.0.
    - `webgl/instancing-test-webgl2.html </../en/source/webgl/instancing-test-webgl2.html>`_ — Demonstrates the use of instanced drawing with gl.drawArraysInstanced(). Mentioned in `Subsection 6.1.8 <c6.1.8>`, but it uses techniques that will be covered later in the textbook. This program requires WebGL 2.0
    - `webgl/webgl-rgb-triangle.html </../en/source/webgl/webgl-rgb-triangle.html>`_ — The standard OpenGL example rendered using WebGL: a triangle whose vertices are red, green, and blue, where the colors of interior pixels are computed by interpolating colors from the vertices. Demonstrates the use of attributes and varying variables. From :ref:`Section 6.2 <c6.2>`
    - `webgl/shape-stamper.html </../en/source/webgl/shape-stamper.html>`_ — The user "stamps" shapes onto the canvas by clicking it with the mouse. Properties of the shape are determined by a set of pop-up menus. Demonstrates the use of uniform variables, the preserveDrawingBuffer option on the WebGL context, and a simple coordinate transformation in the vertex shader. From :ref:`Section 6.2 <c6.2>`
    - `webgl/moving-points.html </../en/source/webgl/moving-points.html>`_ — A set of circles moves around in the canvas, bouncing off the edges. Shows how to use the POINTS primitive in WebGL and introduces the discard statement in the fragment shader. From :ref:`Section 6.2 <c6.2>`
    - `webgl/simple-texture.html </../en/source/webgl/simple-texture.html>`_ — A very minimal texture example. It just applies a texture image to a triangle. From :ref:`Section 6.4 <c6.4>` .
    - `webgl/texture-from-pixels.html </../en/source/webgl/texture-from-pixels.html>`_ — Shows how to load a texture from an array that contains the pixel color component values for the texture. (Also demonstrates the difference between a gl.LINEAR and a gl.NEAREST magnification filter.) From :ref:`Section 6.4 <c6.4>`.
    - `webgl/cubemap-fisheye.html </../en/source/webgl/cubemap-fisheye.html>`_ — Loads a cubemap texture, but uses it in a 2D context to imitate a picture taken with a fisheye lens. 2D texture coordinates are first mapped onto a sphere to get the direction vector that is used to sample the cubemap. From :ref:`Section 6.4 <c6.4>`.
    - `webgl/webgl-game-of-life.html </../en/source/webgl/webgl-game-of-life.html>`_ — An implementation of John H. Conway's "Game of Live" in WebGL, as a basic example of how GPUs can be used to perform computational tasks. From :ref:`Section 6.4 <c6.4>`.
    - `webgl/texelFetch-MonaLisa-webgl2.html </../en/source/webgl/texelFetch-MonaLisa-webgl2.html>`_ — A rather silly demo program that uses the GLSL ES 3.00 function texelFetch() to get colors from a texture image. This program requires WebGL 2.0. From :ref:`Section 6.4 <c6.4>`.
    - `webgl/simple-hierarchy2D.html </../en/source/webgl/simple-hierarchy2D.html>`_ — Demonstrates using 2D modeling transformations in WebGL and GLSL, with some simple animated hierarchical objects. Transforms are implemented in JavaScript as objects of type **AffineTransform2D**, defined in the file webgl/AffineTransform2D.js. From :ref:`Section 6.5 <c6.5>` .
    - `webgl/glmatrix-cube-unlit.html </../en/source/webgl/glmatrix-cube-unlit.html>`_ — A first example of doing 3D graphics directly in WebGL, with no lighting. From :ref:`Section 7.1 <c7.1>`.
    - `webgl/cube-with-simple-rotator.html </../en/source/webgl/cube-with-trackball-rotator.html>`_  — Demonstrates the use of a **SimpleRotator** (defined in `webgl/simple-rotator.js </../en/source/webgl/simple-rotator.js>`_ ) to do mouse rotation. From :ref:`Section 7.1 <c7.1>` .
    - `webgl/cube-with-trackball-rotator.html </../en/source/webgl/cube-with-trackball-rotator.html>`_ — Demonstrates the use of a **TrackballRotator** (defined in `webgl/trackball-rotator.js </../en/source/webgl/trackball-rotator.js>`_ ) to do mouse rotation. This is almost identical to the previous example. From :ref:`Section 7.1 <c7.1>`.
    - `webgl/cube-with-basic-lighting.html </../en/source/webgl/cube-with-basic-lighting.html>`_ — A first example of implementing lighting directly in WebGL. Adds lighting to `webgl/glmatrix-cube-unlit.html </../en/source/webgl/glmatrix-cube-unlit.html>`_ . The lighting in this case uses only diffuse color and a directional light from the direction of the viewer. From :ref:`Section 7.2 <c7.2>` .
    - `webgl/basic-specular-lighting.html </../en/source/webgl/basic-specular-lighting.html>`_ — A first implementation of specular reflection. From :ref:`Section 7.2 <c7.2>`.
    - `webgl/basic-specular-lighting-Phong.html </../en/source/webgl/basic-specular-lighting-Phong.html>`_ — A second implementation of specular reflection, using Phong shading (with the lighting calculations in the fragment shader). Aside from moving the calculation to the fragment shader, this example is identical to the previous example. From :ref:`Section 7.2 <c7.2>` . There is also a version that has been ported to WebGL 2.0 and GLSL ES 3.00: `webgl/basic-specular-lighting-Phong-webgl2.html </../en/source/webgl/basic-specular-lighting-Phong-webgl2.html>`_ . The required changes are minimal.
    - `webgl/parametric-function-grapher.html </../en/source/webgl/parametric-function-grapher.html>`_ — Lets the user graph a parametric surface, given by equations x(u,v), y(u,v), and z(u,v) entered by the user. A relatively complex program, it illustrates GLSL data structures, two-sided lighting, and polygon offset. From :ref:`Section 7.2 <c7.2>`.
    - `webgl/spotlights.html </../en/source/webgl/spotlights.html>`_ — A demo of spotlights, with three colored spotlights. The user can change the cutoff angle and spot exponent. From :ref:`Section 7.2 <c7.2>`
    - `webgl/diskworld-2.html </../en/source/webgl/diskworld-2.html>`_— A relatively complex program with hierarchical modeling and several kinds of lighting, including moving lights, spotlights, and light attenuation. This is the same scene as the three.js example `threejs/diskworld-1.html </../en/source/threejs/diskworld-1.html>`_ , with added lighting features. From :ref:`Section 7.2 <c7.2>`.
    - `webgl/texture-transform.html </../en/source/webgl/texture-transform.html>`_ — Animated texture images, using glMatrix to implement texture transformations. From :ref:`Section 7.3 <c7.3>`.
    - `webgl/bumpmap.html </../en/source/webgl/bumpmap.html>`_ — A mostly successful attempt to implement bumpmapping. From :ref:`Section 7.3 <c7.3>`.
    - `webgl/skybox-and-env-map.html </../en/source/webgl/skybox-and-env-map.html>`_ — Uses a cubemap texture to make a skybox and as an environment map. From :ref:`Section 7.3 <c7.3>`.
    - `webgl/image-blur.html </../en/source/webgl/image-blur.html>`_ — Applies a blur filter to an image. A very simple demo of using blending for something other than transparency. Also a very simple example of a multi-pass algorithm. From :ref:`Section 7.4 <c7.4>`.
    - `webgl/render-to-texture.html </../en/source/webgl/render-to-texture.html>`_ — Uses a WebGL framebuffer to draw an image directly into a texture. From :ref:`Section 7.4 <c7.4>`. There is also a port to WebGL 2.0, which uses vertex array objects and gl.texStorage2D(): `webgl/render-to-texture-webgl2.html </../en/source/webgl/render-to-texture-webgl2.html>`_.
    - `webgl/cube-camera.html </../en/source/webgl/cube-camera.html>`_ — Shows a skybox and moving cubes reflected on the surface of an object. Uses a dynamic cubemap texture as an environment map on the reflective object. The six images for the cubemap texture are redrawn for each frame of an animation. From :ref:`Section 7.4 <c7.4>`.
    - `webgl/anisotropic-filtering.html </../en/source/webgl/anisotropic-filtering.html>`_ — Demonstrates the use of the WebGL anisotropic filtering extension. Shows a large textured rectangle extending into the distance and lets the user turn anisotropic filtering on and off. From :ref:`Section 7.5 <c7.5>`.
    - `webgl/image-evolver.html </../en/source/webgl/image-evolver.html>`_ — Demonstrates use of the WEBGL_color_buffer_float WebGL extension. The application is a simple genetic algorithm that tries to approximate a given image. The floating point color buffer is used for two computations: finding the average of the color values in an image and computing an image that represents the difference between two images. From :ref:`Section 7.5 <c7.5>`.
    - `webgl/instancing-test-webgl1.html </../en/source/webgl/instancing-test-webgl1.html>`_ — Demonstrates the use of an extension to do instanced drawing in WebGL 1.0. This is a copy of `webgl/instancing-test-webgl2.html </../en/source/webgl/instancing-test-webgl2.html>`_, modified to work with WebGL 1.0. From :ref:`Section 7.5 <c7.5>`.
    - `webgl/multiple-draw-buffers-webgl2.html </../en/source/webgl/multiple-draw-buffers-webgl2.html>`_ — Demonstrates drawing to multiple textures attached as draw buffers to the same framebuffer. Requires WebGL 2.0 (but something similar could be done in WebGL 1.0 with an extension.) From :ref:`Section 7.5 <c7.5>`.


7. WebGPU 示例
------------------------

**7. WebGPU Examples**

.. tab:: 中文

    WebGPU 是 Web 上的全新图形 API。它从头开始设计，以整合更现代 API 的一些特性，如 Vulkan、Direct3D 和 Metal。它在 :ref:`c9` 中被介绍。这些程序需要支持 WebGPU 的网络浏览器。截至2023年7月，WebGPU 在 Windows 和 MacOS 上的 Chrome 和 Edge 浏览器中默认启用。在其他一些浏览器中，它是用户可以启用的实验性功能。在网站的下载中，它们可以在源目录中名为 `webgpu </../en/en/source/webgpu/>`_ 的目录中找到。一些示例使用 *wgpu-matrix*  ( :ref:`c9.4.4` ) 以及同一目录中可以找到的其他脚本和资源。

    - `webgpu/basic_webgpu_1.html </../en/source/webgpu/basic_webgpu_1.html>`_ — 一个 WebGPU 的首个示例，它仅绘制一个彩色的三角形。源代码有大量的注释来解释 WebGPU。来自 :ref:`c9.1`。
    - `webgpu/basic_webgpu_2.html </../en/source/webgpu/basic_webgpu_2.html>`_ 和 `webgpu/basic_webgpu_3.html </../en/source/webgpu/basic_webgpu_3.html>`_ — 前一个示例的变化，绘制具有不同颜色顶点的三角形。这需要向顶点着色器程序添加第二个参数。第一个程序通过使用两个顶点缓冲区来实现这一点；第二个程序通过使用一个具有两个输入参数交错值的单一顶点缓冲区来实现。来自 :ref:`c9.1.6` 。
    - `webgpu/instanced_draw.html </../en/source/webgpu/instanced_draw.html>`_ — 使用实例化绘制通过单个 draw() 调用绘制多个彩色圆盘。展示了如何在顶点缓冲区中使用实例属性。来自 :ref:`c9.2.1` 。
    - `webgpu/indexed_draw.html </../en/source/webgpu/indexed_draw.html>`_ — 使用 drawIndexed() 方法使用三角形列表原语绘制单个圆盘作为索引面集合。还使用三角形条带原语绘制圆盘轮廓，并展示了如何在命令缓冲区中使用两个渲染通道。来自 :ref:`c9.2.2` 。
    - `webgpu/draw_multiple.html </../en/source/webgpu/draw_multiple.html>`_ — 使用不同的渲染通道绘制多个轮廓圆盘。还展示了使用 copyBufferToBuffer() 在渲染通道之间设置统一变量的值。另外， `webgpu/draw_multiple_2.html </../en/source/webgpu/draw_multiple_2.html>`_ 是程序的一个变化，它使用 writeBuffer() 做同样的事情，这需要为每个圆盘绘制单独的命令编码器。来自 :ref:`c9.2.3` 。
    - `webgpu/indices_in_shader.html </../en/source/webgpu/indices_in_shader.html>`_ — 一个使用顶点索引和实例索引在顶点着色器函数中的示例。在这种情况下的应用是通过设置点大小来模仿在 WebGL 中可以使用 POINTS 原语完成的事情。WebGPU 没有实现点大小，所以点列表原语只能作为单个像素渲染。来自 :ref:`c9.2.4` 。
    - `webgpu/multisampling.html </../en/source/webgpu/multisampling.html>`_ — 通过将其添加到 `webgpu/instanced_draw.html </../en/source/webgpu/instanced_draw.html>`_ 来演示如何在 WebGPU 程序中添加多重采样，多重采样是一种抗锯齿。来自 :ref:`c9.2.5` 。
    - `webgpu/depth_test.html </../en/source/webgpu/depth_test.html>`_ — 展示了如何在 WebGPU 中启用深度测试。该程序复制了 `webgpu/draw_multiple.html </../en/source/webgpu/draw_multiple.html>`_ 的功能，但是使用实例化绘制来完成。它还添加了多重采样。但是代码中唯一的注释是关于深度测试的。来自 :ref:`c9.4.1` 。
    - `webgpu/Phong_lighting.html </../en/source/webgpu/Phong_lighting.html>`_ — 将 `webgl/basic-specular-lighting-Phong.html </../en/source/webgl/basic-specular-lighting-Phong.html>`_ 直接移植到 WebGPU。它一次显示一个对象，用户可以控制材料和光属性。来自 :ref:`c9.4.2` 。
    - `webgpu/diskworld_webgpu.html </../en/source/webgpu/diskworld_webgpu.html>`_ — 将 `webgl/diskworld-2.html </../en/source/webgl/diskworld-2.html>`_ 直接移植到 WebGPU。它是实现分层 3D 图形和 OpenGL 照明模型的一个示例。来自 :ref:`c9.4.5` 。
    - `webgpu/first_texture.html </../en/source/webgpu/first_texture.html>`_ — WebGPU 中使用纹理的首个示例。用户可以在三种不同的纹理之间进行选择，应用于一个正方形。来自 :ref:`c9.5` 。
    - `webgpu/textured_objects.html </../en/source/webgpu/textured_objects.html>`_ — 将纹理图像应用于 3D 形状，并具有基本照明。来自 :ref:`c9.5` 。
    - `webgpu/texture_from_canvas.html </../en/source/webgpu/texture_from_canvas.html>`_ — 从同一页面上的另一个画布中获取纹理图像，并将其应用于 3D 形状。用户可以在画布上进行一些非常简单的绘图。（除了从画布中获取纹理外，这个程序中没有新内容。）来自 :ref:`c9.5` 。
    - `webgpu/making_mipmaps.html </../en/source/webgpu/making_mipmaps.html>`_ — 定义并测试一个函数，该函数从 ImageBitmap 创建一个带有完整一组 mipmap 的图像纹理。来自 :ref:`c9.5.3` 。
    - `webgpu/cubemap_texture.html </../en/source/webgpu/cubemap_texture.html>`_ — 加载一个立方体贴图，并将其用于天空盒和反射映射。它在功能上与 WebGL 示例 `webgl/skybox-and-env-map.html </../en/source/webgl/skybox-and-env-map.html>`_ 相同。来自 :ref:`c9.5.4` 。
    - `webgpu/life_1.html </../en/source/webgpu/life_1.html>`_ — Conway的“生命游戏”，使用整数格式“r32uint”纹理和 WGSL 函数 textureLoad() 和 textureStore()。程序 `webgpu/life_2.html </../en/source/webgpu/life_2.html>`_ 执行相同的任务，但使用两个“r8unorm”纹理，一个用于着色器中的采样，一个用作渲染管线的颜色附件。来自 :ref:`c9.5.5`。
    - `webgpu/diffusion.html </../en/source/webgpu/diffusion.html>`_ — 使用计算着色器运行布朗运动的模拟。白色粒子随机移动。当它们击中黄色或青色粒子时，它们会改变颜色并停止移动。随着时间的推移，会形成有趣的类似树枝的图案。来自 :ref:`c9.6.3` 。
    - `webgpu/map_buffer_for_read.html </../en/source/webgpu/map_buffer_for_read.html>`_ — 展示了如何将数据从 GPU 缓冲区读取到程序的 JavaScript 端。应用程序（实际上并不是练习的重点）是使用梯形规则来近似定积分。来自 :ref:`c9.6.4`。
    - `webgpu/viewport_and_scissor.html </../en/source/webgpu/viewport_and_scissor.html>`_ — 另一个移动圆盘动画，展示了在不同视口中的四个场景副本。在两个视口中还应用了裁剪矩形。来自 :ref:`c9.7.4` 。
    - `webgpu/alpha_blend.html </../en/source/webgpu/alpha_blend.html>`_ — 使用 alpha 混合绘制半透明颜色。展示了渲染管线中目标的混合属性。来自 :ref:`c9.7.5` 。
    - `webgpu/color_mask.html </../en/source/webgpu/color_mask.html>`_ — 通过让用户选择要写入的颜色通道，演示了渲染管线中目标的 writeMask 属性。来自:ref:`c9.7.5` 。
    - `webgpu/polyhedra.html </../en/source/webgpu/polyhedra.html>`_ — 允许用户查看几种多面体。通过在渲染管线中使用深度偏置绘制多面体的面，以确保边缘的部分不会被面遮挡，演示了深度偏置。同时使用面裁剪。来自 :ref:`c9.7.5` 。



.. tab:: 英文

    WebGPU is a new API for graphics on the Web. It has been designed from scratch to incorporate some of the features of more modern APIs such as Vulkan, Direct3D, and Metal. It is covered in :ref:`Chapter 9 <c9>`. These programs require a web browser that supports WebGPU. As of July, 2023, WebGPU is enabled by default in the Chrome and Edge browsers on Windows and MacOS. In some other browsers, it is an experimental feature that can be enabled by the user. In a download of the web site, they can be found in the directory named `webgpu </../en/en/source/webgpu/>`_ in the source directory. Some of the examples use *wgpu-matrix* ( :ref:`Subsection 9.4.4 <c9.4.4>` ) and other scripts and resources that can be found in the same directory

    - `webgpu/basic_webgpu_1.html </../en/source/webgpu/basic_webgpu_1.html>`_ — A first WebGPU example, which just draws a colored triangle. The source code has extensive comments to explain WebGPU. From :ref:`Section 9.1 <c9.1>`.
    - `webgpu/basic_webgpu_2.html </../en/source/webgpu/basic_webgpu_2.html>`_ and `webgpu/basic_webgpu_3.html </../en/source/webgpu/basic_webgpu_3.html>`_ — Variations on the previous example that draw a triangle with different colored vertices. This requires adding a second parameter to the vertex shader program. The first program does this by using two vertex buffers; the second, by using a single vertex buffer with interleaved values for the two input parameters. From :ref:`Section 9.1.6 <c9.1.6>`.
    - `webgpu/instanced_draw.html </../en/source/webgpu/instanced_draw.html>`_ — Uses instanced drawing to draw multiple colored disks using a single call to draw(). Shows how to use instance attributes in vertex buffers. From :ref:`Section 9.2.1 <c9.2.1>`.
    - `webgpu/indexed_draw.html </../en/source/webgpu/indexed_draw.html>`_ — Uses the drawIndexed() method to draw a single disk as an indexed face set using a triangle-list primitive. Also draws the disk outline using a triangle-strip primitive and shows how to use two render passes in one command buffer. From :ref:`Section 9.2.2 <c9.2.2>`.
    - `webgpu/draw_multiple.html </../en/source/webgpu/draw_multiple.html>`_ — Draws multiple outlined disks using different rendering passes for each disk. Also illustrates using copyBufferToBuffer() to set the value of a uniform variable between rendering passes. Also, `webgpu/draw_multiple_2.html </../en/source/webgpu/draw_multiple_2.html>`_ is a variation on the program that does the same thing using writeBuffer(), which requires a separate command encoder for drawing each disk. From :ref:`Section 9.2.3 <c9.2.3>`.
    - `webgpu/indices_in_shader.html </../en/source/webgpu/indices_in_shader.html>`_ — An example of using the vertex index and the instance index in the vertex shader function. The application in this case is to imitate what can be done in WebGL with a POINTS primitive by setting a point size. WebGPU does not implement point size, so a points-list primitive can only be rendered as individual pixels. From :ref:`Section 9.2.4 <c9.2.4>`.
    - `webgpu/multisampling.html </../en/source/webgpu/multisampling.html>`_  — Demonstrates how to add multisampling to a WebGPU program, by adding it to `webgpu/instanced_draw.html </../en/source/webgpu/instanced_draw.html>`_ . Multisampling is a kind of antialiasing. From :ref:`Section 9.2.5 <c9.2.5>` .
    - `webgpu/depth_test.html </../en/source/webgpu/depth_test.html>`_ — Shows how to enable the depth test in WebGPU. The program duplicates the functionality of `webgpu/draw_multiple.html </../en/source/webgpu/draw_multiple.html>`_ but does it with instanced drawing. It also adds multisampling. But the only comments in the code are about the depth test. From :ref:`Section 9.4.1 <c9.4.1>`
    - `webgpu/Phong_lighting.html </../en/source/webgpu/Phong_lighting.html>`_ — A direct port of `webgl/basic-specular-lighting-Phong.html </../en/source/webgl/basic-specular-lighting-Phong.html>`_ to WebGPU. It displays one object at a time, with some user control of material and light properties. From :ref:`Section 9.4.2 <c9.4.2>`
    - `webgpu/diskworld_webgpu.html </../en/source/webgpu/diskworld_webgpu.html>`_ — A direct port of `webgl/diskworld-2.html </../en/source/webgl/diskworld-2.html>`_ to WebGPU. It is an example of the implementation of hierarchical 3D graphics and of the OpenGL lighting model. From :ref:`Section 9.4.5 <c9.4.5>`
    - `webgpu/first_texture.html </../en/source/webgpu/first_texture.html>`_ — A first example of using textures in WebGPU. The user can select among three different kinds of texture, applied to a square. From :ref:`Section 9.5 <c9.5>`.
    - `webgpu/textured_objects.html </../en/source/webgpu/textured_objects.html>`_ — Applies texture images to 3D shapes, with basic lighting. From :ref:`Section 9.5 <c9.5>`.
    - `webgpu/texture_from_canvas.html </../en/source/webgpu/texture_from_canvas.html>`_ — Takes the image for a texture from another canvas on the same page and applies it to 3D shapes. The user can do some very simple drawing on the canvas. (Aside from grabbing the texture from a canvas, there is nothing new in this program.) From :ref:`Section 9.5 <c9.5>`.
    - `webgpu/making_mipmaps.html </../en/source/webgpu/making_mipmaps.html>`_ — Defines and tests a function that creates an image texture with a full set of mipmaps from an ImageBitmap. From :ref:`Section 9.5.3 <c9.5.3>`.
    - `webgpu/cubemap_texture.html </../en/source/webgpu/cubemap_texture.html>`_ — Loads a cubemap texture and uses it for a skybox and for reflection mapping. It is functionally identical to the WebGL example `webgl/skybox-and-env-map.html </../en/source/webgl/skybox-and-env-map.html>`_. From :ref:`Section 9.5.4 <c9.5.4>`.
    - `webgpu/life_1.html </../en/source/webgpu/life_1.html>`_ — Conway's "Game of Life", using integer-format "r32uint" textures and the WGSL functions textureLoad() and textureStore(). The program `webgpu/life_2.html </../en/source/webgpu/life_2.html>`_ performs the same task, but does it using two "r8unorm" textures, one used for sampling in the shader and one used as a color attachment for the render pipeline. From :ref:`Section 9.5.5 <c9.5.5>` .
    - `webgpu/diffusion.html </../en/source/webgpu/diffusion.html>`_ — Uses compute shaders to run a simulation of Brownian motion. White particles move randomly. When they hit a yellow or cyan particle, they change color and stop moving. Over time, an interesting dendrite-like pattern will form. From :ref:`Section 9.6.3 <c9.6.3>` .
    - `webgpu/map_buffer_for_read.html </../en/source/webgpu/map_buffer_for_read.html>`_ — Illustrates reading data from a GPU buffer into the JavaScript side of the program. The application (which is really not the point of the exercise) is to use the trapezoid rule to approximate a definite integral. From :ref:`Section 9.6.4 <c9.6.4>` .
    - `webgpu/viewport_and_scissor.html </../en/source/webgpu/viewport_and_scissor.html>`_ — Another moving disk animation, showing four copies of the scene in different viewports. A scissor rect is also applied in two of the viewports. From :ref:`Section 9.7.4 <c9.7.4>` .
    - `webgpu/alpha_blend.html </../en/source/webgpu/alpha_blend.html>`_ — Uses alpha blending to draw translucent colors. Demonstrates the blend property of the target in a render pipeline. From :ref:`Section 9.7.5 <c9.7.5>`.
    - `webgpu/color_mask.html </../en/source/webgpu/color_mask.html>`_ — Demonstrates the writeMask property of the target in a render pipeline by letting the user select which color channels to write. From :ref:`Section 9.7.5 <c9.7.5>`.
    - `webgpu/polyhedra.html </../en/source/webgpu/polyhedra.html>`_ — Lets the user view several polyhedra. Demonstrates depth bias in a render pipeline by drawing the faces of the polyhedra with a depth bias, to make sure that parts of the edges are not hidden by the faces. Also uses face culling. From :ref:`Section 9.7.5 <c9.7.5>`.

8. 实时演示
------------------------

**8. Live Demos**

.. tab:: 中文

    这本书包括嵌入在网页中的“实时”或“交互式”演示。这些演示是使用 JavaScript 和 HTML 画布图形或 WebGL 编写的小程序。尽管它们被设计为在其他网页内作为小型应用程序运行，但它们也可以作为独立的网页运行。在这本书的网站下载中，你可以在按章节编号组织的 demos 文件夹中找到演示。它们可以直接从该文件夹运行。请注意，每个演示都需要演示文件夹中包含的某些其他文件；如果你将演示复制到另一个位置，请确保也复制它所依赖的所有文件。

    :ref:`c2` 的演示使用 2D 画布图形 API，它将在几乎所有现代网络浏览器中工作。第3章到第8章的演示使用 WebGL，这也将在几乎所有现代网络浏览器中工作。（然而，在某些机器上的一些浏览器中，WebGL 可能仍然存在问题。）所有使用 WebGL 的演示程序都将与 WebGL 1.0 兼容。第9章的演示需要支持 WebGPU 的网络浏览器。

    :ref:`c3` 和 :ref:`c4` 的演示使用 `glsim.js </../en/source/glsim/glsim.js>`_ ，一个我编写的 JavaScript 库，用于模拟 OpenGL 1.1 的一个子集。关于 glsim 的信息可以在 `glsim/glsim-doc.html </../en/source/glsim/glsim-doc.html>`_ 中找到。

    对于许多演示，读者在书中演示出现的点上并不期望理解演示的程序代码。请注意，演示中的 JavaScipt 代码尚未更新为在 :ref:`a.3` 中介绍的更现代的 JavaSctipt 版本。

    - `c2/pixel-magnifier.html </../en/demos/c2/pixel-magnifier.html>`_ — 来自 :ref:`c2.1` 。放大图像中的一个小像素正方形，以便用户可以看到文本、线条和其他形状是如何由像素构成的，包括抗锯齿。
    - `c2/rgb-hsv.html </../en/demos/c2/rgb-hsv.html>`_ — 来自 :ref:`c2.1` 。让用户通过拖动滑块在 RGB 和 HSV 颜色空间中修改颜色。
    - `c2/approximating-ovals.html </../en/demos/c2/approximating-ovals.html>`_ — 来自 :ref:`c2.2` 。展示了如何通过不同边数的多边形来近似椭圆形。
    - `c2/cubic-bezier.html </../en/demos/c2/cubic-bezier.html>`_ — 来自 :ref:`c2.2` 。让用户通过拖动端点和控制点来修改三次贝塞尔曲线。
    - `c2/quadratic-bezier.html </../en/demos/c2/quadratic-bezier.html>`_ — 来自 :ref:`c2.2` 。让用户通过拖动端点和控制点来修改二次贝塞尔曲线。
    - `c2/transforms-2d.html </../en/demos/c2/transforms-2d.html>`_ — 来自 :ref:`c2.3` 。让用户对形状应用一系列旋转、缩放和平移变换，并查看结果。
    - `c2/transform-equivalence-2d.html </../en/demos/c2/transform-equivalence-2d.html>`_ — 来自 :ref:`c2.4` 。尝试演示 2D 中建模变换和视口变换的等价性。
    - `c2/cart-and-windmills.html </../en/demos/c2/cart-and-windmills.html>`_ — 来自 :ref:`c2.4` 。展示了一个使用分层建模构建的简单、动画化的 2D 场景。
    - `c2/SimplePaintDemo.html </../en/demos/c2/SimplePaintDemo.html>`_ — 来自 :ref:`c2.6` 。让用户使用一些基本形状在画布上绘图。"Smudge" 工具展示了像素操作。这个演示与示例程序 `canvas2d/SimplePaintProgram.html </../en/source/canvas2d/SimplePaintProgram.html>`_ 几乎相同。
    - `c2/image-filters.html </../en/demos/c2/image-filters.html>`_ — 来自 :ref:`c2.6` 。让用户对几张图片应用各种“滤镜”。在这里使用的“滤镜”一词，是指用该像素及其八个邻居的颜色加权平均值替换每个像素的颜色。
    - `c3/first-triangle-demo.html </../en/demos/c3/first-triangle-demo.html>`_ — 来自 :ref:`c3.1` 。展示了 OpenGL 的常见第一个示例：一个顶点颜色不同的三角形。在这个演示中，你可以改变顶点的颜色。
    - `c3/first-cube.html </../en/demos/c3/first-cube.html>`_ — 来自 :ref:`c3.1` 。绘制一个立方体，六个面有不同的颜色（没有照明效果，并使用默认的正交投影）。用户可以开启和关闭深度测试以查看效果。用户可以使用更大的立方体，以查看当立方体的部分超出 z 值可见范围时“裁剪”的效果。
    - `c3/axes3D.html </../en/demos/c3/axes3D.html>`_ — 来自 :ref:`c3.2` 。展示了一组 3D 坐标轴。用户可以通过拖动鼠标来旋转视图。
    - `c3/rotation-axis.html </../en/demos/c3/rotation-axis.html>`_ — 来自 :ref:`c3.2` 。阐释了 3D 中围绕轴的旋转。一个立方体围绕旋转轴旋转。用户可以选择轴。
    - `c3/transform-equivalence-3d.html </../en/demos/c3/transform-equivalence-3d.html>`_ — 来自 :ref:`c3.3` 。尝试演示 3D 中建模和视图之间的等价性。用户拖动滑块来修改变换，并看到这个变换既作为建模变换应用于对象，也作为视图变换应用于视图体积。无论哪种解释，视图体积的内容和产生的图像都是相同的。
    - `c3/ifs-polyhedron-viewer.html </../en/demos/c3/ifs-polyhedron-viewer.html>`_ — 来自 :ref:`c3.4` 。让用户查看程序中定义为索引面集的各种多面体。用户可以旋转多面体并控制一些渲染选项。
    - `c4/materials-demo.html </../en/demos/c4/materials-demo.html>`_ — 来自 :ref:`c4.1` 。让用户改变对象的漫反射、镜面反射和光泽度属性，并查看结果。
    - `c4/smooth-vs-flat.html </../en/demos/c4/smooth-vs-flat.html>`_ — 来自 :ref:`c4.1` 。让用户看到使用法向量来模拟平滑表面与模拟平面多面体之间的区别。
    - `c4/four-lights-demo.html </../en/demos/c4/four-lights-demo.html>`_ — 来自 :ref:`c4.2` 。演示多个不同颜色、移动的灯光的效果。
    - `c4/two-sided-demo.html </../en/demos/c4/two-sided-demo.html>`_ — 来自 :ref:`c4.2` 。一个小型演示，说明了双面照明，前后材料不同。
    - `c4/texture-transform.html </../en/demos/c4/texture-transform.html>`_ — 来自 :ref:`c4.3` 。展示了各种对象上的纹理，以及用户可以使用滑块控制的纹理变换。
    - `c4/texture-from-color-buffer.html </../en/demos/c4/texture-from-color-buffer.html>`_ — 来自 :ref:`c4.3` 。copyTexImage2D()函数的一个简单演示；绘制一个动画化的 2D 场景，并将其作为纹理应用于 3D 对象上。
    - `c4/walkthrough.html </../en/demos/c4/walkthrough.html>`_ — 来自 :ref:`c4.4` 。通过点击按钮让用户在 3D 世界中移动，展示了移动观察者或相机的概念。
    - `c5/point-cloud.html </../en/demos/c5/point-cloud.html>`_ — 来自 :ref:`c5.1` 。使用 three.js JavaScript 3D 建模 API 的第一个示例。它使用 PointCloud 对象来显示一个动画化的点云。
    - `c5/mesh-objects.html </../en/demos/c5/mesh-objects.html>`_ — 来自 :ref:`c5.1` 。让用户查看许多基本的 three.js 几何体，并使用各种材料。
    - `c5/vertex-and-color-animation.html </../en/demos/c5/vertex-and-color-animation.html>`_ — 来自 :ref:`c5.2` 。使用每个面和每个顶点着色来创建一个多色球体。顶点的位置和颜色都可以动画化。
    - `c5/textures.html </../en/demos/c5/textures.html>`_ — 来自 :ref:`c5.2` 。在各种 three.js 对象上演示纹理。
    - `c5/mesh-animation.html </../en/demos/c5/mesh-animation.html>`_ — 来自 :ref:`c5.2` 。展示了使用“形态目标”和类 **THREE.MorphAnimation** 的马和鹳的动画模型。模型来自 three.js 下载包。
    - `c5/raycaster-input.html </../en/demos/c5/raycaster-input.html>`_ — 来自 :ref:`c5.3` 。让用户使用鼠标编辑场景。使用类型为 **THREE.Raycaster** 的对象从用户那里获取鼠标输入。
    - `c5/shadows.html </../en/demos/c5/shadows.html>`_ — 来自 :ref:`c5.3` 。演示了 *three.js* 对阴影的支持。
    - `c5/reflection-demo.html </../en/demos/c5/reflection-demo.html>`_ — 来自 :ref:`c5.3` 。演示了环境映射以模拟环境的反射。在这种情况下，环境是一个天空盒。（这个演示与示例程序 `threejs/reflection.html </../en/source/threejs/reflection.html>`_ 非常相似。）
    - `c6/shape-stamper-demo.html </../en/demos/c6/shape-stamper-demo.html>`_ — 来自 :ref:`c6.2` 。示例 WebGL 程序 `webgl/shape-stamper.html </../en/source/webgl/shape-stamper.html>`_ 的演示版本。用户点击画布将形状盖章到画布上，属性由一组弹出菜单确定。演示与示例程序具有相同的功能，但使用不同的技术绘制形状。
    - `c6/moving-points-demo.html </../en/demos/c6/moving-points-demo.html>`_ — 来自 :ref:`c6.2` 。示例 WebGL 程序 `webgl/moving-points.html </../en/source/webgl/moving-points.html>`_ 的演示版本，具有相同的功能。使用单个 gl.POINTS 原语来显示一组移动的彩色圆盘。
    - `c6/webgl-limits.html </../en/demos/c6/webgl-limits.html>`_ — 来自 :ref:`c6.3` 。显示 WebGL 中某些资源限制的值列表，例如着色程序中的属性数量或视口的大小。这些值在不同的设备和不同的网络浏览器中可能会有所不同。
    - `c6/textured-points.html </../en/demos/c6/textured-points.html>`_ — 来自 :ref:`c6.4` 。展示了在类型为 gl.POINTS 的原语上使用纹理图像。它与 moving-points-demo.html 类似，只是点是带纹理而不是彩色的。
    - `c6/multi-texture.html </../en/demos/c6/multi-texture.html>`_ — 来自 :ref:`c6.4` 。在同一对象上使用两个纹理，在着色程序中使用两个采样器变量来表示用于应用纹理的纹理单元。
    - `c7/rotators.html </../en/demos/c7/rotators.html>`_ — 来自 :ref:`c7.1` 。通过让用户使用两种旋转器旋转立方体，演示了 SimpleRotator ( `webgl/simple-rotator.js </../en/source/webgl/simple-rotator.js>`_ ) 和 TrackballRotator (`webgl/trackball-rotator.js </../en/source/webgl/trackball-rotator.js>`_ ) 之间的区别。
    - `c7/per-pixel-vs-per-vertex.html </../en/demos/c7/per-pixel-vs-per-vertex.html>`_ — 来自 :ref:`c7.2` 。让用户通过将这两种技术应用于具有相同照明设置的相同对象，比较每个像素的照明和每个顶点的照明。
    - `c7/spotlight-demo.html </../en/demos/c7/spotlight-demo.html>`_ — 来自 :ref:`c7.2` 。三个彩色聚光灯照射在一个正方形上，用户控制截止角度和聚光指数。示例程序 [webgl/spotlights.html </../en/source/webgl/spotlights.html>`_ 的演示版本，增加了一些动画以增加趣味性。
    - `c7/generated-texcoords.html </../en/demos/c7/generated-texcoords.html>`_ — 来自 :ref:`c7.3` 。使用从对象或眼睛坐标生成的纹理坐标，而不是将纹理坐标作为属性提供给着色程序。
    - `c7/procedural-textures.html </../en/demos/c7/procedural-textures.html>`_ — 来自 :ref:`c7.3` 。展示了几种 2D 和 3D 过程纹理。
    - `c7/cube-camera-demo.html </../en/demos/c7/cube-camera-demo.html>`_ — 来自 :ref:`c7.4` 。本质上是示例 WebGL 程序 `webgl/cube-camera.html </../en/source/webgl/cube-camera.html>`_ 的副本。展示了一个天空盒和在茶壶或其他物体表面反射的移动立方体。使用动态立方体贴图，每一帧都重新绘制。
    - `c9/first-webgpu-demo.html </../en/demos/c9/first-webgpu-demo.html>`_ — 来自 :ref:`c9.1` 。一个 WebGPU 演示，仅绘制一个彩色三角形。它也用作测试，以检查浏览器是否支持 WebGPU。
    - `c9/multisampling-demo.html </../en/demos/c9/multisampling-demo.html>`_ — 来自 :ref:`c9.2` 。展示了一个移动的随机彩色圆盘的动画。圆盘使用实例化绘制。演示使用多重采样进行反锯齿处理，并允许用户打开和关闭多重采样以查看效果。
    - `c9/diskworld-webgpu-demo.html </../en/demos/c9/diskworld-webgpu-demo.html>`_ — 来自 :ref:`c9.4` 。展示了 WebGPU 中的分层 3D 图形。功能和代码与示例程序 `webgpu/diskworld_webgpu.html </../en/source/webgpu/diskworld_webgpu.html>`_ 相同，只是做了一些更改以将其变成演示。
    - `c9/diffusion-demo.html </../en/demos/c9/diffusion-demo.html>`_ — 来自 :ref:`c9.6.3` 。使用 WebGPU 计算着色器实现扩散模拟。白色粒子通过布朗运动移动。当一个白色粒子击中黄色或青色粒子时，它会变色以匹配并停止移动。结果是建立起一个有趣的类似树枝的图案。这是示例程序 `webgpu/diffusion.html </../en/source/webgpu/diffusion.html>`_ 的演示版本。

.. tab:: 英文

    This book includes "live" or "interactive" demos that are embedded in the web pages. The demos are small programs written as web pages using JavaScript and either HTML canvas graphics or WebGL. Although they are designed to be run as small applications inside other web pages, they can also be run as independent web pages. In the web site download of this book, you can find the demos in the folder named demos, organized by chapter number. They can be run directly from that folder. Note that each of the demos requires certain other files that are contained in the demos folder; if you copy a demo to a different location, be sure to also copy all the files on which it depends.

    The demos from :ref:`Chapter 2 <c2>` use the 2D canvas graphics API, which will work in almost all modern web browsers, Demos from :ref:`Chapter 3 <c3>` through 8 use WebGL, which will also work with almost all modern web browsers. (However, WebGL might still have problems in some of these browsers on some machines.) All demo programs that use WebGL will work with WebGL 1.0. The demos in Chapter 9 require a web browser that supports WebGPU.

    The demos in :ref:`Chapter 3 <c3>` and :ref:`Chapter 4 <c4>` use `glsim.js </../en/source/glsim/glsim.js>`_, a JavaScript library that I wrote to simulate a subset of OpenGL 1.1. Information about glsim can be found in `glsim/glsim-doc.html </../en/source/glsim/glsim-doc.html>`_.

    For many of the demos, the reader is not expected to understand the program code for the demo at the point where the demo occurs in the book. Note that the JavaScipt code in the demos has **not** been updated to use the more modern version of JavaSctipt that is covered in :ref:`Section A.3 <a.3>`.

    - `c2/pixel-magnifier.html </../en/demos/c2/pixel-magnifier.html>`_ — from :ref:`Section 2.1 <c2.1>`. Magnifies a small square of pixels in an image so that the user can see how text, lines and other shapes are made from pixels, including antialiasing.
    - `c2/rgb-hsv.html </../en/demos/c2/rgb-hsv.html>`_ — from :ref:`Section 2.1 <c2.1>`. Lets the user modify a color in the RGB and HSV color spaces by dragging sliders.
    - `c2/approximating-ovals.html </../en/demos/c2/approximating-ovals.html>`_ — from :ref:`Section 2.2 <c2.2>`. Shows how ovals can be approximated by a polygons with different numbers of sides.
    - `c2/cubic-bezier.html </../en/demos/c2/cubic-bezier.html>`_ — from :ref:`Section 2.2 <c2.2>`. Lets the user modify a cubic Bezier curve by dragging endpoints and control points.
    - `c2/quadratic-bezier.html </../en/demos/c2/quadratic-bezier.html>`_ — from :ref:`Section 2.2 <c2.2>`. Lets the user modify a quadratic Bezier curve by dragging endpoints and control points.
    - `c2/transforms-2d.html </../en/demos/c2/transforms-2d.html>`_ — from :ref:`Section 2.3 <c2.3>`. Lets the user apply a sequence of rotation, scaling, and translation transforms to a shape and see the results.
    - `c2/transform-equivalence-2d.html </../en/demos/c2/transform-equivalence-2d.html>`_ — from :ref:`Section 2.4 <c2.4>`. attempts to demonstrate the equivalence between the modeling transform and the viewport transform in 2D.
    - `c2/cart-and-windmills.html </../en/demos/c2/cart-and-windmills.html>`_ — from :ref:`Section 2.4 <c2.4>`. Shows a simple, animated 2D scene constructed using hierarchical modeling.
    - `c2/SimplePaintDemo.html </../en/demos/c2/SimplePaintDemo.html>`_ — from :ref:`Section 2.6 <c2.6>`. Lets the user draw on a canvas using some basic shapes. A "Smudge" tool illustrates pixel manipulation. This demo is pretty much the same as the sample program `canvas2d/SimplePaintProgram.html </../en/source/canvas2d/SimplePaintProgram.html>`_.
    - `c2/image-filters.html </../en/demos/c2/image-filters.html>`_ — from :ref:`Section 2.6 <c2.6>`. Lets the user apply a variety of "filters" to several images. A filter, as the term is used here, replaces the color of each pixel with a weighted average of the colors of that pixel and its eight neighbors.
    - `c3/first-triangle-demo.html </../en/demos/c3/first-triangle-demo.html>`_ — from :ref:`Section 3.1 <c3.1>` . Shows the usual first example for OpenGL: A triangle with differently colored vertices. For this demo, you can change the colors of the vertices.
    - `c3/first-cube.html </../en/demos/c3/first-cube.html>`_ — from :ref:`Section 3.1 <c3.1>` . Draws a cube with six different colors for the sides (with no lighting effects, and with the default orthographic projection). The user can turn the depth test on and off to see the effect. And the user can use a bigger cube, to see the effects of "clipping" when parts of the cube extend outside the visible range of z-values.
    - `c3/axes3D.html </../en/demos/c3/axes3D.html>`_ — from :ref:`Section 3.2 <c3.2>` . Shows a set of coordinate axes in 3D. The user can drag the mouse to rotate the view.
    - `c3/rotation-axis.html </../en/demos/c3/rotation-axis.html>`_ — from :ref:`Section 3.2 <c3.2>`. Illustrates rotation about an axis in 3D. A cube spins about an axis of rotation. The user can select the axis.
    - `c3/transform-equivalence-3d.html </../en/demos/c3/transform-equivalence-3d.html>`_ — from :ref:`Section 3.3 <c3.3>` . attempts to demonstrate the equivalence between modeling and viewing in 3D. The user drags sliders to modify a transform, and sees that transform applied both to objects as a modeling transform and to the view volume as a viewing transform. The contents of the view volume and the image that is produced are the same in either interpretation.
    - `c3/ifs-polyhedron-viewer.html </../en/demos/c3/ifs-polyhedron-viewer.html>`_ — from :ref:`Section 3.4 <c3.4>` . Lets the user view a variety of polyhedra that are defined in the program as indexed face sets. The user can rotate the polyhedron and control some rendering options.
    - `c4/materials-demo.html </../en/demos/c4/materials-demo.html>`_ — from :ref:`Section 4.1 <c4.1>`. Lets the user change the diffuse, specular and shininess properties of an object and see the result.
    - `c4/smooth-vs-flat.html </../en/demos/c4/smooth-vs-flat.html>`_ — from :ref:`Section 4.1 <c4.1>`. Lets the user see the difference between using normal vectors to model a smooth surface versus modeling a flat-sided polyhedron.
    - `c4/four-lights-demo.html </../en/demos/c4/four-lights-demo.html>`_ — from :ref:`Section 4.2 <c4.2>`. Demonstrates the effect of multiple, differently colored, moving lights.
    - `c4/two-sided-demo.html </../en/demos/c4/two-sided-demo.html>`_ — from :ref:`Section 4.2 <c4.2>`. A little demo that illustrates two-sided lighting, with different front and back materials.
    - `c4/texture-transform.html </../en/demos/c4/texture-transform.html>`_ — from :ref:`Section 4.3 <c4.3>` . Shows textures on various objects, with texture transformations that the user can control using sliders.
    - `c4/texture-from-color-buffer.html </../en/demos/c4/texture-from-color-buffer.html>`_ — from :ref:`Section 4.3 <c4.3>`. A simple demo of the copyTexImage2D() function; draws an animated 2D scene and uses it as a texture on a 3D object.
    - `c4/walkthrough.html </../en/demos/c4/walkthrough.html>`_ — from :ref:`Section 4.4 <c4.4>`. Lets the user move around in a 3D world by clicking buttons, demonstrating the idea of a moving viewer or camera.
    - `c5/point-cloud.html </../en/demos/c5/point-cloud.html>`_ — from :ref:`Section 5.1 <c5.1>`. A first example of using the three.js JavaScript 3D modeling API. It uses a PointCloud object to show an animated cloud of points.
    - `c5/mesh-objects.html </../en/demos/c5/mesh-objects.html>`_ — from :ref:`Section 5.1 <c5.1>`. Lets the user view many of the basic three.js geometries, with a variety of materials.
    - `c5/vertex-and-color-animation.html </../en/demos/c5/vertex-and-color-animation.html>`_ — from :ref:`Section 5.2 <c5.2>`. Uses per-face and per-vertex coloring to create a multicolored sphere. Both the colors and the position of the vertices can be animated.
    - `c5/textures.html </../en/demos/c5/textures.html>`_ — from :ref:`Section 5.2 <c5.2>`. Demonstrates textures on a variety of three.js objects.
    - `c5/mesh-animation.html </../en/demos/c5/mesh-animation.html>`_ — from :ref:`Section 5.2 <c5.2>`. Shows animated models of a horse and a stork, using models with "morph targets" and the class **THREE.MorphAnimation**. The models are from the three.js download.
    - `c5/raycaster-input.html </../en/demos/c5/raycaster-input.html>`_ — from :ref:`Section 5.3 <c5.3>`. Lets the user edit a scene using the mouse. Uses an object of type **THREE.Raycaster** to get mouse input from the user.
    - `c5/shadows.html </../en/demos/c5/shadows.html>`_ — from :ref:`Section 5.3 <c5.3>`. Demonstrates support for shadows in *three.js*.
    - `c5/reflection-demo.html </../en/demos/c5/reflection-demo.html>`_ — from :ref:`Section 5.3 <c5.3>`. Demonstrates environment mapping to simulate reflection of an environment. The environment in this case is a skybox. (The demo is very similar to the sample program `threejs/reflection.html </../en/source/threejs/reflection.html>`_.)
    - `c6/shape-stamper-demo.html </../en/demos/c6/shape-stamper-demo.html>`_ — from :ref:`Section 6.2 <c6.2>`. A demo version of the sample WebGL program `webgl/shape-stamper.html </../en/source/webgl/shape-stamper.html>`_. The user clicks the canvas to stamp shapes onto the canvas, with properties determined by a set of popup menus. The demo has the same functionality as the sample program, but the shapes are drawn using a different technique.
    - `c6/moving-points-demo.html </../en/demos/c6/moving-points-demo.html>`_ — from :ref:`Section 6.2 <c6.2>`. A demo version of the sample WebGL program `webgl/moving-points.html </../en/source/webgl/moving-points.html>`_, with identical functionality. Uses a single gl.POINTS primitive to display a set of moving, colored disks.
    - `c6/webgl-limits.html </../en/demos/c6/webgl-limits.html>`_ — from :ref:`Section 6.3 <c6.3>`. Displays a list of values for certain resource limits in WebGL, such as the number of attributes in a shader program or the size of the viewport. These values can be different on different devices and in different web browsers.
    - `c6/textured-points.html </../en/demos/c6/textured-points.html>`_ — from :ref:`Section 6.4 <c6.4>`. shows texture images used on a primitive of type gl.POINTS. It is similar to moving-points-demo.html, except that the points are textured instead of colored.
    - `c6/multi-texture.html </../en/demos/c6/multi-texture.html>`_ — from :ref:`Section 6.4 <c6.4>`. Uses two textures on the same object, with two sampler variables in the shader program to represent the texture units that are used to apply the textures.
    - `c7/rotators.html </../en/demos/c7/rotators.html>`_ — from :ref:`Section 7.1 <c7.1>`. Demonstrates the difference between a SimpleRotator (`webgl/simple-rotator.js </../en/source/webgl/simple-rotator.js>`_) and a TrackballRotator (`webgl/trackball-rotator.js </../en/source/webgl/trackball-rotator.js>`_) by letting the user rotate cubes using the two rotators.
    - `c7/per-pixel-vs-per-vertex.html </../en/demos/c7/per-pixel-vs-per-vertex.html>`_ — from :ref:`Section 7.2 <c7.2>`. Lets the user compare per-pixel lighting to per-vertex lighting, by applying the two techniques to identical objects with identical lighting settings.
    - `c7/spotlight-demo.html </../en/demos/c7/spotlight-demo.html>`_ — from :ref:`Section 7.2 <c7.2>`. Three colored spotlights shine on a square, and the user controls the cutoff angle and spot exponent. A demo version of the sample program `webgl/spotlights.html </../en/source/webgl/spotlights.html>`_ , with some added animation for fun.
    - `c7/generated-texcoords.html </../en/demos/c7/generated-texcoords.html>`_ — from :ref:`Section 7.3 <c7.3>`. Uses texture coordinates generated from object or eye coordinates, instead of providing the texture coordinates to the shader program as an attribute.
    - `c7/procedural-textures.html </../en/demos/c7/procedural-textures.html>`_ — from :ref:`Section 7.3 <c7.3>`. Demonstrates several 2D and 3D procedural textures.
    - `c7/cube-camera-demo.html </../en/demos/c7/cube-camera-demo.html>`_ — from :ref:`Section 7.4 <c7.4>`. Essentially a copy of the sample WebGL program `webgl/cube-camera.html </../en/source/webgl/cube-camera.html>`_. Shows a skybox and moving cubes reflected on the surface of a teapot or other object. Uses a dynamic cubemap texture that is redrawn for every frame.
    - `c9/first-webgpu-demo.html </../en/demos/c9/first-webgpu-demo.html>`_ — from :ref:`Section 9.1 <c9.1>`. A WebGPU demo that just draws a colored triangle. It is also meant as a test to check whether a browser supports WebGPU.
    - `c9/multisampling-demo.html </../en/demos/c9/multisampling-demo.html>`_ — from :ref:`Section 9.2 <c9.2>`. Shows an animation of moving randomly colored disks. The disks are drawn using instanced drawing. The demo uses multisampling for antialiasing, and lets the user turn multisampling on and off to see the effect.
    - `c9/diskworld-webgpu-demo.html </../en/demos/c9/diskworld-webgpu-demo.html>`_ — from :ref:`Section 9.4 <c9.4>`. Illustrates hierarchical 3D graphics in WebGPU. The functionality and code are identical to the sample program `webgpu/diskworld_webgpu.html </../en/source/webgpu/diskworld_webgpu.html>`_ except for changes made to turn it into a demo.
    - `c9/diffusion-demo.html </../en/demos/c9/diffusion-demo.html>`_ —from :ref:`Section 9.6.3 <c9.6.3>`. Uses WebGPU compute shaders to implement a simulation of diffusion. White particles move by Brownian motion. When a white particle hits a yellow or cyan particle, it changes color to match and stops moving. The result is to build up an interesting dendrite-like pattern. This is a demo version of the sample program `webgpu/diffusion.html </../en/source/webgpu/diffusion.html>`_.
