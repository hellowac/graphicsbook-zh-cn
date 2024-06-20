# 第 9 章： WebGPU 简介

**Introduction to WebGPU**

=== "中文"

    This chapter introduces **WebGPU**, the new graphics API for the web. WebGPU has been under development for several years, but it is only recently that it has begun to be included as a standard feature in web browsers. In some browsers, you might find that it is available as an experimental feature that has to be explicitly enabled before it can be used. Some browsers might not support it at all.

    WebGPU will not replace WebGL, which will continue to be well-supported in almost all browsers for the foreseeable future. However, WebGL, like the OpenGL API on which it is based, is not likely to see much further development. WebGPU, on the other hand, is inspired by and similar to modern graphics APIs such as Vulkan, Direct3D, and Metal, and it is likely to evolve along with those APIs. So WebGPU should be thought of as the Web graphics API of the future.

    WebGPU is similar to WebGL in many ways. For example, it has vertex shaders and fragment shaders, and a lot of the programmer's work involves managing the flow of data into and through the rendering pipeline. But WebGPU is an even lower level API than WebGL. It is more verbose, and it puts more responsibility on the programmer for managing details of the rendering process. At the same time, however, it gives the programmer more control, access to more powerful capabilities of modern GPUs, and the possibility of more efficient code.

    The WebGPU specification is at <https://www.w3.org/TR/webgpu/>, but it is not very useful for learning. A simpler and more useful API reference can be found on the Mozilla Developer Network: <https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API>. Hopefully, though, this chapter has enough information to get you started with WebGPU.

    As this chapter is being written in July 2023, the official WebGPU documentation describes itself as a "Working Draft." Some details need to be filled in, and there could still be some minor changes in the API. It is unlikely that changes in the final version will affect anything in this textbook, but that can't be guaranteed.

=== "英文"

    This chapter introduces **WebGPU**, the new graphics API for the web. WebGPU has been under development for several years, but it is only recently that it has begun to be included as a standard feature in web browsers. In some browsers, you might find that it is available as an experimental feature that has to be explicitly enabled before it can be used. Some browsers might not support it at all.

    WebGPU will not replace WebGL, which will continue to be well-supported in almost all browsers for the foreseeable future. However, WebGL, like the OpenGL API on which it is based, is not likely to see much further development. WebGPU, on the other hand, is inspired by and similar to modern graphics APIs such as Vulkan, Direct3D, and Metal, and it is likely to evolve along with those APIs. So WebGPU should be thought of as the Web graphics API of the future.

    WebGPU is similar to WebGL in many ways. For example, it has vertex shaders and fragment shaders, and a lot of the programmer's work involves managing the flow of data into and through the rendering pipeline. But WebGPU is an even lower level API than WebGL. It is more verbose, and it puts more responsibility on the programmer for managing details of the rendering process. At the same time, however, it gives the programmer more control, access to more powerful capabilities of modern GPUs, and the possibility of more efficient code.

    The WebGPU specification is at <https://www.w3.org/TR/webgpu/>, but it is not very useful for learning. A simpler and more useful API reference can be found on the Mozilla Developer Network: <https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API>. Hopefully, though, this chapter has enough information to get you started with WebGPU.

    As this chapter is being written in July 2023, the official WebGPU documentation describes itself as a "Working Draft." Some details need to be filled in, and there could still be some minor changes in the API. It is unlikely that changes in the final version will affect anything in this textbook, but that can't be guaranteed.
