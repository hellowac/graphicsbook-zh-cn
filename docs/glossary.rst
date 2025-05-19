术语表
=========


.. glossary::

    abstract class
        In object-oriented programming, a class that is meant to be used only as a basis for subclasses. Objects can be created from the subclasses, but not from the abstract class itself. The purpose of an abstract class is to define the properties and behaviors that all of its subclasses have in common.

        在面向对象编程中，一种仅用于作为子类基础的类。对象可以从子类创建，但不能直接从抽象类本身创建。抽象类的目的是定义所有子类共有的属性与行为。

    address space (in WGSL)
        WGSL memory is divided into address spaces. From the WGSL specification: "Each address space has unique properties determining mutability, visibility, the values it may contain, and how to use variables with it."

        WGSL 的内存被划分为多个地址空间。来自 WGSL 规范：“每个地址空间具有唯一的属性，决定其可变性、可见性、可包含的值，以及如何使用其中的变量。”

    affine transform
        A transform that preserves parallel lines. That is, when the transform is applied to a pair of lines that are parallel, then the resulting transformed lines are also parallel. An affine transform, T, has the property that the transform of the line segment between a point (x1,y1) and a point (x2,y2) is the line between the points T(x1,y1) and T(x2,y2). Effectively, the transform of a line segment can be computed just by transforming its two endpoints. This makes affine transforms very efficient for computer graphics. Any affine transform can be represented as a composition of rotations, translations, and scalings.

        一种保持平行线性质的变换。也就是说，当该变换作用于一对平行线时，结果中的线条仍然保持平行。仿射变换 T 满足以下性质：将点 (x1, y1) 与点 (x2, y2) 之间的线段进行变换，结果为 T(x1, y1) 与 T(x2, y2) 之间的线段。换言之，只需变换线段的两个端点即可得到变换后的线段。这使得仿射变换在计算机图形学中非常高效。任意仿射变换都可以表示为旋转、平移和缩放的组合。

    alignment (in WGSL)
        Restrictions on the legal location of a value in memory, depending on the data type. For example, the address of a vec3f variable in WGSL must be a multiple of 16.

        根据数据类型，限制某个值在内存中的合法位置。例如，WGSL 中的 vec3f 变量的地址必须是 16 的倍数。

    alpha
        An extra component (that is, one of the numbers that are used to specify a color) in a color model that is not part of the actual color specification. The alpha component is extra information. It is most often used to specify the degree of transparency of a color.

        一种在颜色模型中额外的分量（即用于指定颜色的数值之一），不属于实际颜色值本身。Alpha 分量是额外信息，最常用于指定颜色的透明度。


    alpha blending
        Using the alpha component of a color to blend the color with a background color, when the color is drawn over the background color. That is, the new color of a pixel is obtained by blending the drawing color with the current color, with the degree of blending depending on the alpha component of the drawing color. Alpha blending is most commonly used to simulate transparency.

        使用颜色的 alpha 分量，在绘制时将该颜色与背景色进行混合。也就是说，像素的新颜色是通过将绘图颜色与当前颜色按一定比例混合得到的，混合比例取决于绘图颜色的 alpha 分量。Alpha 混合通常用于模拟透明效果。

    
    alpha color component
        An extra component (that is, one of the numbers that are used to specify a color) in a color model that is not part of the actual color specification. The alpha component is extra information. It is most often used to specify the degree of transparency of a color.
        
        一种在颜色模型中额外的分量（即用于指定颜色的数值之一），不属于实际颜色值本身。Alpha 分量是额外信息，最常用于指定颜色的透明度。

    ambient color
        A material property that represents the proportion of ambient light in the environment that is reflected by a surface.

        一种材质属性，表示表面对环境中环境光的反射比例。

    ambient light
        Directionless light that exists in an environment but does not seem to come from a particular source in the environment. An approximation for light that has been reflected so many times that its original source can't be identified. Ambient light illuminates all objects in a scene equally.

        一种没有方向性的光，在场景中存在但不来自任何特定的光源。通常用作对经过多次反射、已无法辨识其原始来源的光的近似。环境光会均匀地照亮场景中的所有物体。

    ambient occlusion
        A rendering technique that takes into account the fact that ambient light will illuminate different surfaces to varying extents, depending on the degree to which ambient light is blocked, or "occluded," from reaching each surface by other geometry in the scene. Ambient occlusion is an improvement on basic ambient lighting, but, like ambient light itself, it is not an actual physical phenomenon.

        一种渲染技术，考虑环境光因被场景中其他几何体遮挡（即“遮蔽”）而对不同表面照亮程度的差异。环境遮蔽相比基础环境光照效果更加真实，但与环境光一样，并不代表真实的物理现象。


    anaglyph stereo
        A technique for combining stereographic images of a scene, one for the left eye and one for the right eye, into a single image. Typically, the image for the left eye is drawn using only shades of red, and the image for the right eye contains only blue and green color components. The 3D effect can be seen by viewing the combined image through red/cyan glasses, which allow each eye to see only the image that is intended for that eye.

        一种立体图像合成技术，将分别为左眼和右眼绘制的图像合并为一张图像。通常，左眼图像仅使用红色通道绘制，右眼图像仅使用蓝色和绿色通道。通过佩戴红/青立体眼镜可以看到三维效果，每只眼睛仅能看到为其设计的图像。


    animation
        A sequence of images that, when displayed quickly one after the other, will produce the impression of continuous motion or change. The term animation also refers to the process of creating such image sequences.

        一组连续图像序列，在快速播放时会产生连续运动或变化的视觉印象。该术语也指创建此类图像序列的过程。


    anisotropic filtering
        A technique for more accurate sampling of texture images, in the case where a pixel on the surface that is being textured corresponds to a non-rectangular region in the texture. Anisotropic filtering is available as an optional extension in WebGL.

        一种在贴图过程中更加精确的采样技术，适用于当被贴图表面的一个像素对应于纹理中一个非矩形区域时。各向异性过滤作为 WebGL 的一个可选扩展提供。


    antialiasing
        A technique used to reduce the jagged or "staircase" appearance of diagonal lines, text, and other shapes that are drawn using pixels. When a pixel is only partly covered by a geometric shape, then the color of the pixel is a blend of the color of the shape and the color of the background, with the degree of blending depending on the fraction of the pixel that is covered by the geometric shape.

        一种用于减少由像素绘制的对角线、文本和其他图形所产生的锯齿或“阶梯”效果的技术。当某个像素只被几何图形部分覆盖时，其颜色会是图形颜色与背景颜色的混合，混合比例取决于图形覆盖该像素的面积比例。


    Antialiasing
        A technique used to reduce the jagged or "staircase" appearance of diagonal lines, text, and other shapes that are drawn using pixels. When a pixel is only partly covered by a geometric shape, then the color of the pixel is a blend of the color of the shape and the color of the background, with the degree of blending depending on the fraction of the pixel that is covered by the geometric shape.

        一种用于减少由像素绘制的对角线、文本和其他图形所产生的锯齿或“阶梯”效果的技术。当某个像素只被几何图形部分覆盖时，其颜色会是图形颜色与背景颜色的混合，混合比例取决于图形覆盖该像素的面积比例。

    API
        Application Programming Interface. A collection of related classes, functions, constants, etc., for performing some task. An API is an "interface" in the sense that it can be used without understanding how its functionality is actually implemented.

        应用程序编程接口（Application Programming Interface）。一组相关的类、函数、常量等，用于执行某些任务。API 是一种“接口”，意味着使用者可以在不了解其内部实现细节的情况下使用其功能。


    aspect ratio
        The ratio of the width, w, of a rectangle to the height, h, of the rectangle, expressed either as a ratio **w:h** or as a fraction **w/h**.

        长宽比。矩形的宽度 *w* 与高度 *h* 的比值，可表示为比率 **w:h** 或分数形式 **w/h**。

    async function
        In JavaScript, an async function is one that can use an "await" statement to wait for the result of a promise. When an await statement is executed, the execution of the async function is suspended until the promise has either been fulfilled or rejected, giving other JavaScript code a chance to run in the meantime.

        在 JavaScript 中，async 函数是一种可以使用 ``await`` 语句等待 Promise 结果的函数。当执行 ``await`` 语句时，该 async 函数的执行将被挂起，直到该 Promise 被兑现（fulfilled）或拒绝（rejected），此时其他 JavaScript 代码可以并发运行。


    attenuation
        Refers to the way that illumination from a point light or spot light decreases with distance from the light. Physically, illumination should decrease with the square of the distance, but computer graphics often uses a linear attenuation with distance, or no attenuation at at all.

        表示从点光源或聚光灯发出的光照随距离衰减的方式。从物理上讲，光照应随距离的平方递减，但在计算机图形学中，通常采用线性衰减，甚至完全不考虑衰减。


    attribute
        A property, such as color, of a graphical object. An image can be specified by the geometric shapes that it contains, together with their attributes.

        图形对象的某个属性，例如颜色。图像可以由其包含的几何图形及其属性来描述。

    attributes
        A property, such as color, of a graphical object. An image can be specified by the geometric shapes that it contains, together with their attributes.

        图形对象的若干属性，例如颜色。图像可以由其包含的几何图形及其属性来描述。


    attribute variable
        Variables that represent input to the vertex shader in a programmable graphics pipeline. An attribute variable can take on a different value for each vertex in a primitive.

        在可编程图形管线中，表示传入顶点着色器的变量。每个图元中的顶点可以具有不同的 attribute 变量值。


    axis of rotation
        Rotation in 3D space is rotation about a line, which is called the axis of rotation. The axis of rotation remains fixed, while everything else moves in circles around the axis.

        在三维空间中，旋转是绕一条直线进行的，该直线称为旋转轴（axis of rotation）。旋转轴保持不动，其他所有东西围绕它作圆周运动。


    back faces
        One of the two sides of a polygon in 3D. A polygon has two sides. One is taken to be the front face, and the other is the back face. In OpenGL, the difference is determined by the order in which the vertices of the polygon are enumerated. The default is that, seen from the back, the vertices are enumerated in clockwise order around the polygon.

        三维多边形的两面之一。每个多边形都有正面与背面之分。在 OpenGL 中，这一区别由多边形顶点的排列顺序决定。默认情况下，从背面观察时顶点按顺时针顺序排列。


    barycentric coordinates
        A coordinate system on a triangle in which a point is written as a linear combination of the vertices of the triangle, that is, `a*A+b*B+c*C`, where A, B, and C are the vertices and a, b, and c are numbers. Any point in the triangle can be written in this form where the coefficients a, b, and c have values in the range 0 to 1 and a+b+c is equal to 1.

        三角形上的一种坐标系，在该坐标系中，一个点可写作该三角形三个顶点的线性组合形式，即 `a*A + b*B + c*C`，其中 A、B、C 是顶点，a、b、c 是系数。在三角形内任意一点都可以表示为 a、b、c 介于 0 到 1 且 a + b + c = 1 的组合。


    Bezier curve
        A smooth curve between two points defined by parametric polynomial equations. A cubic Bezier curve segment is defined by its two endpoints P1 and P2 and by two control points C1 and C2. The tangent to the curve (its direction and speed) at P1 is given by the line from P1 to C1. The tangent vector to the curve at P2 is given by the line from C2 to P2. A quadratic Bezier curve is defined by its two endpoints and a single control point C. The tangent at each endpoint is the line between that endpoint and C.

        一种通过参数化多项式方程定义的在两个点之间的平滑曲线。三次 Bézier 曲线段由两个端点 P1 和 P2 以及两个控制点 C1 和 C2 定义。在 P1 处的切线由 P1 到 C1 的直线决定，在 P2 处的切线由 C2 到 P2 的直线决定。二次 Bézier 曲线由两个端点和一个控制点 C 定义，每个端点的切线是该端点与 C 之间的直线。


    bind group (in WebGPU)
        A data structure that can hold resources such as buffers, textures, and samples, for input into a pipeline.

         WebGPU 中的一种数据结构，可用于存储缓冲区、纹理、采样器等资源，以供管线输入使用。

    Blender
        A free and open source 3D modeling and animation program.

        一个自由且开源的 3D 建模与动画制作程序。

    Bresenham's line algorithm
        A specific algorithm for deciding which pixels to color to represent a geometric line segment, using only integer arithmetic. The algorithm can be implemented very efficiently in computer hardware

         一种使用整数运算决定应着色哪些像素以表示几何线段的特定算法。该算法可被高效地实现于硬件中。

    BSDF
        Bidirectional Scattering Distribution Function. A generalization of the idea of "material" in 3D graphics. A BSDF gives the probability that a light ray that arrives at point of space from one direction will leave that point heading in a another direction. The probability is a function of the two directions, the point, and the wavelength of the light. One kind of scattering is reflection of light from a surface. For that case, the term BRDF (Bidirectional Reflectance Distribution Function) is used.

        双向散射分布函数（Bidirectional Scattering Distribution Function）。在 3D 图形中对“材质”概念的泛化。BSDF 给出一束光从某一方向射入空间某点后，以另一方向离开该点的概率。该概率是入射方向、出射方向、空间点以及光波长的函数。若考虑的是表面反射，则使用术语 BRDF（Bidirectional Reflectance Distribution Function）。


    bumpmapping
        Using a texture to modify the normal vectors on a surface, to give the appearance of variations in height without actually modifying the geometry of the surface.

        使用纹理来修改表面法向量，从而在不改变表面几何结构的情况下表现出高度变化的视觉效果。

    camera
        In 3D computer graphics, an object that combines the projection and viewing transforms into an abstraction that imitates a physical camera or eye.

        在三维计算机图形中，一种将投影变换与观察变换组合成抽象模型的对象，模仿物理相机或人眼的功能。


    clip coordinates
        The default coordinate system in OpenGL. The projection transform maps the 3D scene to clip coordinates. The rendered image will show the contents of the cube in the clip coordinate system that contains x, y, and z values in the range from -1 to 1; anything outside that range is "clipped" away.

        OpenGL 中的默认坐标系。投影变换会将 3D 场景映射到裁剪坐标（clip coordinates）中。最终图像显示的是裁剪坐标系中立方体范围内（x、y、z ∈ [-1, 1]）的内容，超出该范围的部分将被“裁剪”掉。

    color buffer
        In OpenGL, the region of memory that holds the color data for the image. It acts as the drawing surface where images are rendered.

        在 OpenGL 中，保存图像颜色数据的内存区域。它充当图像渲染时的绘制表面。

    color component
    color components
        One of the numbers used in a color model to specify a color. For example, in the RGB color model, a color is specified by three color components representing the amounts of red, green, and blue in the color.

        用于在颜色模型中指定颜色的数值之一。例如，在 RGB 颜色模型中，颜色由三个颜色分量表示，分别表示红色、绿色和蓝色的数量。


    color gamut
        The color gamut of a display device, such as a printer or computer screen, is the set of colors can be displayed by the device.

        显示设备（如打印机或计算机屏幕）所能显示的颜色集合，称为该设备的色域。

    color mask
        In WebGL, a setting that determines which "channels" in the color buffer are written during rendering. The channels are the RGBA color components red, green, blue, and alpha. A color mask consists of four boolean values, one for each channel. A false value prevents any change from being made to the corresponding color component in the color buffer.

        在 WebGL 中，一种设置，用于控制渲染过程中哪些“通道”会被写入颜色缓冲区。通道包括 RGBA 四个颜色分量：红、绿、蓝和 alpha。颜色掩码由四个布尔值组成，每个对应一个颜色分量。若值为 false，则对应的颜色通道在渲染过程中不会被修改。


    color model
        A way of specifying colors numerically. Each color that can represented in a color model is assigned one or more numerical component values. An example is the RGB color model, where a color is specified by three numbers giving the red, green, and blue components of the color.

        一种通过数值方式指定颜色的方法。每个颜色模型中的颜色由一个或多个数值分量表示。例如，在 RGB 颜色模型中，一个颜色由三个数值组成，分别表示红、绿、蓝的成分。


    column-major order
        Column-by-column ordering of the elements of a two-dimensional matrix; that is, an ordering that starts with the elements in the first column, followed by the elements in the second column, and so on. Column-major order is used for matrices in OpenGL and GLSL.

        将二维矩阵的元素按列优先排列的顺序：先存储第一列的所有元素，然后是第二列，依此类推。OpenGL 和 GLSL 中的矩阵采用列主序存储方式。


    compute shader
        A stage in a GPU pipeline that does purely computational work, rather than participating directly in graphical rendering.

        GPU 管线中的一个阶段，专门执行通用计算任务，而不直接参与图形渲染过程。

    constructor
        In object-oriented programming, a subroutine that is used to create objects. A constructor for a class creates and initializes objects belonging to that class.

        面向对象编程中用于创建对象的子程序。类的构造函数负责创建并初始化属于该类的对象。

    control point
        A point that does not lie on the curve but that is used to help control the shape of the curve. For example, a control point for a Bezier curve segment is used to specify the tangent vector (direction and speed) of the curve at an endpoint.

        一个不在曲线上的点，用于控制曲线的形状。例如，Bezier 曲线的控制点用于确定曲线在端点处的切线方向和速度。


    convex
        A convex geometric shape has the property that whenever two points are contained in the shape, then the line segment between those two points is entirely contained in the shape.

        凸几何形状具有如下性质：若两个点都在该形状内，则连接这两个点的线段也完全位于该形状内。

    coordinates
    coordinate system
        A way of assigning numerical coordinates to geometric points. In two dimensions, each point corresponds to a pair of numbers. In three dimensions, each point corresponds to a triple of numbers.

        将几何点分配数值坐标的方法。在二维中，每个点由一对数值表示；在三维中，则由三个数值表示。

    coordinate systems
        A way of assigning numerical coordinates to geometric points. In two dimensions, each point corresponds to a pair of numbers. In three dimensions, each point corresponds to a triple of numbers.

        将几何点分配数值坐标的方法。在二维中，每个点由一对数值表示；在三维中，则由三个数值表示。

    CPU
        The Central Processing Unit in a computer, the component that actually executes programs. The CPU reads machine language instructions from the computer's memory and carries them out.

        中央处理单元（Central Processing Unit），计算机中执行程序的核心部件。CPU 从内存中读取机器语言指令并执行它们。


    cross product
        A vector product of two 3D vectors. The cross product of v and w is a vector that is perpendicular to both v and w and whose length is equal to the absolute value of the sine of the angle between v and w. If v=(x,y,z) and w=(a,b,c), then their cross product is the vector (yc-zb,za-xc,xb-ya).

        两个三维向量的向量积。v 和 w 的叉积是一个垂直于 v 和 w 的向量，其长度等于 v 和 w 之间夹角的正弦值的绝对值。若 v=(x, y, z)，w=(a, b, c)，则它们的叉积为向量 (yc - zb, za - xc, xb - ya)。


    CSS
        Cascading Style Sheets. A language that is used for specifying the style, or presentation, of the content of web pages. CSS can control things like colors, backgrounds, fonts, shadows, borders, and the size and position of elements of the page.

        层叠样式表（Cascading Style Sheets），用于定义网页内容的样式或呈现形式的语言。CSS 可控制颜色、背景、字体、阴影、边框以及页面元素的大小和位置等。


    cubemap texture
        A texture made up of six images, one for each of the directions positive x, negative x, positive y, negative y, positive z, and negative z. The images are intended to include everything that can be seen from a given point. Cubemap textures are used for environment mapping and skyboxes.

        由六张图像组成的纹理，分别对应正 x、负 x、正 y、负 y、正 z 和负 z 方向。这些图像共同表示从某个点出发所能看到的所有内容。立方体贴图常用于环境映射和天空盒。


    deferred shading
        A multi-pass rendering technique where a first pass processes the geometry and saves relevant information such as transformed coordinates, normal vectors, and material properties. The data can be stored in textures, which are called "geometry buffers" or "G-buffers" in this context. Lighting and other effects can then be computed in additional passes, using the pre-computed information from the geometry buffers instead of re-computing it for each pass.

        一种多通道渲染技术，第一阶段处理几何信息并保存必要数据，如变换后的坐标、法向量和材质属性。这些数据可存储在称为几何缓冲（G-buffer）的纹理中。随后阶段的光照和其它效果可基于几何缓冲中的预计算数据，而无需在每次渲染通道中重复计算。


    depth buffer
        A region of memory that stores the information needed for the depth test in 3D graphics, that is, a depth value for each pixel in the image. Also called the "z-buffer."

        一块内存区域，用于在三维图形中进行深度测试，即为图像中每个像素保存一个深度值。也称为“z-buffer”。


    depth mask
        In WebGL, a setting that controls whether depth values are written to the depth buffer during rendering. When the depth mask is set to false, the depth value is discarded and the depth buffer is unchanged.

        在 WebGL 中，用于控制渲染过程中是否将深度值写入深度缓冲区的设置。若深度掩码设为 false，则丢弃深度值，深度缓冲保持不变。


    depth test
        A solution to the hidden surface problem that involves keeping track of the depth, or distance from the viewer, of the object currently visible at each pixel in the image. When a new object is drawn at a pixel, the depth of the new object is compared to the depth of the current object to decide which one is closer to the viewer. The advantage of the depth test is that objects can be rendered in any order. A disadvantage is that only a limited range of depths can be represented in the image.

        一种解决隐藏面问题的方法，通过跟踪当前图像中每个像素可见对象的深度（即到观察者的距离）来决定是否绘制新对象。当绘制新对象时，会将其深度与当前像素的深度进行比较，以判断哪个对象更靠近观察者。深度测试的优势是对象可以按任意顺序绘制，缺点是图像中可表示的深度范围有限。


    device coordinates
        The coordinate system used on a display device or rendered image, often using pixels as the unit of measure.

        显示设备或渲染图像中使用的坐标系统，通常以像素为单位。

    diffuse color
        A material property that represents the proportion of incident light that is reflected diffusely from a surface.

        一种材质属性，表示表面反射的漫反射光的比例。

    diffuse reflection
        Reflection of incident light in all directions from a surface, so that diffuse illumination of a surface is visible to all viewers, independent of the viewer's position.

        光在表面以各个方向均匀反射的现象，使得表面的漫反射照明在任何观察角度下都可见。

    Direct3D
        Microsoft's proprietary API for 3D graphics on the Windows operating system.

        微软在 Windows 操作系统中用于 3D 图形的专有 API。

    directed acyclic graph
        Also called a "dag." A linked data structure in which there are no cycles. That is, it is not possible to find a sequence of nodes where each node links to the next and the last node links back to the first.

        也称为 "dag"（有向无环图）。一种链式数据结构，不包含任何循环。也就是说，不可能存在一个节点序列，其中每个节点都链接到下一个节点，且最后一个节点又链接回第一个节点。

    directional light
        A light source whose light rays are parallel, all arriving from the same direction. Can be considered to be a light source at an effectively infinite distance. Also called a "sun," since the Sun is an example of a directional light source.

        一种光源，其光线是平行的，全部从同一方向照射而来。可以看作是处于“无限远处”的光源。也称为 “sun”（太阳光），因为太阳就是方向光的一个例子。


    displacement mapping
        A technique used to modify a polygonal mesh by moving, or displacing, the vertices of the mesh.

        一种通过移动（位移）多边形网格顶点来修改该网格的技术。

    display list
        A list of graphics primitives and attributes which can be traversed to create all or part of an image. Display lists were used in some early vector-graphics hardware. They were also available in traditional OpenGL.

        一组图元和属性的列表，可用于遍历并生成全部或部分图像。显示列表曾用于一些早期的矢量图形硬件中，也在传统 OpenGL 中提供支持。


    DOM
        Document Object Model. A specification for representing a web page (and other kinds of structured document) as a tree-like data structure. Can also refer to the data structure itself, as in "the DOM for this web page." A web page can be modified dynamically by manipulating its DOM, using the JavaScript programming language.

        文档对象模型（Document Object Model）。一种将网页（或其他类型结构化文档）表示为类树状数据结构的规范。“DOM”也可指这种数据结构本身，例如“这个网页的 DOM”。网页可以通过使用 JavaScript 编程语言操作其 DOM 实现动态修改。


    dot product
        The dot product of two vectors is the sum of the products of corresponding coordinates. For 3D vectors `v=(x,y,z)` and `w=(a,b,c)`, the dot product of v and w is `x*a+y*b+z*c`. The dot product is equal to the cosine of the angle between the vectors, divided by the product of their lengths.

        两个向量的点积是其对应坐标乘积之和。对于 3D 向量 `v=(x,y,z)` 和 `w=(a,b,c)`，其点积为 `x*a+y*b+z*c`。点积等于两个向量之间夹角的余弦值乘以它们长度的乘积。


    double buffering
        A graphics technique in which an image is drawn off-screen, in a region of memory called an off-screen buffer or "back buffer." When the image is drawn, it can be copied to the buffer that represents the contents of the screen, which is also known as the "front buffer." In true double buffering, the image doesn't have to be copied; instead, the buffers can be "swapped" so that the back buffer becomes the front buffer, and the front buffer becomes the back buffer.

        一种图形技术，图像先在屏幕外的一块内存区域（称为屏幕外缓冲区或“后缓冲区”）中绘制。当图像绘制完成后，可以将其复制到表示屏幕内容的缓冲区（称为“前缓冲区”）中。在真正的双缓冲中，不需要复制，而是通过“交换”缓冲区实现，即将后缓冲变为前缓冲，前缓冲变为后缓冲。


    drawing programs
        A computer program for creating images using vector-style graphics, where the user creates the image by specifying shapes that make up the image and their attributes.

        用于创建矢量图风格图像的计算机程序，用户通过指定构成图像的形状及其属性来绘制图像。


    Eclipse
        An integrated development environment for writing programs in Java (and other programming languages). Eclipse is a free program that can be downloaded from http://eclipse.org.

        一个集成开发环境（IDE），用于编写 Java（及其他编程语言）程序。Eclipse 是一个可从 http://eclipse.org 免费下载的程序。


    emission color
        A material property that represents color that is intrinsic to a surface, rather than coming from light from other sources that is reflected by the surface. Emission color can make the object look like it is glowing, but it does not illuminate other objects. Emission color is often called "emissive color."

        一种材质属性，表示物体表面自身发出的颜色，而非反射其他光源照射到表面的颜色。发射颜色（emission color）可以使物体看起来像是在发光，但它并不会照亮其他物体。发射颜色也常称为“自发光颜色”（emissive color）。


    environment mapping
        A way of simulating mirror-like reflection from the surface of an object. The environment that is to be reflected from the surface is represented as a cubemap texture. To determine what point in the texture is visible at a given point on the object, a ray from the viewpoint is reflected from the surface point, and the reflected ray is intersected with the texture cube. Environment mapping is also called reflection mapping.

        一种模拟物体表面镜面反射效果的方法。被反射的环境由立方体贴图（cubemap texture）表示。为了确定物体表面某点反射后在贴图中对应的位置，会从视点发出一条射线，反射该点后与贴图立方体相交。环境映射也称为反射映射（reflection mapping）。


    ES6
        A version of JavaScript implemented by almost all modern web browsers. More formally known as ECMAScript 6 or ECMAScript 2015. ES6 introduced a large number of new features.

        一种由几乎所有现代网页浏览器实现的 JavaScript 版本。正式名称为 ECMAScript 6 或 ECMAScript 2015。ES6 引入了大量新特性。


    Euclidean transform
        A transform that preserves distances and angles. A Euclidean transform represents a "rigid motion." That is, the transform of an object is an exact copy of the object, with the same size and shape. Any Euclidean transform can be represented as a composition of rotations and translations.

        一种保持距离与角度不变的变换。欧几里得变换（Euclidean transform）表示“刚性运动”，即变换后的对象在大小和形状上与原对象完全一致。任意欧几里得变换都可以表示为一系列旋转与平移的组合。


    Euler angles
        Express the rotation of an object in its own coordinate system, given as individual rotations about the x, y, and z axes in that coordinate system. The cumulative effect of rotations about the three coordinate axes depends on the order in which the rotations are applied.

        用物体自身坐标系中的 x、y、z 轴上的旋转来表示物体的旋转。三个轴上的旋转顺序会影响最终的旋转效果。


    extrusion
        A technique for producing a solid from a 2D shape by moving the shape along a curve in 3D. The solid is the set of points through which the shape passes as it moves along the curve. The most common case is moving the shape along a line segment that is perpendicular to the plane that contains the shape. In practice, in computer graphics, the object that is produced by extrusion is just the surface of the extruded solid.

        一种将二维图形沿三维曲线移动以生成实体的技术。该实体是图形沿曲线移动所经过的点的集合。最常见的情况是沿与图形所在平面垂直的线段移动图形。在计算机图形学中，拉伸生成的对象通常仅是实体的表面。


    eye coordinates
        The coordinate system on 3D space defined by the viewer. In eye coordinates in OpenGL 1.1, the viewer is located at the origin, looking in the direction of the negative z-axis, with the positive y-axis pointing upwards, and the positive x-axis pointing to the right. The modelview transformation maps objects into the eye coordinate system, and the projection transform maps eye coordinates to clip coordinates.

        观察坐标系。在 OpenGL 1.1 中，观察坐标系是由观察者定义的三维坐标系统。观察者位于原点，视线朝向负 z 轴，正 y 轴向上，正 x 轴向右。模型视图变换（modelview transform）将对象转换到观察坐标系，投影变换（projection transform）则将观察坐标转换为裁剪坐标。


    filling a shape
        Drawing the interior of a shape, by coloring the pixels that lie inside the shape. Filling does not apply to shapes, such as lines, that have no interior.

        绘制图形内部的过程，通过为图形内部的像素上色实现。对于线段等没有内部区域的图形，不适用“填充”。

    fixed-function pipeline
        A graphics processing pipeline with a fixed set of processing stages that cannot be modified by a programmer. Data for an image passes through a sequence of processing stages, with the image as the end product. The sequence is called a "pipeline." With a fixed-function pipeline, the programmer can enable and disable stages and set options that control the processing but cannot add to the functionality.

        一种图形处理流水线，其处理阶段是固定的，程序员无法自定义。图像数据经过一系列处理阶段，最终生成图像。这种序列称为“流水线”。在固定功能流水线中，程序员只能启用或禁用某些阶段，设置相关选项，但不能扩展其功能。


    flat shading
        A lighting computation for the faces of a polygon or polygonal mesh that uses the same normal vector at each point in the polygon, giving the polygon a flat or faceted appearance.

        一种对多边形或多边形网格面进行光照计算的方法，该方法在整个多边形上使用相同的法向量，使其呈现出平坦或棱角分明的外观。


    fragment shader
    fragment shaders
        A shader program that will be executed once for each pixel in a primitive. A fragment shader must compute a color for the pixel, or discard it. Fragment shaders are also called pixel shaders.

        在图元中的每个像素上执行的着色器程序。片元着色器必须计算出该像素的颜色，或者丢弃该像素。片元着色器也称为像素着色器（pixel shaders）。


    framebuffer
        In WebGL, a data structure that organizes the buffers for rendering an image, possibly including a color buffer, a depth buffer, and a stencil buffer. A WebGL graphics context has a default framebuffer for on-screen rendering, and additional framebuffers can be created for off-screen rendering.

        在 WebGL 中，用于组织图像渲染所需缓冲区的数据结构，可能包括颜色缓冲区、深度缓冲区和模板缓冲区。WebGL 图形上下文有一个默认帧缓冲区用于屏幕渲染，还可以创建其他帧缓冲区用于离屏渲染。

    frame buffer
        A region of memory that contains color data for a digital image. Most often refers to the memory containing the image that appears on the computer's screen.

        帧缓冲区。用于存储数字图像颜色数据的一块内存区域。最常指代用于显示在计算机屏幕上的图像所对应的内存。


    front face
        One of the two sides of a polygon in 3D. A polygon has two sides. One is taken to be the front face, and the other is the back face. In OpenGL, the difference is determined by the order in which the vertices of the polygon are enumerated. The default is that, seen from the front, the vertices are enumerated in counterclockwise order around the polygon.

        多边形在三维空间中的两个面之一。每个多边形都有正面和背面两个面。在 OpenGL 中，正反面是由多边形顶点的排列顺序决定的。默认情况下，如果从正面观察一个多边形，其顶点以逆时针方向排列。


    frustum
        A truncated pyramid; that is, a pyramid from which the top has been cut off. In OpenGL 1.1, the view volume for a perspective projection is a frustum.

        截头锥体；即一个被截去顶部的金字塔体。在 OpenGL 1.1 中，透视投影的视锥体就是一个截头锥体。


    geometric modeling
        Creating a scene by specifying the geometric objects contained in the scene, together with geometric transforms to be applied to them and attributes that determine their appearance.

        几何建模。通过指定场景中包含的几何对象，以及应用于这些对象的几何变换和描述其外观的属性，来创建一个三维场景。

    primitive
    primitives
    geometric primitive
        Geometric objects in a graphics system, such as OpenGL, that are not made up of simpler objects. Examples in OpenGL include points, lines, and triangles, but the set of available primitives depends on the graphics system. (Note that as the term is used in OpenGL, a single primitive can be made up of many points, line segments, or triangles.)

        几何图元。在图形系统（如 OpenGL）中，不由更简单对象组成的基本几何体。例如，在 OpenGL 中包括点、线和三角形。注意在 OpenGL 的术语中，一个图元本身可以由多个点、线段或三角形构成。


    geometric primitives
        Geometric objects in a graphics system, such as OpenGL, that are not made up of simpler objects. Examples in OpenGL include points, lines, and triangles, but the set of available primitives depends on the graphics system. (Note that as the term is used in OpenGL, a single primitive can be made up of many points, line segments, or triangles.)

        几何图元。在图形系统（如 OpenGL）中，不由更简单对象组成的基本几何体。例如，在 OpenGL 中包括点、线和三角形。注意在 OpenGL 的术语中，一个图元本身可以由多个点、线段或三角形构成。


    transforming
    geometric transform
        A coordinate transformation; that is, a function that can be applied to each of the points in a geometric object to produce a new object. Common transforms include scaling, rotation, and translation.

        几何变换。一个坐标变换函数，可以应用于几何对象中的每个点，从而生成一个新的对象。常见的几何变换包括缩放（scaling）、旋转（rotation）和平移（translation）。


    glMatrix
        An open-source JavaScript library for vector and matrix math in two and three dimensions.

        一个开源的 JavaScript 库，用于二维和三维空间中的向量与矩阵运算。

    global ambient intensity
        In OpenGL, ambient light that is present in the environment independent of any light source. Total ambient light is the sum of the global ambient light plus the ambient light intensity of each enabled light source.

        全局环境光强度。在 OpenGL 中，表示独立于任何光源而存在于整个环境中的环境光。场景中的总环境光等于全局环境光加上所有启用光源的环境光成分。


    global illumination
        The goal of 3D rendering algorithms that take into account all the interactions of light in a scene, including indirect illumination by light that bounces off other objects.

        全局光照。三维渲染算法的目标之一，用于模拟场景中所有光线交互的影响，包括经由物体反射产生的间接照明。


    GLSL
    OpenGL Shading Language
        OpenGL Shader Language, the programming language that is used to write shader programs for use with OpenGL.

        OpenGL 着色语言。用于编写与 OpenGL 搭配使用的着色器程序的编程语言。


    GLTF
        GL Transfer Format. A file format for 3D models. A GLTF file can contain complete 3D scenes, including objects, materials, lights, and even animations. The GLTF specification comes from the Khronos Group, which is also responsible for OpenGL, WebGL, and Vulkan.

        GL 传输格式（GL Transfer Format）。一种用于三维模型的文件格式。GLTF 文件可以包含完整的三维场景，包括对象、材质、光照，甚至动画。GLTF 规范由 Khronos Group 提出，该组织也是 OpenGL、WebGL 和 Vulkan 的制定方。


    GLU
        The OpenGL Utility library. Defines several functions for use with older versions of OpenGL, including gluPerspective and gluLookAt. Not to be confused with GLUT. GLU is a standard part of OpenGL.

        OpenGL 实用工具库（OpenGL Utility library）。为旧版本 OpenGL 提供辅助函数的库，如 `gluPerspective` 和 `gluLookAt`。不要与 GLUT 混淆。GLU 是 OpenGL 的标准组成部分。


    GLUT
        The OpenGL Utility Toolkit. A platform-independent library for writing OpenGL applications. OpenGL does not include support for windows or events. GLUT adds such support. It also has functions for drawing 3D shapes such as spheres and polyhedra (not to mention a teapot). GLUT is written in the C programming language and is used with the C API for OpenGL. However, many GLUT functions are also available in JOGL, the Java API for OpenGL. A newer, and somewhat improved, version of the toolkit named "FreeGLUT" is commonly used in place of the original version.

        OpenGL 工具包（OpenGL Utility Toolkit）。一个平台无关的库，用于编写 OpenGL 应用程序。OpenGL 本身不包含窗口或事件支持，GLUT 为此提供支持。它还提供绘制三维形状（如球体、多面体，甚至茶壶）的函数。GLUT 使用 C 语言编写，配合 OpenGL 的 C API 使用。不过，许多 GLUT 函数也在 JOGL（Java 的 OpenGL API）中可用。一个较新的改进版本称为 FreeGLUT，常作为原始 GLUT 的替代品使用。


    GPU
        Graphics Processing Unit, a computer hardware component that performs graphical computations that create and manipulate images. Operations such as drawing a line on the screen or rendering a 3D image are done in the GPU, which is optimized to perform such operations very quickly.

        图形处理单元（Graphics Processing Unit）。一种用于执行图形计算以生成和处理图像的计算机硬件组件。GPU 可以快速执行诸如在屏幕上绘制线条或渲染三维图像等操作，并对此类任务进行了专门优化。


    gradient
        A pattern of color produced by assigning colors to certain reference points and computing color for other points by interpolating or extrapolating colors from the reference points. The effect is a color progression along line segments between reference points. Different rules for extending the colors beyond those lines produce different types of gradient, such as linear gradients and radial gradients.

        渐变。通过为一些参考点指定颜色，并对其他点通过插值或外推计算颜色，从而生成颜色过渡的图案。颜色沿参考点之间的线段平滑过渡。根据颜色扩展规则的不同，常见的渐变类型包括线性渐变和径向渐变。


    grayscale
        Refers to a color scheme or image in which each color is a shade of gray (where the term "shade of gray" here includes black and white). Typically, 256 shades of gray are used. Grayscale is also called "monochrome."

        灰度。表示图像或颜色方案中，每个颜色都是某种灰色（“灰色”包括黑和白）。典型情况下有 256 个灰度级。灰度图像也称为“单色图像”（monochrome）。


    GUI
        (Graphical User Interface.) A user interface for a program where the user interacts with the program using components such as windows, menus, buttons, and text-input boxes.

        图形用户界面（Graphical User Interface）。一种程序的用户界面形式，用户通过窗口、菜单、按钮、文本输入框等图形组件与程序交互。


    HDR image
        A high dynamic range image. An HDR image has more color information than the usual eight bits per color channel per pixel. This makes it more suitable to uses that require calculation with the color values.

        高动态范围图像（High Dynamic Range image）。相比每通道每像素仅 8 位的普通图像，HDR 图像包含更多的颜色信息，因此更适用于需要对颜色值进行计算的应用场景。


    height map
        An image in which the grayscale value represents a height, or elevation. Height maps can be used in displacement mapping to specify the amount of displacement.

        高度图。一种图像，其灰度值代表高度或海拔。高度图常用于位移贴图（displacement mapping）中，指定顶点的偏移量。

    hidden surface problem
        The problem in 3D graphics of deciding which object is visible at each pixel in an image. When one object is behind another object from the point of view of the viewer, only the front object should appear in the image. A rendering algorithm for 3D graphics must satisfy this constraint. Algorithms that solve the hidden surface problem include the painter's algorithm and the depth test algorithm.

        三维图形中的一个问题，即确定图像中每个像素处哪些物体是可见的。当某个物体位于另一个物体之后（从观察者视角来看），图像中应只显示前方的物体。三维图形的渲染算法必须满足这一可见性约束。解决隐藏面问题的算法包括“画家算法（painter's algorithm）”和“深度测试算法（depth test algorithm）”。


    hierarchical modeling
        Creating complex geometric models in a hierarchical fashion, starting with geometric primitives, combining them into components that can then be further combined into more complex components, and so on.

        以分层方式创建复杂几何模型的过程，先由几何图元开始组合为组件，再将组件进一步组合为更复杂的组件，依此类推。


    homogeneous coordinates
        A way of representing n-dimensional vectors as (n+1)-dimensional vectors where two (n+1) vectors represent the same n-dimensional vector if they differ by a scalar multiple. In 3D, for example, if w is not zero, then the homogeneous coordinates (x,y,z,w) are equivalent to homogeneous coordinates (x/w,y/w,z/w,1), since they differ by multiplication by the scalar w. Both sets of coordinates represent the 3D vector (x/w,y/w,z/w)

        一种将 n 维向量表示为 (n+1) 维向量的方法，其中两个 (n+1) 维向量若仅相差一个标量倍数，则表示相同的 n 维向量。例如在三维中，如果 w 不为零，则齐次坐标 (x, y, z, w) 等价于齐次坐标 (x/w, y/w, z/w, 1)，因为它们仅相差一个标量 w。这两个坐标都表示 3D 向量 (x/w, y/w, z/w)。


    HSL
    HSL color
        A color specified by three numbers giving the hue, saturation, and lightness of the component. The HSL color model is similar to the HSV color model. The main difference is that in HSL, pure spectral colors occur when L=0.5, while in HSV, they occur when V=1.

        一种使用三个数值来表示色相（hue）、饱和度（saturation）和亮度（lightness）的颜色。HSL 颜色模型与 HSV 类似，主要区别在于：在 HSL 中，当 L=0.5 时为纯光谱色；而在 HSV 中，纯光谱色出现在 V=1 时。


    HSV
    HSV color
        A color specified by three numbers giving the hue, saturation, and value of the component. The hue represents the basic color. The saturation is the purity of the color, with a saturation value of zero producing a shade of gray, that is a color with no actual hue at all. The value represents the brightness of the color, with a value of zero giving black. (Value is also called brightness, and the name HSB is sometimes used instead of HSV.)

        一种使用三个数值来表示色相（hue）、饱和度（saturation）和值（value）的颜色。色相表示基本颜色；饱和度表示颜色的纯度，饱和度为 0 时为灰色（即不具有实际色相的颜色）；值表示颜色的亮度，值为 0 时表示黑色。Value 有时也称为亮度（brightness），因此 HSV 有时也称为 HSB。


    HTML
        HyperText Markup Language. A language that is used for specifying the content of web pages. An HTML document is made up of text, along with "elements" for adding other content, such as images, and for defining the structure of the document. Because of nesting of elements, the document can be represented by a tree-like data structure.

        超文本标记语言（HyperText Markup Language）。用于指定网页内容的语言。HTML 文档由文本和“元素”构成，元素可用于嵌入图像等内容，以及定义文档的结构。由于元素具有嵌套性，HTML 文档可表示为一棵树形数据结构。


    HTML canvas
        A canvas element on a web page. The canvas appears as a rectangular area on the page. The JavaScript programming language can use a canvas element as a drawing surface. HTML is a language for specifying the content of a web page. JavaScript is the programming language for web pages. The canvas element supports a 2D graphics API. In many browsers, it also supports the 3D graphics API, WebGL.

        网页中的 canvas 元素。canvas 以矩形区域形式出现在页面上。JavaScript 可将其用作绘图表面。HTML 负责网页内容的定义，而 JavaScript 是网页的编程语言。canvas 元素支持 2D 图形 API，并在许多浏览器中也支持 3D 图形 API（如 WebGL）。


    identity matrix
        The n-by-n identity matrix is an n-by-n matrix which has ones on the diagonal and zeros elsewhere. Multiplication of any matrix B by the identity matrix, in either order, leaves B unchanged. Multiplication of an n-dimensional vector by the n-by-n identity matrix leaves the vector unchanged; that is, the identity matrix is the matrix for the identity transformation.

        n×n 单位矩阵是一个主对角线为 1、其余元素为 0 的 n×n 矩阵。将任意矩阵 B 与单位矩阵相乘（无论左右顺序），结果仍为 B。将 n 维向量与 n×n 单位矩阵相乘也保持向量不变，即单位矩阵表示恒等变换。


    identity transform
        A transform that has no effect on its argument. For example, the identity transform in 2D is given by the formula I(x,y) = (x,y). The identity transform I has the property that if T is any transform, then I followed by T is the same as T, and T followed by I is the same as T.

        对输入无任何作用的变换。例如，在二维中，恒等变换 I(x, y) = (x, y)。恒等变换 I 具有如下性质：若 T 是任意变换，则 I 后接 T 与 T 等价，T 后接 I 也与 T 等价。


    image texture
        An image that is applied to a surface as a texture, so that it looks at if the image is "painted" onto the surface.

        贴附在表面上的图像，用作纹理，使图像看起来像是被“绘制”在该表面上一样。


    index buffer
        In WebGPU, an index buffer is a GPU buffer that holds vertex indices for use with the drawIndexed(). A vertex index gives the position of a vertex in the list of vertices of a primitive.

        在 WebGPU 中，索引缓冲区是一种 GPU 缓冲区，用于存储顶点索引，并与 drawIndexed() 函数配合使用。顶点索引给出图元顶点列表中各个顶点的位置。


    indexed color
        A color scheme in which colors are selected from a limited palette of colors. For example, if the palette contains 256 colors, then a color can be specified by an eight-bit integer, giving its position, or index, in the list of colors.

        一种使用有限调色板选择颜色的颜色方案。例如，当调色板包含 256 种颜色时，每种颜色可用一个 8 位整数来表示，其值表示颜色在调色板中的位置（索引）。


    indexed drawing
        In WebGPU, drawing a primitive using the drawIndexed() function. With that function, vertices are not generated in the order in which they are listed. Instead, a list of vertex indices in an index buffer determines the order of the vertices. Indexed drawing is used to render indexed face sets.

        在 WebGPU 中，使用 drawIndexed() 函数进行图元绘制。该函数不按顶点列表中的顺序生成顶点，而是由索引缓冲区中的索引列表确定顶点顺序。索引绘制通常用于渲染“索引面集合（indexed face sets）”。


    indexed face set
        (IFS). A data structure that represents a polyhedron or polygonal mesh. The data structure includes a numbered list of vertices and a list of faces. A face is specified by listing the indices of the vertices of the face; that is, a face is given as a list of numbers where each number is an index into the list of vertices.

        （IFS）一种表示多面体或多边形网格的数据结构。该结构包含一个带编号的顶点列表和一个面列表。每个面通过列出其顶点的索引来指定，即每个面由一组索引值表示，这些索引值对应于顶点列表中的顶点位置。


    instanced drawing
        The ability to render multiple versions of a primitive with a single function call. Each copy can have its own values for certain attributes, such as color or transformation.

        一种通过一次函数调用渲染多个图元副本的能力。每个副本可以具有独立的属性值，如颜色或几何变换等。


    intensity of a light source
        A light source emits light at various wavelengths. The intensity of a light at a given wavelength is the amount of energy in the light at that wavelength. The total intensity of the light is its total energy at all wavelengths. The color of a light is determined by its intensities at all wavelengths.

        光源在不同波长下发出光的强度。某个波长上的强度指的是该波长上的光能量。光的总强度是所有波长能量之和。光的颜色由各波长上的强度分布决定。


    interpolation
        Given values for some quantity at certain reference points, computing a value for that quantity at other points by some kind of averaging applied to the values at the reference points.

        已知某些参考点上的数值，通过某种平均方式推算其他点上的数值的过程，称为插值。

    invariant qualifier
        In GLSL, a modifier that ensures that when the same expression is used to compute the value of a variable in two different shaders, the value will be the same in both shaders. This can be important for multi-pass algorithms, where several shader programs are applied in succession to render one image.

        在 GLSL 中，一种修饰符，用于确保在两个不同的着色器中使用相同表达式计算变量值时，所得结果也相同。这在多通道算法中非常重要，该类算法通常需要多个着色器程序连续执行以完成图像渲染。


    inverse transform
        Given a transform T, the inverse transform of T is a transform that reverses the operation of T. For example, for a 2D transform, for R to be the inverse of T means that R(T(x,y)) = (x,y). Scaling by 0.5 is the inverse of scaling by 2. Translation by (-3,5) is the inverse of translation by (3,-5). Not every transform has an inverse. For example, scaling by a factor of zero has no inverse.

        给定变换 T，其逆变换是能逆转 T 效果的变换。例如，对于二维变换，若 R 是 T 的逆变换，则满足 R(T(x, y)) = (x, y)。如缩放因子 2 的缩放，其逆为缩放因子 0.5；平移 (3, -5) 的逆为平移 (-3, 5)。并非所有变换都有逆，如因子为 0 的缩放没有逆变换。


    IOR
        Index of Refraction. A property of a medium, such as air or glass, that transmits light. The refraction, or bending, of light rays that pass from one medium to another depends on the ratio of the IORs of the two media. The index of refraction of a medium depends on the speed of light in that medium.

        折射率（Index of Refraction）。表示介质（如空气、玻璃）透光特性的一个物理量。光线从一种介质进入另一种介质时，其折射角取决于两种介质折射率的比值。介质的折射率取决于光在该介质中的传播速度。

    JavaScript
        A programming language for web pages. JavaScript code on a web page is executed by a web browser that displays the page, and it can interact with the contents of the web page and with the user. There are JavaScript APIs for 2D and for 3D graphics

        一种用于网页的编程语言。网页上的 JavaScript 代码由显示该网页的浏览器执行，能够与网页内容及用户进行交互。JavaScript 提供了用于 2D 和 3D 图形的 API。


    JOGL
        A Java implementation of OpenGL. JOGL is very complicated, since it attempts to support all versions of OpenGL in one programming system. JOGL integrates seamlessly with Java's Swing and AWT graphics.

        一种基于 Java 的 OpenGL 实现。由于试图在一个编程系统中支持所有版本的 OpenGL，JOGL 本身非常复杂。它可与 Java 的 Swing 和 AWT 图形系统无缝集成。


    JSON
        (JavaScript Object Notation.) A syntax for representing JavaScript objects as strings, similar to the object literal syntax that is used in JavaScript. JSON objects cannot contain functions, but they can contain strings, numbers, and booleans. JSON has become a popular standard for storage and transmission of structured data.

        （JavaScript Object Notation，JavaScript 对象表示法。）一种将 JavaScript 对象表示为字符串的语法，类似于 JavaScript 中的对象字面量语法。JSON 对象不能包含函数，但可以包含字符串、数字和布尔值。JSON 已成为用于结构化数据存储与传输的流行标准。


    keyframe animation
        An animation technique in which the value of some quantity is given explicitly only at certain times during the animation. The times when the quantity is specified are called keyframes. Between keyframes, the value of the quantity is obtained by interpolating between the values specified for the keyframes.

        一种动画技术，其中某个量的取值只在动画过程中的某些时间点被明确指定。这些时间点被称为关键帧（keyframe）。在关键帧之间，该量的取值通过对关键帧上的值进行插值得出。


    Lambert shading
        A technique for computing pixel colors on a primitive using a lighting equation that takes into account ambient and diffuse reflection. In Lambert shading, the lighting equation is applied only at the vertices of the primitive. Color values for pixels in the primitive are calculated by interpolating the values that were computed for the vertices. Lambert shading is named after Johann Lambert, who developed the theory on which it is based in the eighteenth century.

        一种基于光照方程、并考虑环境光与漫反射的像素颜色计算技术。在 Lambert 着色中，光照方程只在图元的顶点处进行计算，像素颜色通过对顶点颜色值进行插值获得。Lambert 着色法以十八世纪提出该理论的约翰·兰伯特（Johann Lambert）命名。


    lathing
        A technique for producing a surface by rotating a planar curve about a line that lies in the same plane as the curve. As each point rotates about the line, it generates a circle. The surface is the union of the circles generated by all the points on the curve. Lathing imitates shapes that can be produced by a mechanical lathe.

        一种通过绕位于平面内的直线旋转平面曲线来生成曲面的技术。每个点绕直线旋转会生成一个圆，这些圆的集合构成了最终曲面。Lathing 模拟了机械车床可加工出的形状。


    length of a vector
        A vector is defined by its length and its direction, so length is a fundamental property. When a vector is represented as an arrow, its length is just the length of that arrow. For a 2D vector given by coordinates (x,y), the length is the square root of `x*x+y*y`. For a 3D vector given as (x,y,z), the length is the square root of `x*x+y*y+z*z`.

        向量由其长度与方向定义，因此长度是基本属性。当向量表示为箭头时，其长度就是箭头的长度。对于二维向量 (x,y)，长度为 `sqrt(x*x + y*y)`；对于三维向量 (x,y,z)，长度为 `sqrt(x*x + y*y + z*z)`。


    lighting
        Using light sources in a 3D scene, so that the appearance of objects in the scene can be computed based on the interaction of light with the objects' material properties.

        在三维场景中引入光源，从而能够根据光与物体材质属性之间的相互作用来计算物体的可见外观。


    lighting equation
        The equation that is used in OpenGL to compute the visible color of a point on a surface from the material properties of the surface, the normal vector for that point, the direction to the viewer, the ambient light level, and the direction and intensity of light sources.

        OpenGL 中用于根据表面材质属性、法向量、观察方向、环境光水平、以及光源方向与强度来计算表面某点可见颜色的光照方程。


    linear algebra
        The field of mathematics that studies vector spaces and linear transformations between them. Linear algebra is part of the essential mathematical foundation of computer graphics.

        研究向量空间及其之间的线性变换的数学分支。线性代数是计算机图形学的基础数学组成部分之一。

    linear gradient
        A color gradient pattern in which there is a color variation along a certain line, with constant color along lines perpendicular to that line.

        一种颜色渐变模式，其中颜色沿某条线连续变化，并在垂直于该线的方向上保持不变。

    linear transformation
        A function from one vector space to another that preserves vector addition and multiplication by constants. Linear transformations can be represented by matrices. In computer graphics, they are used to implement geometric operations such as rotation and translation.

        从一个向量空间到另一个向量空间的函数，保持向量加法与标量乘法不变。线性变换可用矩阵表示。在图形学中用于实现几何操作，例如旋转与平移。


    lossless data compression
        A scheme for reducing the size of a dataset without losing any of the information in that dataset. The original data can be recovered exactly from the compressed data. The image formats GIF and PNG use lossless data compression to reduce the size of the image file.

        一种无信息损失的数据压缩方案，可在不丢失任何原始信息的前提下减小数据体积。原始数据可从压缩数据中精确恢复。GIF 与 PNG 图像格式采用无损压缩来减小文件大小。


    lossy data compression
        A scheme for reducing the size of a dataset in which some of the information in the dataset can be lost. The data that is recovered from the compressed data can differ from the original data. The image format JPEG use lossy data compression to reduce the size of the image file.

        一种压缩数据时可能丢失部分信息的方案。从压缩数据中恢复得到的数据可能与原始数据不同。JPEG 图像格式采用有损压缩来减小图像文件体积。


    luminance
        A quantity representing the perceived brightness of a color. For an RGB color, it is a weighted average of the red, green, and blue components of the color. The usual formula is `0.3*red + 0.59*green + 0.11*blue`.

        表示颜色感知亮度的一个量。对于 RGB 颜色，它是红、绿、蓝分量的加权平均值。常用公式为：`0.3*red + 0.59*green + 0.11*blue`。


    magnification filter
        An operation that is used when applying a texture to an object, when the texture has to be stretched to fit the object. For an image texture, a magnification filter is applied to compute the color of a pixel when that pixel covers just a fraction of a pixel in the image.

        将纹理应用于物体时，如果纹理需要放大以适应物体，所使用的处理操作。对于图像纹理，当像素仅覆盖图像的部分像素时，放大滤波器用于计算该像素的颜色。


    material
        The properties of an object that determine how that object interacts with light in the environment. Material properties in OpenGL include, for example, diffuse color, specular color, and shininess.

        决定物体如何与环境光交互的属性。在 OpenGL 中，材质属性包括例如漫反射颜色、高光颜色与光滑度等。


    matrix
        A rectangular array of numbers. A matrix can be represented as a two-dimensional array, with numbers arranged in rows and columns. An N-by-N matrix represents a linear transformation from N-dimensional space to itself.

        数字构成的矩形数组。矩阵可表示为二维数组，由行与列组成。一个 N×N 的矩阵表示从 N 维空间到其自身的线性变换。


    matrix mode
        In OpenGL 1.1, a state variable that determines which one of several transformation matrices will be affected by functions such as glRotatef and glFrustum. The matrix mode is set with the function glMatrixMode. Possible values include GL_MODELVIEW, GL_PROJECTION, and GL_TEXTURE.

        在 OpenGL 1.1 中，一种状态变量，用于指定哪些变换矩阵会受 glRotatef 与 glFrustum 等函数的影响。该模式通过 glMatrixMode 函数设置。可选值包括 GL_MODELVIEW、GL_PROJECTION 和 GL_TEXTURE。


    Metal
        Apple's proprietary API for 3D graphics and computation on MacOS computers and iOS devices.

        Apple 公司在 macOS 与 iOS 设备上用于 3D 图形与计算的专有 API。

    minification filter
        An operation that is used when applying a texture to an object, when the texture has to be shrunk to fit the object. For an image texture, a minification filter is applied to compute the color of a pixel when that pixel covers several pixels in the image.

        将纹理应用于物体时，如果纹理需要缩小以适应物体，所使用的处理操作。对于图像纹理，当一个像素覆盖多个图像像素时，缩小滤波器用于计算该像素的颜色。


    mipmap
        One of a series of reduced-size copies of a texture image, of decreasing width and height. Starting from the original image, each mipmap is obtained by dividing the width and height of the previous image by two (unless it is already 1). The final mipmap is a single pixel. Mipmaps are used for more efficient mapping of the texture image to a surface, when the image has to be shrunk to fit the surface.

        一系列逐级缩小尺寸的纹理图像副本。从原始图像出发，每一级 mipmap 的宽高均为上一图像宽高的一半（除非已为 1）。最终的 mipmap 是单个像素。Mipmap 用于在纹理映射缩小时提高效率。

    mipmaps
        One of a series of reduced-size copies of a texture image, of decreasing width and height. Starting from the original image, each mipmap is obtained by dividing the width and height of the previous image by two (unless it is already 1). The final mipmap is a single pixel. Mipmaps are used for more efficient mapping of the texture image to a surface, when the image has to be shrunk to fit the surface.

        一系列逐步缩小尺寸的纹理图像副本之一，其宽度和高度依次递减。从原始图像开始，每个 mipmap 都是通过将前一个图像的宽度和高度除以二得到的（除非其尺寸已经为 1）。最终的 mipmap 是一个单像素图像。mipmap 用于在图像需缩小以适配表面时，提高纹理映射的效率。


    modeling transformation
        A transformation that is applied to an object to map that object into the world coordinate system or into the object coordinate system for a more complex, hierarchical object.

        应用于对象的变换，用于将对象映射到世界坐标系中，或映射到更复杂的分层对象的对象坐标系中。


    modelview transformation
        In OpenGL 1.1, a transform that combines the modeling transform with the viewing transform. That is, it is the composition of the transformation from object coordinates to world coordinates and the transformation from world coordinates to eye coordinates. Because of the equivalence between modeling and viewing transformations, world coordinates are not really meaningful for OpenGL, and only the combined transformation is tracked.

        在 OpenGL 1.1 中，将建模变换与视图变换结合的变换。它是从对象坐标到世界坐标的变换与从世界坐标到视点（eye）坐标的变换的复合。由于建模和视图变换的等价性，OpenGL 实际上并不明确使用世界坐标系，仅跟踪组合后的变换。


    multi-pass algorithm
        A rendering algorithm that draws a scene several times and combines the results somehow to compute the final image. A simple example is anaglyph stereo, in which a left-eye and right-eye image of the scene are rendered separately and combined.

        一种渲染算法，通过多次绘制场景并以某种方式组合结果来计算最终图像。一个简单的示例是立体红蓝眼镜（anaglyph stereo）技术，其中左眼和右眼视角的图像分别渲染并组合显示。


    multisampling
        A kind of antialiasing where the fragment shader is evaluated at several points in each pixel, and the results are averaged to get the color of the pixel.

        一种抗锯齿技术，其中片段着色器会在每个像素内的多个点上执行，并对结果进行平均以确定像素颜色。


    NDC
        Normalized Device Coordinates. In WebGPU, refers to the default xyz coordinate system in which x and y range from -1 to 1 and z ranges from 0 to 1. The x and y in NDC map linearly to device, or pixel, coordinates on the viewport.

        归一化设备坐标（Normalized Device Coordinates）。在 WebGPU 中，指默认的 xyz 坐标系，其中 x 和 y 的范围是 [-1, 1]，z 的范围是 [0, 1]。NDC 中的 x 和 y 与设备坐标（像素）在视口中线性映射。


    nio buffer
        A Java object belonging to the class java.nio.Buffer or one of its subclasses. Nio buffers are similar to arrays, but they are optimized for input/output operations. Nio buffers are used instead of arrays for certain purposes in Java's JOGL API for OpenGL.

        Java 中属于类 `java.nio.Buffer` 或其子类的对象。NIO 缓冲区与数组相似，但针对输入/输出操作进行了优化。在 Java 的 JOGL API 中，NIO 缓冲区被用于替代数组以支持某些操作。


    normalized vector
        The result of dividing a non-zero vector by its length, giving a unit vector, that is, a vector of length one. (Note that "normalized vector" and "normal vector" are, confusingly, unrelated terms!)

        将一个非零向量除以其长度后得到的单位向量，即长度为 1 的向量。（注意“normalized vector”（归一化向量）和“normal vector”（法向量）这两个术语虽然相似，但含义无关。）


    normal vector
        A normal vector to a surface at a point on that surface is a vector that is perpendicular to the surface at that point. Normal vectors to curves are defined similarly. Normal vectors are important for lighting calculations.

        曲面某点的法向量是该点处垂直于曲面的向量。对曲线而言，法向量的定义类似。法向量在光照计算中非常重要。


    norm of a vector
        Another term for the length of the vector. For a 3D vector given as (x,y,z), the norm is the square root of `x*x+y*y+z*z`.

        向量的范数，等同于向量的长度。对于给定坐标为 (x, y, z) 的 3D 向量，其范数为 `sqrt(x*x + y*y + z*z)`。


    object coordinates
        The coordinate system in which the coordinates for points in an object are originally specified, before they are transformed by any modeling or other transform that will be applied to the object.

        对象中点的初始坐标所在的坐标系，在建模变换或其他变换应用前使用的坐标系统。

    off-screen canvas
        My term for a segment of the computer's memory that can be used as a drawing surface, for drawing images that are not visible on the screen. Some method should exist for copying the image from an off-screen canvas onto the screen. In Java, for example, an off-screen canvas can be implemented as an object of type BufferedImage.

        指计算机内存中可作为绘图表面的区域，用于绘制在屏幕上不可见的图像。应有方法将离屏画布中的图像复制到屏幕上。例如在 Java 中，可使用 `BufferedImage` 类型对象实现离屏画布。


    OpenGL
        A family of computer graphics APIs that is implemented in many graphics hardware devices. There are several versions of the API, and there are implementations, or "bindings" for several different programming languages. Versions of OpenGL for embedded systems such as mobile phones are known as OpenGL ES. WebGL is a version for use on Web pages. OpenGL can be used for 2D as well as for 3D graphics, but it is most commonly associated with 3D.

        一个图形 API 家族，在许多图形硬件设备中实现。OpenGL 有多个版本，也有多个编程语言的绑定（bindings）。面向嵌入式系统（如手机）的版本称为 OpenGL ES，用于网页的版本称为 WebGL。OpenGL 可用于 2D 和 3D 图形，但通常与 3D 图形联系更为紧密。


    orthographic projection
        A projection from 3D to 2D that simply discards the z-coordinate. It projects objects along lines that are orthogonal (perpendicular) to the xy-plane. In OpenGL 1.1, the view volume for an orthographic projection is a rectangular solid.

        一种将 3D 投影为 2D 的方式，直接丢弃 z 坐标。该投影沿垂直于 xy 平面的直线进行。在 OpenGL 1.1 中，正交投影的视图体是一个矩形立方体。


    painter's algorithm
        A solution to the hidden surface algorithm that involves drawing the objects in a scene in order from back to front, that is, in decreasing order of distance from the viewer. A disadvantage is that the order is usually not well-defined unless some objects are decomposed into smaller sub-objects. Another issue is that the order of drawing has to change when objects move or when the point of view changes.

        一种隐藏面消除算法，通过按从远到近的顺序绘制场景中的对象实现，即根据对象与视点的距离降序绘制。其缺点是除非将对象拆分为更小的子对象，否则绘制顺序通常不唯一；另外，当对象移动或视角变化时，绘制顺序也必须更新。


    painting programs
        A computer program for creating images using raster-style graphics, where the user creates the image by controlling the colors of each pixel.

        用于创建图像的计算机程序，采用栅格图形风格，用户通过控制像素颜色来绘制图像。


    path tracing
        A rendering algorithm based on the idea of computing all the paths that light could have followed to arrive at the position of a viewer from each direction. Since that is literally impossible, the algorithm traces a random sample of paths and averages the results. As the number of samples increases, the average converges to a very high-quality image.

        一种基于计算光线从各个方向到达观察者位置可能路径的渲染算法。由于枚举所有路径在实践中不可行，该算法会随机采样若干路径并对结果求平均。随着样本数量的增加，平均值逐渐收敛为高质量图像。


    pattern fill
        Using copies of an image to fill the interior of a two-dimensional shape. The image can be repeated horizontally and vertically as necessary to cover the shape.

        使用图像副本填充二维图形的内部。图像可在水平和垂直方向上重复以覆盖整个形状。

    PBR
        Physically Based Rendering. A general term encompassing a variety of techniques for rendering materials that look more physically realistic than the materials traditionally used in OpenGL and similar graphics APIs. The idea is to implement the actual physics of light and material more directly. PBR has become common in real-time graphics such as video games.

        基于物理的渲染（Physically Based Rendering）。泛指一类渲染技术，其材质效果比 OpenGL 等传统图形 API 所用材质更接近物理现实。其核心思想是更直接地模拟光与材料之间的真实物理行为。PBR 在实时图形（如视频游戏）中已成为主流。


    Perlin noise
        A technique invented by Ken Perlin in 1983 that is used in the computation of natural-looking procedural textures. A Perlin noise function has numerical inputs (usually 2 or 3) and produces an output number in the range -1.0 to 1.0. The output is pseudo-random, but has some regularity, with features that are similarly sized and regularly distributed, and with variation on several scales.

        一种由 Ken Perlin 于 1983 年发明的技术，用于生成具有自然外观的程序纹理。Perlin 噪声函数接受数值输入（通常为 2 或 3 个维度），输出范围为 -1.0 到 1.0 的数值。其输出为伪随机，但具有一定规律性：特征尺寸相近、分布均匀，并且具备多尺度变化。


    per-pixel lighting
        Doing lighting calculations at each pixel of a primitive, which gives better results in most cases than per-vertex lighting. Phong shading uses per-pixel lighting, with normal vectors interpolated from the vertices.

        在图元的每个像素级别进行光照计算，在多数情况下比每顶点光照效果更好。Phong 着色模型即使用逐像素光照，通过从顶点插值得到像素的法向量。

    perspective projection
        A projection from 3D to 2D that projects objects along lines radiating out from a viewpoint. A perspective projection attempts to simulate realistic viewing. A perspective projection preserves perspective; that is, objects that are farther from the viewpoint are smaller in the projection. In OpenGL 1.1, the view volume for a perspective projection is a frustum, or truncated pyramid.

        一种从 3D 到 2D 的投影方式，将物体沿从视点辐射出的直线进行投影。透视投影试图模拟现实中的视觉效果，具有保持透视的特性；即，距离视点越远的物体在投影中越小。在 OpenGL 1.1 中，透视投影的视景体是一个截头四棱锥（frustum）。


    per-vertex lighting
        Doing lighting calculations only at the vertices of a primitive, and interpolating the results to get the colors of interior pixels. Per-vertex lighting is the standard in traditional OpenGL. Per-vertex lighting without specular reflection is Lambert shading.

        仅在图元的顶点处执行光照计算，并通过插值得到图元内部像素的颜色。顶点光照是传统 OpenGL 中的标准方式。不包含镜面反射的顶点光照称为 Lambert 着色。


    Phong shading
        A technique for computing pixel colors on a primitive using a lighting equation that takes into account ambient, diffuse, and specular reflection. In Phong shading, the lighting equation is applied at each pixel. Normal vectors are specified only at the vertices of the primitive. The normal vector that is used in the lighting equation at a pixel is obtained by interpolating the normal vectors for the vertices. Phong shading is named after Bui Tuong Phong, who developed the theory in the 1970s.

        一种使用光照方程计算图元像素颜色的技术，该方程考虑了环境光、漫反射和镜面反射。在 Phong 着色中，光照方程在每个像素处执行。法向量只在图元的顶点处指定，用于某像素的法向量由顶点法向量插值得出。Phong 着色得名于 20 世纪 70 年代提出该理论的 Bui Tuong Phong。


    pipeline
        A sequence of computational stages in a GPU that are applied to incoming data to produce some result. Some of the stages can be programmable shaders, such as vertex shaders, fragment shaders, and compute shaders. In a graphics rendering pipeline, the output is the colors of the pixels in an image.

        GPU 中的一系列计算阶段序列，应用于输入数据以产生某种输出结果。其中某些阶段可以是可编程着色器，例如顶点着色器、片段着色器和计算着色器。在图形渲染流水线中，最终输出是图像中的像素颜色。


    pixel
        A digital image is made up of rows and columns of small rectangles called pixels. To specify a digital image, a color is assigned to each pixel in the image.

        数字图像由若干行和列的小矩形组成，这些小矩形称为像素。描述一幅数字图像时，需要为图像中的每个像素指定颜色。


    pixels
        A digital image is made up of rows and columns of small rectangles called pixels. To specify a digital image, a color is assigned to each pixel in the image.

        数字图像由若干行和列的小矩形组成，这些小矩形称为像素。描述一幅数字图像时，需要为图像中的每个像素指定颜色。


    point light
        A light source whose light rays emanate from a single point. Also called a "lamp," since a lamp approximates a point source of light. Also called a positional light.

        一种从单个点发出光线的光源。也称为“灯光”（lamp），因为台灯可近似看作点光源。也称为位置光源（positional light）。


    polygon
        A multi-sided shape lying in a plane and specified by a list of points, called its vertices, and made up of the line segments from each point in the list to the next point in the list, plus a line segment from the last point in the list to the first point. All the points are required to lie in the same plane. Sometimes the term "polygon" includes the interior of the shape as well as its boundary.

        位于同一平面上的多边形图形，由若干点（称为顶点）定义，边为相邻顶点之间的线段，最后一个点与第一个点之间也有一条边。所有点必须共面。有时“polygon”也指包括内部区域的多边形。


    polygonal mesh
        A collection of polygons, where the polygons can be joined together along their edges. A polygonal mesh can represent a polyhedron, or can be used as an approximation for a curved surface. A polygonal mesh can be represented as an indexed face set.

        多边形的集合，其中各多边形可在边界处连接。多边形网格可表示多面体，或作为曲面的一种近似。多边形网格可使用索引面集（indexed face set）表示。


    polygon offset
        A 3D graphics technique that slightly increases or decreases the depth of the pixels in a primitive as it is rendered. Polygon offset is used to avoid having several objects at exactly the same depth, a situation that is not handled well by the depth test.

        一种 3D 图形技术，在渲染图元时轻微改变其像素的深度值。用于避免多个对象深度完全相同时出现的深度测试问题。


    polyhedron
        A closed 3D figure whose faces, or sides, are polygons. Usually, it is assumed that the faces of a polyhedron do not intersect, except along their edges.

        一个封闭的三维几何体，其面由多边形组成。通常假设其面之间仅在边处相交。

    power-of-two texture
        A texture image whose width and height are powers of two. In some graphics systems, this is a requirement of any image that is to be used as a texture.

        宽度和高度均为 2 的整数次幂的纹理图像。在某些图形系统中，用作纹理的图像必须满足这一要求。


    precision qualifier
        In GLSL, one of the following modifiers on a numeric variable declaration: lowp, mediump, or highp. A precision modifier specifies the minimum number of bits or range of values for the variable.

        在 GLSL 中用于数值变量声明的修饰符之一：`lowp`、`mediump` 或 `highp`。精度修饰符指定了该变量的最小位数或取值范围。


    procedural texture
        A texture for which the value at a given set of texture coordinates is computed as a mathematical function of the coordinates, as opposed to an image texture where the value is obtained by sampling an image.

        一种纹理，其在特定纹理坐标处的值是由数学函数计算得出的，而不是通过采样图像获得的，后者称为图像纹理。


    programmable pipeline
        A graphics processing pipeline in which some of the processing stages can or must be implemented by programs. Data for an image passes through a sequence of processing stages, with the image as the end product. The sequence is called a "pipeline." Programmable pipelines are used in modern GPUs to provide more flexibility and control to the programmer. The programs for a programmable pipeline are known as shaders and are written in a shader programming language such as GLSL.

        一种图形处理流水线，其某些处理阶段可以或必须由程序实现。图像数据通过一系列处理阶段传递，最终生成图像，整个序列称为“流水线”。现代 GPU 使用可编程流水线以提供更强的灵活性与可控性。可编程流水线的程序称为着色器（shader），通常使用如 GLSL 之类的着色器语言编写。


    projected
        transformation that maps coordinates in 3D to coordinates in 2D. Projection is used to convert a three-dimensional scene into a two-dimensional image.

        一种将三维坐标映射为二维坐标的变换。投影用于将三维场景转换为二维图像。

    projection
        A transformation that maps coordinates in 3D to coordinates in 2D. Projection is used to convert a three-dimensional scene into a two-dimensional image.

        一种将三维坐标映射为二维坐标的变换。投影用于将三维场景转换为二维图像。


    projection transformation
        In 3D graphics, a transformation that maps a scene in 3D space onto a 2D image. In OpenGL 1.1, the projection maps the view volume (that is, the region in 3D space that is visible in the image) to clip coordinates, in which the values of x, y, and z range from -1 to 1. The x- and y-coordinates are then mapped to the image, while the z coordinate provides depth information.

        在三维图形中，将三维空间中的场景映射为二维图像的变换。在 OpenGL 1.1 中，该投影将视景体（即图像中可见的三维空间区域）映射为剪裁坐标，其中 x、y、z 的取值范围均为 -1 到 1。x 和 y 最终映射到图像，而 z 提供深度信息。


    promise (in JavaScript)
        In JavaScript programming, a promise represents a result that might be available immediately or at some time in the future. A programmer can provide a function to be called if and when the promise is fulfilled (that is when the result becomes available). A programmer can also provide a function to be called when the promise is rejected (for example, if some error occurs). Promises are asynchronous since the function that handles success or failure will be called at some unpredictable time.

        在 JavaScript 编程中，Promise 表示一个可能立即可用，也可能在将来某时才可用的结果。程序员可以提供一个函数，当 Promise 成功兑现（即结果可用）时调用该函数；也可以提供一个函数，在 Promise 被拒绝（例如发生错误）时调用。Promise 是异步的，因为处理成功或失败的函数将在不可预测的时间点执行。


    quad
        A quadrilateral, that is a four-sided figure in the plane. OpenGL 1.1 has the primitives GL_QUADS and GL_QUAD_STRIP for drawing quads, but it assumes without checking that the vertices that are provided are in fact planar and define quadrilaterals that are convex.

        四边形，即一个平面内的四边图形。OpenGL 1.1 提供 GL_QUADS 和 GL_QUAD_STRIP 原语用于绘制四边形，但不检查所提供的顶点是否共面并构成凸四边形。


    quaternion
        A vector in the quaternion algebra, which is a four dimensional vector space in which two vectors, in addition to being added, can be multiplied. In computer graphics, quaternions of length one are often used to represent rotations. An advantage is that in the quaternion representation, it is possible to smoothly interpolate between two rotations.

        四元数代数中的一个向量，它是四维向量空间中的元素，不仅可进行加法，也可相乘。在计算机图形中，单位长度的四元数常用于表示旋转。其优势在于：四元数表示方式可以实现两个旋转之间的平滑插值。


    radial gradient
        A color gradient pattern in which there are concentric circles, or sometimes ellipses, of constant color, with a color variation along the radius of the circles.

        一种颜色渐变图案，其中颜色在若干同心圆（或椭圆）之间保持恒定，并沿半径方向渐变。

    raster graphics
        Pixel-based graphics in which an image is specified by assigning a color to each pixel in a grid of pixels.

        基于像素的图形，通过为像素网格中的每个像素赋予颜色来指定图像。

    rasterization
        The process of creating a raster image, that is one made of pixels, from other data that specifies the content of the image. For example, a vector graphics image must be rasterized in order to be displayed on a computer screen.

        光栅化  

        从指定图像内容的其他数据生成由像素组成的光栅图像的过程。例如，矢量图形图像在显示到计算机屏幕上之前必须经过光栅化处理。


    ray casting
        The process of following a ray (that is, half of an infinite line) starting at a given point and extending in a given direction, in order to find points of intersection of the ray with objects in a scene. Usually, only the intersection point that is closest to the starting point of the ray is of interest.

        光线投射  

        沿某一方向从给定起点出发，跟踪一条射线（即一条有向直线的一部分），以查找射线与场景中对象的交点的过程。通常仅关心距离起点最近的交点。


    ray tracing
        A recursive rendering algorithm that uses ray casting. A ray is cast from the viewpoint through a point in the image and into the scene, to determine what is seen at that point. To determine the color that is seen at that point, further rays are cast from the point, including a reflected ray (if the object has specular reflections), a refracted ray (if the object is translucent) and shadow rays towards light sources (to determine whether the object is illuminated by that light). Finding a color for a reflected or refracted ray can use a recursive application of the ray tracing algorithm.

        光线追踪  
        
        一种递归渲染算法，基于光线投射。在此过程中，从观察点通过图像中的某一点向场景投射光线，以确定该点可见的内容。为确定该点的最终颜色，会从该点继续投射多条光线，包括反射光线（若物体具有镜面反射）、折射光线（若物体为半透明）和朝向光源的阴影光线（用于判断是否被光源照亮）。对反射光线或折射光线的颜色计算可递归调用光线追踪算法。


    real-time graphics
        The type of computer graphics that is needed for computer animation or other applications where the images must be rendered quickly, at the time when they are viewed. For computer animation, real-time graphics generally requires the ability to render the scene sixty times per second.

        实时图形  

        用于计算机动画或其他需要即时渲染图像的应用中的图形类型。对于计算机动画而言，实时图形通常要求场景每秒渲染 60 次。


    reflection mapping
        Another name for environment mapping.

        反射贴图  

        环境贴图的另一种称呼。


    reflectivity
        The proportion or fraction of incident light that is reflected by an object. An object can have different reflectivities at different wavelengths. The color of an object is determined by its reflectivities at all wavelengths.

        反射率  
    
        物体反射入射光的比例。物体在不同波长下的反射率可能不同。一个物体的颜色由其在各波长下的反射率共同决定。


    refraction
        The bending of light as it passes from one transparent or translucent medium into another.

        折射  

        当光线从一种透明或半透明介质进入另一种介质时发生的方向改变。


    regular polygon
        A polygon in which all the sides have the same length and all the angles between consecutive sides are equal. Usually the term is restricted to simple polygons, which have sides that do not intersect except at their endpoints.

        正多边形  

        边长相等且相邻边之间夹角相等的多边形。通常，该术语仅用于不自交的简单多边形。


    regular polyhedron
        A polyhedron in which each face is a regular polygon, and all the faces and angles are identical. There are only five regular polyhedra: the tetrahedron with 4 triangular faces, the cube with 6 square faces, the octahedron with 8 triangular faces, the dodecahedron with 12 pentagonal faces, and the icosahedron, with 20 triangular faces.

        正多面体  

        每个面均为正多边形，且所有面和角都相同的多面体。仅存在五种正多面体：四面体（4 个三角形面）、立方体（6 个正方形面）、八面体（8 个三角形面）、十二面体（12 个五边形面）和二十面体（20 个三角形面）。


    renderbuffer
        In WebGL, a buffer (that is, a region of memory) that can be attached to a framebuffer for use as a color buffer, depth buffer, or stencil buffer.

        渲染缓冲区  

        在 WebGL 中，一种缓冲区（即内存区域），可附加到帧缓冲对象中，用作颜色缓冲区、深度缓冲区或模板缓冲区。


    rendering
    rendered
        The process of producing a 2D image from a 3D scene description.

        渲染  

        根据 3D 场景描述生成 2D 图像的过程。

    render-to-texture
        A technique in which the output of a rendering operation is written directly to a texture. In WebGL, render-to-texture can be implemented by attaching the texture as one of the buffers in a framebuffer.

        渲染至纹理  

        一种技术，其中渲染操作的输出直接写入一个纹理。在 WebGL 中，通过将纹理附加为帧缓冲对象中的一个缓冲区实现该功能。


    RGBA color
        An RGB color—specified by red, green, and blue component values—together with an alpha component. The alpha component is most often take to specify the degree of transparency of the color, with a maximal alpha value giving a fully opaque color.

        RGBA 颜色  

        基于红色、绿色和蓝色分量值的 RGB 颜色，加上一个 alpha 分量。Alpha 分量通常表示颜色的不透明度，最大值表示完全不透明。


    RGB color
    RGB color model
        A color specified by three numbers giving the amount of red, green, and blue in the color.

        RGB 颜色 / RGB 颜色模型  

        由三个数值指定的颜色，分别表示红、绿、蓝成分的强度。


    right-handed coordinate system
        A coordinate system on 3D space in which the x, y, and z-axes satisfy this property: If you point the thumb of your right hand in the direction of the positive z-axis, then your fingers will curl from the positive x-axis towards the positive y-axis.

        右手坐标系  

        三维空间中的坐标系，其中 x、y、z 三个坐标轴满足如下关系：若右手拇指指向正 z 轴方向，则其余四指从正 x 轴方向弯向正 y 轴方向。


    right-hand rule
        A rule that is used to determine the positive direction of rotation about an axis in 3D space: If you point the thumb of your right hand in the direction of the axis, then your fingers will curl in the direction of positive angles of rotation. Note that this assumes that the axis has a direction; in OpenGL, an axis of rotation is determined by the point (0,0,0) and another point (x,y,z), and the direction of the axis is from (0,0,0) towards (x,y,z).

        右手法则  

        一种用于确定三维空间中绕轴正向旋转方向的规则：若右手拇指指向轴的方向，则四指弯曲的方向即为正向旋转角度的方向。注意，这依赖于轴的方向；在 OpenGL 中，旋转轴由原点 (0,0,0) 和另一个点 (x,y,z) 定义，方向为从原点指向该点。


    rotation
        A geometric transform that rotates each point by a specified angle about some point (in 2D) or axis (in 3D).

        旋转  
    
        一种几何变换，使得每个点围绕某个点（在 2D 中）或某条轴线（在 3D 中）按指定角度旋转。

    sampler variable
        In GLSL, a variable in a shader program that can be used to do lookup in an image texture. The value of a sampler variable specifies the texture unit that will be used to do the lookup. In WebGL, sampler variables are of type "sampler2D" or "samplerCube."

        采样器变量  

        在 GLSL 中，用于在着色器中从图像纹理中查找值的变量。采样器变量的值指定将用于纹理查找的纹理单元。在 WebGL 中，采样器变量的类型通常为 "sampler2D" 或 "samplerCube"。


    sampling
        The operation of mapping texture coordinates to colors from a texture, including using mipmaps if available and applying a minification or magnification filter if necessary.

        采样  

        将纹理坐标映射到纹理中对应颜色的过程，可能涉及 mipmap（多级渐远纹理）以及必要时应用缩小或放大滤波器。


    scalar product
        The product of a number and a vector. The scalar product of a number s and vector v is the vector obtained by multiplying each coordinate of v by s. In 3D, if s is a number and v=(x,y,z), then the scalar product of s times v is the vector (sx,sy,sz).

        数量积（标量乘积）  

        数与向量的乘积。数 s 与向量 v 的数量积是一个新向量，其每个坐标等于 v 的对应坐标乘以 s。在三维空间中，若 s 是一个数且 v = (x, y, z)，则 s * v = (sx, sy, sz)。


    scaling
        A geometric transform that multiplies each coordinate of a point by a number called the scaling factor. Scaling increases or decreases the size of an object, but also moves its points closer to or farther from the origin. Scaling can be uniform—the same in every direction—or non-uniform—with a different scaling factor in each coordinate direction. A negative scaling factor can be used to apply a reflection.

        缩放  

        一种几何变换，通过将点的每个坐标乘以一个称为缩放因子的数来实现。缩放可以改变物体的大小，同时也会使其各点靠近或远离原点。缩放可以是均匀的（各方向因子相同），也可以是非均匀的（各方向因子不同）。负的缩放因子可用于实现反射操作。


    scene description language
        A language that can be used to specify graphics images by stating what's in the image. That is, the scene is created "declaratively," by stating what it contains, as opposed to being created "procedurally," by a program. A document written in a scene description language can be used to generate a scene graph for the scene.

        场景描述语言  

        一种用于通过声明图像内容来指定图形图像的语言。即，场景是“声明式”地定义的，而不是通过程序“过程式”地构建的。用场景描述语言编写的文档可用于生成场景图。


    scene graph
        A data structure that represents the objects in a scene, together with attributes of the objects and the modeling transformations that are applied to the objects. An image of the scene is created by traversing the scene graph data structure. A scene graph might exist only conceptually, or it might be an actual data structure in a program.

        场景图  
    
        一种表示场景中对象的结构化数据，同时包含对象的属性及其应用的建模变换。通过遍历场景图结构生成图像。场景图可以只是概念上的，也可以是程序中实际的数据结构。

    shader
    shaders
        A program to be executed at some stage of the rendering pipeline. OpenGL shaders are written in the GLSL programming languages. For WebGL, only vertex shaders and fragment shaders are supported. WebGPU also has compute shaders, which are used in compute pipelines.

        渲染管线某个阶段要执行的程序。OpenGL 的着色器使用 GLSL 编程语言编写。对于 WebGL，仅支持顶点着色器和片段着色器。WebGPU 还支持计算着色器（compute shaders），用于计算管线中。

    shadow mapping
        A technique for determining which parts of a scene are illuminated and which are in shadow from a given light source. The technique involves rendering the scene from the point of the view of the light source, but uses only the depth buffer from that rendering. The depth buffer is the "shadow map." Along a given direction from the light source, the object that is illuminated by the light is the one that is closest to the light. The distance to that object is essentially encoded in the depth buffer. Objects at greater distance are in shadow.

        一种判断场景中哪些部分被光源照亮、哪些部分处于阴影中的技术。该技术会从光源的视角渲染整个场景，但只使用渲染产生的深度缓冲区作为“阴影贴图（shadow map）”。沿着从光源出发的某个方向，最靠近光源的对象将被其照亮，其距离被编码在深度缓冲中，距离更远的对象则被视为处于阴影中。


    shadow ray
        In the ray tracing algorithm, a ray that is cast from a point on object in the direction of a light source to determine whether that point is illuminated by that light source or is in shadow.

        在光线追踪算法中，从物体表面某点朝光源方向投射的一条光线，用于判断该点是否被该光源照亮，还是处于阴影中。


    shear transform
        A shear transformation in 2D leaves some line, L, fixed, and lines perpendicular to L are "tilted" relative to L by the same angle. Another description is that a line parallel to L is mapped to itself, but is moved by an amount proportional to its distance from L. In 3D, a shear transformation leaves some plane, P, fixed, and it maps a plane parallel to P to itself, but moved by an amount proportional to its distance from P.

        2D 中的剪切变换保持某条直线 L 不动，并使垂直于 L 的直线相对于 L 倾斜相同的角度。另一种描述是，与 L 平行的直线被映射到自身，但根据其与 L 的距离，整体会被平移相应的距离。3D 中的剪切变换保持某个平面 P 不动，并使与 P 平行的平面整体平移一个与其距 P 的距离成比例的量。


    shininess
        A material property that determines the size and sharpness of specular highlights. Also called the "specular exponent" because of the way it is used in lighting calculations. In OpenGL, shininess is a number in the range 0 to 128.

        控制镜面高光大小与锐度的材质属性。在光照计算中也称为“镜面指数（specular exponent）”。在 OpenGL 中，shininess 是 0 到 128 之间的数值。


    single buffering
        As opposed to double buffering, a graphics technique in which the image is drawn directly to the screen (that is, to the buffer that serves as the source for the screen image). The disadvantage of single buffering is that, for a complex image, the user can observe the process of drawing the image.

        与双缓冲相对的一种图形渲染技术，即图像直接绘制到屏幕缓冲区（该缓冲区也是屏幕图像的来源）。其缺点是对于复杂图像，用户可能会看到绘制过程。


    skybox
        A large cube that surrounds a scene and is textured with images that form a background for that scene, in all directions.

        包围整个场景的大立方体，其各面贴有图像，用于构建该场景在各个方向上的背景。


    smooth shading
        A lighting computation for the faces of a polygon or polygonal mesh that uses a different normal vector at each vertex of the polygon. When two polygons share a vertex, both polygons use the same normal vector for that vertex, resulting in a smooth appearance at that vertex. Smooth shading is appropriate when a polygonal mesh is used as an approximation for a smooth surface.

        一种用于多边形或多边形网格的光照计算方式，每个顶点使用不同的法向量。当两个多边形共享一个顶点时，它们使用该顶点相同的法向量，从而在该顶点处呈现平滑过渡。此技术适用于将多边形网格用作平滑曲面的近似。


    specular color
        A material property that represents the proportion of incident light that is reflected specularly by a surface.

        一种材质属性，表示表面对入射光的镜面反射比例。

    specular exponent
        A material property that determines the size and sharpness of specular highlights. Called "shininess" in OpenGL.

        控制镜面高光大小与锐度的材质属性。在 OpenGL 中称为 shininess。

    specular highlight
        Illumination of a surface produced by specular reflection. A specular highlight is seen at points on the surface where the angle from the surface to the viewer is approximately equal to the angle from the surface to a light source.

        由于镜面反射而在表面上产生的高光区域。高光出现在观察方向与光源方向相对于表面法线近似对称的位置。

    specular reflection
        Mirror-like reflection of light rays from a surface. A ray of light is reflected as a ray in the direction that makes the angle of reflection equal to the angle of incidence. A specular reflection can only be seen by a viewer whose position lies on the path of the reflected ray.

        表面对光线的镜面反射。入射光线会以等角度被反射出去。只有观察者处在反射光线方向上时才能看到该反射。


    spotlight
        A light that emits a cone of illumination. A spotlight is similar to a point light in that it has a position in 3D space, and light radiates from that position. However, the light only affects objects that are in the spotlight's cone of illumination.

        一种发出锥形光束的光源。聚光灯类似于点光源，有其在三维空间中的位置，但只影响锥形光束覆盖到的对象。


    stack
        A data structure with the operations push() and pop(). Pushing an item onto a stack just adds that item to the stack. Popping from the stack will remove and return the item that was most recently pushed onto the stack.

        一种支持 push() 与 pop() 操作的数据结构。push 表示将元素压入栈顶，pop 表示移除并返回栈中最后压入的元素（后进先出）。


    storage buffer
        In WebGPU, a general purpose buffer on the GPU, which can be used in compute shaders as well as in vertex and fragment shaders.

        WebGPU 中的一种通用 GPU 缓冲区，可用于计算着色器，也可用于顶点和片段着色器中。

    storage qualifier
        In GLSL, one of the following modifiers on a variable declaration: uniform, attribute, varying, or const.

        在 GLSL 中，用于变量声明的修饰符之一，包括：uniform、attribute、varying 或 const。


    stroking a shape
        Drawing the outline of a shape, as if a pen is dragged along the boundary of the shape. For a shape with no interior, such as a line segment, stroking the shape simply means dragging the pen along the shape.

        描边绘制图形轮廓的过程，类似于将笔沿图形边界拖动。对于如线段等无内部区域的图形，描边即为在其路径上绘制。


    subsurface scattering
        A lighting effect in which light enters a slightly translucent object, is reflected internally one or more times, and then exits the object at a different point. Subsurface scattering contributes to the appearance of materials such as jade, milk, and skin.

        一种光照效果：光线进入略微半透明的物体，在其内部反射一到多次后从不同点射出。此现象决定了如玉石、牛奶与皮肤等材质的视觉表现。


    SVG
        Scalable Vector Graphics. An XML language for specifying 2D vector graphics. SVG is a scene description language. It is designed to integrate into web pages.

        可缩放矢量图（Scalable Vector Graphics）。一种用于定义二维矢量图形的 XML 语言。SVG 是一种场景描述语言，设计用于嵌入网页中。


    swizzler
        In GLSL and WGSL, a notation such as v.yzx, where v is a vector and v.yzx represents the three-component vector made up of the y, z, and x components of v. Technically, any use of the dot notation with vectors is considered to be a swizzler.

        在 GLSL 与 WGSL 中的向量访问语法，如 v.yzx，其中 v 是一个向量，v.yzx 表示由其 y、z、x 分量组成的三分量向量。技术上，任何对向量使用点操作符的表达式都称为 swizzler。


    texel
        A pixel in a texture image.

        纹理图像中的一个像素。

    texture
        Variation in some property from point-to-point on an object. The most common type is image texture. When an image texture is applied to a surface, the surface color varies from point to point.

        表面上某个属性随空间位置变化的映射。最常见的是图像纹理，将图像贴附于表面后，使其颜色在不同位置有所变化。


    texture coordinates
        Refers to the 2D coordinate system on a texture image, or to similar coordinate systems for 1D and 3D textures. Texture coordinates typically range from 0 to 1 both vertically and horizontally, with (0,0) at the lower left corner of the image. The term also refers to coordinates that are given for a surface and that are used to specify how a texture image should be mapped to the surface.

        指纹理图像中的二维坐标系（对于 1D 或 3D 纹理也有类似坐标系）。纹理坐标通常在水平和垂直方向上取值范围为 0 到 1，(0,0) 位于图像左下角。该术语也指为表面指定的一组坐标，用于定义图像纹理如何映射到该表面上。

    texture objects
    texture object
        A data structure that can potentially be stored on the graphics card, and which can hold a texture image, a set of mipmaps, and configuration data such as the current setting for the minification and magnification filters. Using texture objects makes it possible to switch rapidly between textures without having to reload the data into the graphics card.

        一种可存储在图形卡上的数据结构，用于保存纹理图像、一组多级渐远纹理（mipmap）以及诸如缩小与放大过滤器设置等配置数据。使用纹理对象可以在多个纹理之间快速切换，而无需每次都将数据重新加载到图形卡中。


    texture repeat mode
        Determines how texture coordinates outside the range 0.0 to 1.0 are treated when sampling an image texture. The texture image itself has vertical and horizontal coordinates in the range 0.0 to 1.0. For coordinates outside that range, the texture repeat mode CLAMP or CLAMP_TO_EDGE, for example, clamps the coordinates to the range 0.0 to 1.0, essentially extending the color at the edge of the image indefinitely in all directions. Other repeat modes include REPEAT and MIRRORED_REPEAT.

        决定在采样图像纹理时，对于超出 0.0 到 1.0 范围的纹理坐标应如何处理。纹理图像本身的垂直和水平坐标范围为 0.0 到 1.0。对于超出此范围的坐标，诸如 CLAMP 或 CLAMP_TO_EDGE 的重复模式会将坐标限制（clamp）在 0.0 到 1.0 范围内，实质上将图像边缘处的颜色无限延展。其他重复模式包括 REPEAT 与 MIRRORED_REPEAT。


    texture target
        In OpenGL, one of several kinds of texture, such as 2D image texture, 1D texture, and cube map texture. A texture target is specified by a constant such as GL_TEXTURE_2D or GL_TEXTURE_CUBE_MAP_POSITIVE_X. The texture target is a parameter to many OpenGL functions that work with textures.

        在 OpenGL 中，表示某类纹理类型，例如 2D 图像纹理、1D 纹理或立方体贴图纹理。纹理目标由常量指定，如 GL_TEXTURE_2D 或 GL_TEXTURE_CUBE_MAP_POSITIVE_X。纹理目标是许多处理纹理的 OpenGL 函数的参数。


    texture transformation
        A transformation that is applied to texture coordinates before they are used to sample data from a texture. The effect is to translate, rotate, or scale the texture on the surface to which it is applied.

        一种在使用纹理坐标进行采样前应用于其上的变换。效果是在贴图到表面之前对纹理进行平移、旋转或缩放操作。


    texture unit
        A hardware component in a GPU that does texture lookup. (Can also refer to an abstraction for such a component, whether or not it is actually implemented in hardware.) That is, it maps texture coordinates to colors from an image texture. This is the operation called "sampling," and texture units are associated with sampler variables in GLSL shader programs.

        GPU 中用于执行纹理查找的硬件组件（也可指代该组件的软件抽象，不论是否有硬件实现）。也就是说，它将纹理坐标映射为图像纹理中的颜色值。此操作称为“采样”（sampling），纹理单元通常与 GLSL 着色器程序中的采样器变量（sampler）关联。


    three.js
        A JavaScript library for 3D graphics. The library implements an object-oriented scene graph API. While it is used primarily with WebGL, three.js can also render 3D scenes using the 2D canvas graphics API.

        一个用于 3D 图形的 JavaScript 库。该库实现了基于对象的场景图 API。尽管主要与 WebGL 配合使用，three.js 也支持使用 2D canvas 图形 API 渲染 3D 场景。


    TMU
        Texture Mapping Unit, another name for texture unit (perhaps with a stronger implication of actual hardware support). Also called a TPU (Texture Processing Unit).

        纹理映射单元（Texture Mapping Unit），是纹理单元的另一个名称（可能更强调硬件实现的含义）。有时也称为 TPU（Texture Processing Unit）。


    torus
        A 3D geometric object having the shape of a doughnut (or bagel).

        一种三维几何体，具有甜甜圈（或百吉饼）形状。


    translation
        A geometric transform that adds a given translation amount to each coordinate of a point. Translation is used to move objects without changing their size or orientation.

        一种几何变换，它对点的每个坐标加上一个给定的平移量。平移变换用于在不改变对象尺寸与方向的情况下移动对象。


    two-sided lighting
        An option in OpenGL that allows the back face of a polygon to have different material properties from the front face. Also, when this option is on, the normal vector that is used in lighting calculations for the back face is taken to be the negative of the vector for the front face. (The negative of a vector points in the opposite direction.)

        OpenGL 中的一种选项，允许多边形的背面具有与正面不同的材质属性。当此选项启用时，背面在光照计算中使用的法向量为正面的法向量的相反方向（即负向）。


    typed array
        In JavaScript, an array type that is limited to holding numerical values of a single type. For example, the type Float32Array represents arrays that can hold 32-bit floating point values, and Uint8Array arrays can hold only 8-bit integer values. Such arrays are more efficient than general JavaScript arrays for numerical calculations. The were introduced into JavaScript along with HTML canvas graphics and WebGL.

        JavaScript 中的一类数组类型，仅能包含单一类型的数值。例如，Float32Array 表示可容纳 32 位浮点数的数组，Uint8Array 表示只能容纳 8 位整数的数组。与通用 JavaScript 数组相比，这类数组在数值计算中更高效。typed arrays 是伴随 HTML canvas 图形与 WebGL 一同引入 JavaScript 的。


    uniform scaling
        A scaling transformation in which the scaling factors in all directions are the same. Uniform scaling changes the size of an object without distorting its shape.

        一种缩放变换，其在所有方向上的缩放因子相同。统一缩放在不改变对象形状的前提下改变其尺寸。


    uniform variable
        Variables that represent input to a shader program in a programmable graphics pipeline. A uniform variable has the same value at every vertex and at every pixel of a primitive.

        在可编程图形流水线中，表示传入着色器程序的变量。uniform 变量在图元的每个顶点和像素处取值相同。


    unit normal
        A normal vector of length one; that is, a unit vector that is perpendicular to a curve or surface at a given point on the curve or surface.

        长度为 1 的法向量；也就是说，一个在曲线或曲面某点上与该点垂直的单位向量。


    unit vector
        A vector of length one.

        长度为 1 的向量。

    unsigned byte
        A data type representing 8-bit non-negative integer values, taking values in the range from 0 to 255.

        表示 8 位非负整数值的数据类型，取值范围为 0 到 255。

    URL
        Uniform Resource Locator. An address of some resource on the World Wide Web. For example, " http://math.hws.edu/grahicsbook ".

        Uniform Resource Locator，统一资源定位符。用于表示互联网上资源的地址。例如：“ http://math.hws.edu/graphicsbook ”。


    VAO
        Vertex Array Object. In WebGL 2.0, a region of memory, typically on the graphics card, that holds a collection of attribute settings such as enabled state and values of vertex attribute pointers. All of the settings can then be selected simply by binding the VAO.

        顶点数组对象（Vertex Array Object）。在 WebGL 2.0 中，一段内存区域（通常位于图形卡上），保存一组属性设置，如顶点属性指针的启用状态与取值。通过绑定 VAO，可一次性应用全部设置。


    varying variable
        A variable that is used to communicate values from the vertex shader to the fragment shader in the WebGL or OpenGL ES 2.0 graphics pipeline. A varying variable is assigned a value in the vertex shader. The value of the variable in the fragment shader for a pixel in the primitive is obtained by interpolating the values from the vertices of the primitive. (In newer versions of GLSL, which support additional shader stages, the term "varying variable" is replaced by the more general terms "in variable" and "out variable," which refer to variables that are used for input to or output from a shader.)

        在 WebGL 或 OpenGL ES 2.0 图形流水线中，用于从顶点着色器向片段着色器传递值的变量。在顶点着色器中为 varying 变量赋值，图元中某像素的片段着色器将通过插值顶点值来获得该变量的值。在新版支持更多着色器阶段的 GLSL 中，"varying" 已被更通用的 "in" 与 "out" 变量所替代，分别表示着色器的输入与输出变量。


    VBO
    Vertex Buffer Objects
        Vertex Buffer Object. A block of memory that can hold the coordinates or other attributes for a set of vertices. A VBO can be stored on a GPU. VBOs make it possible to send such data to the GPU once and then reuse it several times. In OpenGL, VBOs are used with the functions glDrawArrays and glDrawElements.

        顶点缓冲对象（Vertex Buffer Object），用于存储一组顶点的坐标或其他属性的数据块，可存放于 GPU 上。使用 VBO 可以一次性将数据发送到 GPU，并多次重复使用。在 OpenGL 中，VBO 通常与 glDrawArrays 和 glDrawElements 函数配合使用。


    vector
        An element of a vector space. Elements of a vector space can be added and can be multiplied by constants. For computer graphics, a vector is just a list or array containing two, three, or four numbers. Vectors in that sense are often used to represent points in 2D, 3D, or 4D space. Properly, however, a vector represents a quantity that has a length and a direction; a vector used in this way can be visualized as an arrow.

        向量空间中的一个元素。向量可以相加、也可与常数相乘。在计算机图形中，向量通常是包含 2、3 或 4 个数字的列表或数组，常用于表示二维、三维或四维空间中的点。不过从数学意义来看，向量表示具有长度和方向的量；在这种用法下，向量可视为一支箭头。


    vector graphics
        Shape-based graphics in which an image is specified as a list of the shapes or objects that appear in the image.
        
        基于形状的图形，其图像由所包含的形状或对象的列表来描述。


    vertices
    vertex
        One of the points that define a geometric primitive, such as the two endpoints of a line segment or the three vertices of a triangle. (The plural is "vertices.") A vertex can be specified in a coordinate system by giving its x and y coordinates in 2D graphics, or its x, y, and z coordinates in 3D graphics.

        构成几何图元的点之一，例如线段的两个端点，或三角形的三个顶点。（复数形式为 "vertices"。）一个顶点可通过坐标系中的位置来表示，在 2D 图形中为 x 与 y 坐标，在 3D 图形中则为 x、y 与 z 坐标。

    vertex array
        In OpenGL, an array that is used to store coordinates or other attribute values for vertices, to be used with the functions glDrawArrays and glDrawElements. A vertex array exists on the "client side" of OpenGL, and it must be transmitted to the GPU to be used. In Java's JOGL API for OpenGL, nio buffers are used instead of arrays.

        在 OpenGL 中，顶点数组用于存储顶点的坐标或其他属性值，供函数 ``glDrawArrays`` 和 ``glDrawElements`` 使用。顶点数组存在于 OpenGL 的“客户端”侧，必须传输到 GPU 才能使用。在 Java 的 JOGL API 中，使用 ``nio`` 缓冲区代替数组。


    vertex buffer
        In WebGPU, a vertex buffer is a GPU data structure that holds values to be used as input the vertex shader.

        在 WebGPU 中，顶点缓冲区是一种 GPU 数据结构，用于存储将作为顶点着色器输入的值。

    vertex shader
    vertex shaders
        A shader program that will be executed once for each vertex in a primitive. A vertex shader must compute the vertex coordinates in the clip coordinate system. It can also compute other properties, such as color.

        顶点着色器是一种着色程序，它会针对图元中的每个顶点执行一次。顶点着色器必须计算该顶点在裁剪坐标系中的坐标；它还可以计算颜色等其他属性。


    viewing
        Setting the position and orientation of the viewer in a 3D world, which determine what will be visible when the 2D image of a 3D world is rendered.

        在三维世界中设置观察者的位置与方向，用以确定当三维世界被渲染为二维图像时哪些内容可见。


    viewing transformation
        The transformation in 3D graphics that maps world coordinates to eye coordinates. The viewing transform establishes the position, orientation, and scale of the viewer in the world.

        三维图形中的一种变换，用于将世界坐标映射到视点（眼睛）坐标。视图变换定义了观察者在世界中的位置、方向和比例。


    viewport
        The rectangular area in which the image for 2D or 3D graphics is displayed. The coordinates on the viewport are pixel coordinates, more properly called device coordinates since they are actual physical coordinates on the device where the image is being displayed.

        显示二维或三维图像的矩形区域。视口中的坐标是像素坐标，更准确地称为“设备坐标”，因为它们代表图像所显示设备上的物理坐标。


    viewport transformation
        In OpenGL 1.1, the final transformation from clip coordinates to device coordinates. The viewport transformation maps the clipping cube (the cube in 3D given by x, y, and z coordinates in the range from -1 to 1) to the viewport (the rectangle in the drawing surface where the image is rendered).

        在 OpenGL 1.1 中，这是从裁剪坐标到设备坐标的最终变换。视口变换将裁剪立方体（一个以 x、y、z 范围为 -1 到 1 定义的三维立方体）映射到视口（图像渲染所在的绘图表面矩形区域）。


    view volume
        In OpenGL 1.1, the region is 3D space that is visible in the rendered image. For orthographic projections, the view volume is a rectangular solid. For perspective projection, the view volume is a frustum (truncated pyramid).

        在 OpenGL 1.1 中，指渲染图像中可见的三维空间区域。对于正交投影，视景体是一个矩形立方体；对于透视投影，视景体是一个截头四棱锥体。


    view window
        As used in this book, the window, or view window, for 2D graphics is the rectangle in the xy-plane that contains the portion of the plane that will be displayed in the image. (The corresponding term in 3D graphics is "view volume.")

        本书中提到的“窗口”或“视图窗口”是指二维图形中 xy 平面上的一个矩形，它包含了将被显示在图像中的平面部分。（在三维图形中，对应的术语是“视景体”。）


    Vulkan
        An open-source cross-platform API for 3D graphics and computation, designed as a more modern and efficient replacement for OpenGL.

        一种开源的跨平台 3D 图形与计算 API，被设计为 OpenGL 的现代高效替代方案。


    WebGL
        A 3D graphics API for use on web pages. WebGL programs are written in the JavaScript programming language and display their images in HTML canvas elements. WebGL is based on OpenGL ES, the version of OpenGL for embedded systems, with a few changes to adapt it to the JavaScript language and the Web environment.

        用于网页中的 3D 图形 API。WebGL 程序使用 JavaScript 编写，图像显示在 HTML 的 ``<canvas>`` 元素中。WebGL 基于 OpenGL ES（用于嵌入式系统的 OpenGL 版本），做出了一些针对 JavaScript 与 Web 环境的修改。


    WebGL extension
        An optional capability in WebGL that is not available in all implementations. The WebGL API has a function for checking whether a given extension is available and, if so, activating it.

        WebGL 中的一种可选功能，并非所有实现都支持。WebGL API 提供函数用于检查给定扩展是否可用，并在可用时启用该扩展。


    WebGPU
        A new JavaScript graphics API, similar to WebGL, but designed to let web programs access modern GPU capabilities such as compute shaders.

        一种新的 JavaScript 图形 API，与 WebGL 类似，但设计上可访问现代 GPU 功能，例如计算着色器。


    WGSL
        The WebGPU Shader Language, the programming language in which shaders for use in WebGPU are written.

        WebGPU 着色语言（WebGPU Shader Language），用于编写 WebGPU 着色器的编程语言。

    winding number
        The winding number of a path about a point that does not lie on the path is the number of times that the path winds around the point, counting each 360-degree rotation in the positive direction about the point as one and each 360-degree turn in the negative direction as minus one. To compute the winding number, draw a ray extending from the point to infinity. Each crossing of the ray by the path counts as 1 if it crosses the ray going in the positive direction and as negative 1 if it crosses in the negative direction.

        环绕数是指路径绕过一个不在路径上的点的次数。每次正向（逆时针）绕该点旋转 360 度记为 +1，反向（顺时针）绕 360 度记为 -1。计算环绕数的方法之一是从该点画一条无限延伸的射线，每当路径穿过该射线时，若为正向穿越则记为 +1，负向穿越则记为 -1，最后求和。


    wireframe
        A style of drawing a polyhedron or polygonal mesh in which only the edges are drawn, resulting in an image made up of line segments.

        一种绘制多面体或多边形网格的样式，仅绘制其边，从而生成由线段组成的图像。

    world coordinates
        The coordinate system in which a scene is defined. The image that is produced of the scene will show the contents of the world coordinate system that lie within some view volume (for 3D) or view window (for 2D). Objects are defined in their own object coordinate system. Modeling transformations are then applied to place objects into the scene; that is, they transform object coordinates to world coordinates.

        场景所定义的坐标系。最终生成的图像显示的是该世界坐标系中位于视景体（3D）或视图窗口（2D）内的部分。对象初始定义在各自的对象坐标系中，建模变换（modeling transformation）将对象坐标转换为世界坐标。

    XML
        eXtensible Markup Language. Not a single language as such, but a class of languages that follow certain syntax rules. For example, SVG is an XML language because it follows those rules, but it also has further restrictions on its syntax that make it appropriate for specifying 2D graphics. XML documents, like HTML documents, have a tree-like structure defined by "elements." However, HTML is not an XML language since it does not follow all the syntax rules. XHTML is an alternative language for web pages that is similar to HTML but follows XML syntax rules.

        可扩展标记语言（eXtensible Markup Language），并非某种特定语言，而是一类遵循特定语法规则的语言。例如，SVG 是一种 XML 语言，因为它遵循 XML 规则，并基于此添加了用于描述二维图形的进一步语法限制。XML 文档像 HTML 文档一样具有由“元素”构成的树状结构。不过 HTML 并不是 XML 语言，因为它不完全遵守 XML 的语法规则；XHTML 是一种遵循 XML 语法的网页标记语言，是 HTML 的替代方案。