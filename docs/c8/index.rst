.. _c8:

第 8 章： 超越基本 3D 图形
========================

**Beyond Basic 3D Graphics**

.. tab:: 中文

    这本教科书的前七章涵盖了基本的实时计算机图形学，即能够在几秒钟内生成图像的图形系统。典型的例子是视频游戏，在那里新的画面每秒可以渲染多达六十次。使用本书介绍的技术，加上现代GPU的强大处理能力，以及一些技巧和高级算法，可以实时渲染非常复杂和逼真的场景。现代高端GPU已经开始增加一些对光线追踪和全局照明的直接硬件支持，但实时图形仍然无法与电影中所能找到的最高质量的计算机图形的逼真度相匹配。事实上，今天电影中的CGI（计算机生成图像）有时与现实无法区分。要达到那种质量的图形可能需要数小时的计算时间来渲染单个画面。

    这一章是对一些可用于非常高画质图形的技术的非常简要的介绍。讨论将用一般术语进行。我不会提供示例代码或对技术背后的数学进行详细讨论，但我希望至少提供基本的概念理解。

    然而，你应该明白的第一件事是，到目前为止你所学的大部分内容仍然适用。场景仍然使用几何基本体、变换、材质、纹理和光源（尽管可能使用比我们到目前为止遇到的更高级的材质属性和照明）来组成。为电影制作CGI的图形设计师可以看到使用我们已经介绍过的技术渲染的他们工作的实时预览。你在电影中看到的最终场景只是使用不同的、更耗费计算的技术来渲染的。


.. tab:: 英文

    The first seven chapters of this textbook have covered basic real-time computer graphics, that is, graphics systems in which an image can be generated in a fraction of a second. The typical case is a video game, where new frames can be rendered as many as sixty times per second. Very complex and realistic-looking scenes can be rendered in real time, using techniques covered in this book and the immense processing power of modern GPUs, plus some tricks and advanced algorithms. Modern high-end GPUs have begun adding some direct hardware support for ray tracing and global illumination, but real-time graphics still can't match the realism of the very highest quality computer graphics, such as what can be found in movies. In fact, the CGI (computer generated imagery) in today's movies is sometimes indistinguishable from reality. Getting graphics of that quality can require hours of computing time to render a single frame.

    This chapter is a very brief look at some techniques that can be used for very high quality graphics. The discussion will be in general terms. I won't be giving sample code or detailed discussions of the mathematics behind the techniques, but I hope to provide at least a basic conceptual understanding.

    The first thing that you should understand, though, is that most of what you have leaned so far still applies. Scenes are still composed using geometric primitives, transformations, materials, textures, and light sources (although perhaps using more advanced material properties and lighting than we have encountered so far). The graphic designers working on CGI for a movie can see real time previews of their work that are rendered using techniques that we have covered. The final scene that you see in the movie is just rendered using different, much more computation-intensive techniques.
