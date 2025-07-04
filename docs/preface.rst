.. _preface:

前言
========================

这本教科书代表了我开发一学期计算机图形学第一门课程的尝试，该课程通常由计算机科学专业的学生在大学第三年或第四年学习。 （考虑到计算机图形学领域总是在快速变化，它能持续适用多久是一个悬而未决的问题。）我也试图使这本书适合自学。

本书的读者应该具有至少一种编程语言的丰富经验，包括一些面向对象编程和数据结构的知识。每个参加我自己的计算机图形课程的人都至少有两个学期的编程经验，而且大多数人都有除此之外的额外经验。我的学生学习了 Java 编程语言，但具有其他语言背景的人也应该可以阅读这本书。书中的示例使用 JavaScript、Java 和 C。可以用 JavaScript 进行所有编程，但一些 C 知识对于本书的某些部分也很重要。附录中介绍了这三种编程语言的基本功能。 （如果您需要从头开始学习编程，请尝试我的免费 Java 入门教科书，可从 http://math.hws.edu/javanotes 获取。）

我在 2015 年秋季的一门课程中使用了本书的 1.0 版本。1.1 版本纠正了一些错误和拼写错误，并添加了一些材料。我的课程 2017 年秋季版本中使用了它。我在 2021 年秋季使用的版本 1.3 添加了一些有关 WebGL 2.0 和 GLSL ES 3.00 的材料，更新了大部分 JavaScript 代码以使用 ES6，并更新了第 5 章以使用Three.js库的版本 129。

尽管我已经从教学岗位退休，但我决定在 2023 年夏季开发 1.4 版本。我添加了有关 WebGPU 的新章节，并迁移到Three.js的版本 154 。由于 WebGPU 使用 JavaScript Promise，因此我在附录 A 中添加了一个新部分来介绍 Promise 和异步函数。因为Three.js很快就会删除该库的非模块化版本，所以我在第 5 章开头添加了一个关于 JavaScript 模块的简短部分，并且修改了Three.js示例以使用模块。除了转向模块化的Three.js之外，第 5 章中的内容没有改变。整本书中的许多错别字和小错误都得到了修正。 （感谢读者 Danny Hurlburt 修复了其中的许多问题。）

本书的主页网站是 https://math.hws.edu/graphicsbook 。该地址的页面包含用于下载网站副本和下载本书PDF版本的链接。

这是一本免费教科书。欢迎您重新分发它，只要您不收取任何费用。您可以在您自己的网站上发布未经修改的副本。您可以制作和分发修改版本（包括翻译），只要您的版本明确原始来源并且在同一许可证下免费分发即可。 （正式地，这本书是根据“知识共享非商业署名相同方式共享许可证”获得许可的。）

----

本书的许多示例程序实际上都是要在 Web 浏览器中查看的网页。本书的网络版本包括集成到本书网页中的交互式演示程序。

大多数示例程序和所有演示都使用 HTML 画布图形（ :ref:`第 2 章 <c2>` 中）、WebGPU（ :ref:`第 9 章 <c9>` 中）或 WebGL（其他章节中）。 Canvas 图形和 WebGL 应该可以在几乎所有现代浏览器中正常工作。 WebGPU是一项新技术，问题也比较多。到 2023 年 7 月，它默认仅在少数 Web 浏览器（Windows 和 MacOS 上的 Chrome 和 Edge）中可用，甚至在那些浏览器上也可能无法在所有硬件上运行。在其他一些浏览器中，它可以作为实验性功能启用。然而，WebGPU 很可能成为 Web 3D 图形的未来，因此开始学习它很重要。

示例程序和演示都可以在本书的网站版本的下载中找到，该版本可以从其 主页获得。在名为source和demo 的文件夹中查找它们。请注意，大多数 Web 浏览器不愿意使用本地文件系统中的某些资源，例如 3D 模型和模块化 JavaScript 脚本。当这些浏览器尝试在本地而不是通过 Web 运行某些示例时，它们将会出现错误。此问题仅影响部分示例。对于这些示例，您可以使用本书的在线版本。另一种解决方案是在您自己的计算机上运行网络服务器并通过该网络服务器查看教科书。可以将 Web 浏览器配置为使用本地文件中的资源，尽管使用该配置浏览 Web 可能不是一个好主意。

----

在近 35 年的时间里，我每隔几年左右就教授一次计算机图形学。随着该领域的发展，我几乎每次教授课程时都必须做出重大改变，但在大部分时间里，我能够主要围绕 OpenGL 1.1（一种在很长一段时间内普遍使用的图形 API）来构建课程。 OpenGL 1.1 以透明且相当易于使用的方式实现基本图形概念（顶点、法向量、坐标变换、光照和材质）。较新的图形 API 更灵活、更强大，但学习曲线更陡峭。我相信任何计算机科学入门课程都受益于从更简单的框架或库开始，而 OpenGL 1.1 很好地实现了这一目的。

OpenGL 仍然受到广泛支持，但是，由于各种原因，它易于使用的部分已从最新版本中正式删除（尽管实际上大多数台式计算机都支持它们）。此外，OpenGL 正在很大程度上被更新的图形 API（例如 Direct3D、Metal 和 Vulkan）所取代。 WebGL 基于 OpenGL，并将在一段时间内继续得到广泛支持。 WebGPU 受到较新 API 的启发，并且可能在某些时候取代新应用程序的 WebGL。

我在本书中的方法是使用 OpenGL 1.1 的一个子集作为框架来介绍三维图形的基本概念。然后我将继续介绍 WebGL，这是在 Web 浏览器中运行的 OpenGL 版本。在上一章中，我介绍了WebGPU。虽然 OpenGL 构成了本课程的主要基础，但真正的重点是几何建模和变换等基本概念；分层建模和场景图；颜色、灯光和纹理；和动画。我仍然相信 OpenGL 1.1 很好地介绍了这种材质。

:ref:`第 1 章 <c1>` 是计算机图形学的简短概述。它介绍了许多概念，本书的其余部分将更详细地介绍这些概念。

:ref:`第 2 章 <c2>` 介绍了 Java、JavaScript 和 SVG 中的二维图形，重点介绍了诸如转换和场景图等可扩展到三维的概念。

:ref:`第 3 章 <c3>` 和 :ref:`第4 章 <c4>` 介绍了 OpenGL 1.1。虽然按照今天的标准来看 OpenGL 1.1 相当原始，但它包含的许多基本功能仍然是 3D 计算机图形学的基础。仅涵盖部分 API。

:ref:`第 5 章 <c5>` 介绍了Three.js，这是一个使用 JavaScript 进行 Web 图形的高级面向对象 3D 图形 API。本章展示了如何在更高级别的接口中使用基本概念。

:ref:`第 6 章 <c6>` 和 :ref:`第7 章 <c7>` 介绍了 WebGL，它是用于 Web 图形的 OpenGL 的现代版本。 WebGL 非常底层，它需要程序员编写“着色器程序”来实现 OpenGL 1.1 中内置的许多功能。查看实现是一个更深入地了解计算机如何实际制作 3D 图像的机会。

:ref:`第 8 章 <c8>` 非常简要地介绍了 OpenGL 中无法实现的一些高级技术。

:ref:`第 9 章 <c9>` 介绍了 WebGPU，这是最新的 Web 图形 API 。

:ref:`附录 A <appendx A>` 简要介绍了本书中使用的三种编程语言：Java、C 和 JavaScript。 :ref:`附录 B <appendx B>` 旨在让读者开始了解 Blender（一个复杂的 3D 建模程序）的最基本用法。我发现向学生介绍 Blender 是帮助他们发展三维直觉的好方法。 :ref:`附录 C <appendx C>` 包含对两个 2D 图形程序 Gimp 和 Inkscape 的更简要介绍。

----

旧版本仍然可用：

- 1.0版：https://math.hws.edu/eck/cs424/graphicsbook-1.0/
- 版本 1.1：https://math.hws.edu/eck/cs424/graphicsbook-1.1/
- 版本 1.2：https://math.hws.edu/eck/cs424/graphicsbook-1.2/
- 版本 1.3：https://math.hws.edu/eck/cs424/graphicsbook-1.3/
- 所有版本的下载都可以在 https://math.hws.edu/eck/cs424/downloads/ 找到。

----

本书的 PDF 和网站版本是根据一组常见来源构建的。可以通过在 GitHub 上克隆以下 git 存储库来获取源代码： https://github.com/davidjeck/graphicsbook

这些来源最初并不打算出版，并且对可能有兴趣研究它们的人没有任何保证和非常有限的支持。

源包括图像、HTML 文件、Java 和 C 源代码、XML 文件、XSLT 转换、bash shell 脚本和 LaTeX 宏。使用源代码需要额外的软件（LaTeX、Xalan-J、Java 和 bash shell）。有关详细信息，请参阅 :ref:`自述文件 <README>`。

----

David J. Eck， 霍巴特和威廉史密斯学院

数学与计算机科学系名誉教授 300 Pulteney StreetGeneva , New York 14456, USA

电子邮件：eck@hws.edu

WWW：http://math.hws.edu/eck/ , 2023
