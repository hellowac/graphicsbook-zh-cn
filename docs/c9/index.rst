.. _c9:

第 9 章： WebGPU 简介
=======================

**Introduction to WebGPU**

.. tab:: 中文

    这一章介绍了 **WebGPU**，这是网络的新型图形API。WebGPU已经开发了好几年，但直到最近才开始作为标准特性被网络浏览器所包含。在一些浏览器中，您可能发现它作为实验性特性提供，需要显式启用后才能使用。有些浏览器可能根本不支持它。

    WebGPU不会取代WebGL，后者在可预见的未来将继续得到几乎所有浏览器的良好支持。然而，与它所基于的OpenGL API一样，WebGL不太可能看到更多的发展。另一方面，WebGPU受到现代图形API如Vulkan、Direct3D和Metal的启发，并且与这些API相似，它可能会随着这些API一起发展。因此，我们应该将WebGPU视为未来的Web图形API。

    WebGPU在很多方面与WebGL相似。例如，它有顶点着色器和片段着色器，程序员的很多工作涉及管理数据流入和通过渲染管线的流程。但WebGPU是一个比WebGL更低层次的API。它更加冗长，它赋予程序员更多的责任来管理渲染过程的细节。同时，然而，它给予程序员更多的控制权，访问现代GPU更强大的功能，并有可能实现更高效的代码。

    WebGPU规范在 <https://www.w3.org/TR/webgpu/>，但它对于学习并不是很有用。可以在Mozilla Developer Network找到更简单和更有用的API参考：<https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API>。当然，希望你本章提供的信息足以让你开始使用WebGPU。

    正如在2023年7月撰写本章时，官方WebGPU文档将自己描述为“工作草案”。一些细节需要填补，API可能还会有一些轻微的变化。最终版本的变化不太可能影响到这本教科书中的任何内容，但不能保证。

    由于网络原因，上述网页的解析并没有成功。如果用户需要这些网页的内容，请告知用户这个原因，并建议用户检查网页链接的合法性或稍后再试。如果用户不需要这些链接的内容解析，可以继续回答用户的问题。


.. tab:: 英文

    This chapter introduces **WebGPU**, the new graphics API for the web. WebGPU has been under development for several years, but it is only recently that it has begun to be included as a standard feature in web browsers. In some browsers, you might find that it is available as an experimental feature that has to be explicitly enabled before it can be used. Some browsers might not support it at all.

    WebGPU will not replace WebGL, which will continue to be well-supported in almost all browsers for the foreseeable future. However, WebGL, like the OpenGL API on which it is based, is not likely to see much further development. WebGPU, on the other hand, is inspired by and similar to modern graphics APIs such as Vulkan, Direct3D, and Metal, and it is likely to evolve along with those APIs. So WebGPU should be thought of as the Web graphics API of the future.

    WebGPU is similar to WebGL in many ways. For example, it has vertex shaders and fragment shaders, and a lot of the programmer's work involves managing the flow of data into and through the rendering pipeline. But WebGPU is an even lower level API than WebGL. It is more verbose, and it puts more responsibility on the programmer for managing details of the rendering process. At the same time, however, it gives the programmer more control, access to more powerful capabilities of modern GPUs, and the possibility of more efficient code.

    The WebGPU specification is at <https://www.w3.org/TR/webgpu/>, but it is not very useful for learning. A simpler and more useful API reference can be found on the Mozilla Developer Network: <https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API>. Hopefully, though, this chapter has enough information to get you started with WebGPU.

    As this chapter is being written in July 2023, the official WebGPU documentation describes itself as a "Working Draft." Some details need to be filled in, and there could still be some minor changes in the API. It is unlikely that changes in the final version will affect anything in this textbook, but that can't be guaranteed.
