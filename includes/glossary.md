*[abstract class]:  In object-oriented programming, a class that is meant to be used only as a basis for subclasses. Objects can be created from the subclasses, but not from the abstract class itself. The purpose of an abstract class is to define the properties and behaviors that all of its subclasses have in common.

*[address space (in WGSL)]:  WGSL memory is divided into address spaces. From the WGSL specification: "Each address space has unique properties determining mutability, visibility, the values it may contain, and how to use variables with it."

*[affine transform]:  A transform that preserves parallel lines. That is, when the transform is applied to a pair of lines that are parallel, then the resulting transformed lines are also parallel. An affine transform, T, has the property that the transform of the line segment between a point (x1,y1) and a point (x2,y2) is the line between the points T(x1,y1) and T(x2,y2). Effectively, the transform of a line segment can be computed just by transforming its two endpoints. This makes affine transforms very efficient for computer graphics. Any affine transform can be represented as a composition of rotations, translations, and scalings.

*[alignment (in WGSL)]:  Restrictions on the legal location of a value in memory, depending on the data type. For example, the address of a vec3f variable in WGSL must be a multiple of 16.

*[alpha]: An extra component (that is, one of the numbers that are used to specify a color) in a color model that is not part of the actual color specification. The alpha component is extra information. It is most often used to specify the degree of transparency of a color.

*[alpha blending]:  Using the alpha component of a color to blend the color with a background color, when the color is drawn over the background color. That is, the new color of a pixel is obtained by blending the drawing color with the current color, with the degree of blending depending on the alpha component of the drawing color. Alpha blending is most commonly used to simulate transparency.

*[alpha color component]:  An extra component (that is, one of the numbers that are used to specify a color) in a color model that is not part of the actual color specification. The alpha component is extra information. It is most often used to specify the degree of transparency of a color.

*[ambient color]:  A material property that represents the proportion of ambient light in the environment that is reflected by a surface.

*[ambient light]:  Directionless light that exists in an environment but does not seem to come from a particular source in the environment. An approximation for light that has been reflected so many times that its original source can't be identified. Ambient light illuminates all objects in a scene equally.

*[ambient occlusion]:  A rendering technique that takes into account the fact that ambient light will illuminate different surfaces to varying extents, depending on the degree to which ambient light is blocked, or "occluded," from reaching each surface by other geometry in the scene. Ambient occlusion is an improvement on basic ambient lighting, but, like ambient light itself, it is not an actual physical phenomenon.

*[anaglyph stereo]:  A technique for combining stereographic images of a scene, one for the left eye and one for the right eye, into a single image. Typically, the image for the left eye is drawn using only shades of red, and the image for the right eye contains only blue and green color components. The 3D effect can be seen by viewing the combined image through red/cyan glasses, which allow each eye to see only the image that is intended for that eye.

*[animation]:  A sequence of images that, when displayed quickly one after the other, will produce the impression of continuous motion or change. The term animation also refers to the process of creating such image sequences.

*[anisotropic filtering]:  A technique for more accurate sampling of texture images, in the case where a pixel on the surface that is being textured corresponds to a non-rectangular region in the texture. Anisotropic filtering is available as an optional extension in WebGL.

*[antialiasing]:  A technique used to reduce the jagged or "staircase" appearance of diagonal lines, text, and other shapes that are drawn using pixels. When a pixel is only partly covered by a geometric shape, then the color of the pixel is a blend of the color of the shape and the color of the background, with the degree of blending depending on the fraction of the pixel that is covered by the geometric shape.

*[Antialiasing]:  A technique used to reduce the jagged or "staircase" appearance of diagonal lines, text, and other shapes that are drawn using pixels. When a pixel is only partly covered by a geometric shape, then the color of the pixel is a blend of the color of the shape and the color of the background, with the degree of blending depending on the fraction of the pixel that is covered by the geometric shape.

*[API]:  Application Programming Interface. A collection of related classes, functions, constants, etc., for performing some task. An API is an "interface" in the sense that it can be used without understanding how its functionality is actually implemented.

*[aspect ratio]:  The ratio of the width, w, of a rectangle to the height, h, of the rectangle, expressed either as a ratio **w:h** or as a fraction** w/h**.

*[async function]:  In JavaScript, an async function is one that can use an "await" statement to wait for the result of a promise. When an await statement is executed, the execution of the async function is suspended until the promise has either been fulfilled or rejected, giving other JavaScript code a chance to run in the meantime.

*[attenuation]:  Refers to the way that illumination from a point light or spot light decreases with distance from the light. Physically, illumination should decrease with the square of the distance, but computer graphics often uses a linear attenuation with distance, or no attenuation at at all.

*[attribute]:  A property, such as color, of a graphical object. An image can be specified by the geometric shapes that it contains, together with their attributes.

*[attributes]:  A property, such as color, of a graphical object. An image can be specified by the geometric shapes that it contains, together with their attributes.

*[attribute variable]:  Variables that represent input to the vertex shader in a programmable graphics pipeline. An attribute variable can take on a different value for each vertex in a primitive.

*[axis of rotation]:  Rotation in 3D space is rotation about a line, which is called the axis of rotation. The axis of rotation remains fixed, while everything else moves in circles around the axis.

*[back face]:  One of the two sides of a polygon in 3D. A polygon has two sides. One is taken to be the front face, and the other is the back face. In OpenGL, the difference is determined by the order in which the vertices of the polygon are enumerated. The default is that, seen from the back, the vertices are enumerated in clockwise order around the polygon.

*[barycentric coordinates]:  A coordinate system on a triangle in which a point is written as a linear combination of the vertices of the triangle, that is, `a*A+b*B+c*C`, where A, B, and C are the vertices and a, b, and c are numbers. Any point in the triangle can be written in this form where the coefficients a, b, and c have values in the range 0 to 1 and a+b+c is equal to 1.

*[Bezier curve]:  A smooth curve between two points defined by parametric polynomial equations. A cubic Bezier curve segment is defined by its two endpoints P1 and P2 and by two control points C1 and C2. The tangent to the curve (its direction and speed) at P1 is given by the line from P1 to C1. The tangent vector to the curve at P2 is given by the line from C2 to P2. A quadratic Bezier curve is defined by its two endpoints and a single control point C. The tangent at each endpoint is the line between that endpoint and C.

*[bind group (in WebGPU)]:  A data structure that can hold resources such as buffers, textures, and samples, for input into a pipeline.

*[Blender]:  A free and open source 3D modeling and animation program.

*[Bresenham's line algorithm]:  A specific algorithm for deciding which pixels to color to represent a geometric line segment, using only integer arithmetic. The algorithm can be implemented very efficiently in computer hardware

*[BSDF]:  Bidirectional Scattering Distribution Function. A generalization of the idea of "material" in 3D graphics. A BSDF gives the probability that a light ray that arrives at point of space from one direction will leave that point heading in a another direction. The probability is a function of the two directions, the point, and the wavelength of the light. One kind of scattering is reflection of light from a surface. For that case, the term BRDF (Bidirectional Reflectance Distribution Function) is used.

*[bumpmapping]:  Using a texture to modify the normal vectors on a surface, to give the appearance of variations in height without actually modifying the geometry of the surface.

*[camera]:  In 3D computer graphics, an object that combines the projection and viewing transforms into an abstraction that imitates a physical camera or eye.

*[clip coordinates]:  The default coordinate system in OpenGL. The projection transform maps the 3D scene to clip coordinates. The rendered image will show the contents of the cube in the clip coordinate system that contains x, y, and z values in the range from -1 to 1; anything outside that range is "clipped" away.

*[color buffer]:  In OpenGL, the region of memory that holds the color data for the image. It acts as the drawing surface where images are rendered.

*[color component]:  One of the numbers used in a color model to specify a color. For example, in the RGB color model, a color is specified by three color components representing the amounts of red, green, and blue in the color.

*[color gamut]:  The color gamut of a display device, such as a printer or computer screen, is the set of colors can be displayed by the device.

*[color mask]:  In WebGL, a setting that determines which "channels" in the color buffer are written during rendering. The channels are the RGBA color components red, green, blue, and alpha. A color mask consists of four boolean values, one for each channel. A false value prevents any change from being made to the corresponding color component in the color buffer.

*[color model]:  A way of specifying colors numerically. Each color that can represented in a color model is assigned one or more numerical component values. An example is the RGB color model, where a color is specified by three numbers giving the red, green, and blue components of the color.

*[column-major order]:  Column-by-column ordering of the elements of a two-dimensional matrix; that is, an ordering that starts with the elements in the first column, followed by the elements in the second column, and so on. Column-major order is used for matrices in OpenGL and GLSL.

*[compute shader]:  A stage in a GPU pipeline that does purely computational work, rather than participating directly in graphical rendering.

*[constructor]:  In object-oriented programming, a subroutine that is used to create objects. A constructor for a class creates and initializes objects belonging to that class.

*[control point]:  A point that does not lie on the curve but that is used to help control the shape of the curve. For example, a control point for a Bezier curve segment is used to specify the tangent vector (direction and speed) of the curve at an endpoint.

*[convex]:  A convex geometric shape has the property that whenever two points are contained in the shape, then the line segment between those two points is entirely contained in the shape.

*[coordinate system]:  A way of assigning numerical coordinates to geometric points. In two dimensions, each point corresponds to a pair of numbers. In three dimensions, each point corresponds to a triple of numbers.

*[coordinate systems]:  A way of assigning numerical coordinates to geometric points. In two dimensions, each point corresponds to a pair of numbers. In three dimensions, each point corresponds to a triple of numbers.

*[CPU]:  The Central Processing Unit in a computer, the component that actually executes programs. The CPU reads machine language instructions from the computer's memory and carries them out.

*[cross product]:  A vector product of two 3D vectors. The cross product of v and w is a vector that is perpendicular to both v and w and whose length is equal to the absolute value of the sine of the angle between v and w. If v=(x,y,z) and w=(a,b,c), then their cross product is the vector (yc-zb,za-xc,xb-ya).

*[CSS]:  Cascading Style Sheets. A language that is used for specifying the style, or presentation, of the content of web pages. CSS can control things like colors, backgrounds, fonts, shadows, borders, and the size and position of elements of the page.

*[cubemap texture]:  A texture made up of six images, one for each of the directions positive x, negative x, positive y, negative y, positive z, and negative z. The images are intended to include everything that can be seen from a given point. Cubemap textures are used for environment mapping and skyboxes.

*[deferred shading]:  A multi-pass rendering technique where a first pass processes the geometry and saves relevant information such as transformed coordinates, normal vectors, and material properties. The data can be stored in textures, which are called "geometry buffers" or "G-buffers" in this context. Lighting and other effects can then be computed in additional passes, using the pre-computed information from the geometry buffers instead of re-computing it for each pass.

*[depth buffer]:  A region of memory that stores the information needed for the depth test in 3D graphics, that is, a depth value for each pixel in the image. Also called the "z-buffer."

*[depth mask]:  In WebGL, a setting that controls whether depth values are written to the depth buffer during rendering. When the depth mask is set to false, the depth value is discarded and the depth buffer is unchanged.

*[depth test]:  A solution to the hidden surface problem that involves keeping track of the depth, or distance from the viewer, of the object currently visible at each pixel in the image. When a new object is drawn at a pixel, the depth of the new object is compared to the depth of the current object to decide which one is closer to the viewer. The advantage of the depth test is that objects can be rendered in any order. A disadvantage is that only a limited range of depths can be represented in the image.

*[device coordinates]:  The coordinate system used on a display device or rendered image, often using pixels as the unit of measure.

*[diffuse color]:  A material property that represents the proportion of incident light that is reflected diffusely from a surface.

*[diffuse reflection]:  Reflection of incident light in all directions from a surface, so that diffuse illumination of a surface is visible to all viewers, independent of the viewer's position.

*[Direct3D]:  Microsoft's proprietary API for 3D graphics on the Windows operating system.

*[directed acyclic graph]:  Also called a "dag." A linked data structure in which there are no cycles. That is, it is not possible to find a sequence of nodes where each node links to the next and the last node links back to the first.

*[directional light]:  A light source whose light rays are parallel, all arriving from the same direction. Can be considered to be a light source at an effectively infinite distance. Also called a "sun," since the Sun is an example of a directional light source.

*[displacement mapping]:  A technique used to modify a polygonal mesh by moving, or displacing, the vertices of the mesh.

*[display list]:  A list of graphics primitives and attributes which can be traversed to create all or part of an image. Display lists were used in some early vector-graphics hardware. They were also available in traditional OpenGL.

*[DOM]:  Document Object Model. A specification for representing a web page (and other kinds of structured document) as a tree-like data structure. Can also refer to the data structure itself, as in "the DOM for this web page." A web page can be modified dynamically by manipulating its DOM, using the JavaScript programming language.

*[dot product]:  The dot product of two vectors is the sum of the products of corresponding coordinates. For 3D vectors `v=(x,y,z)` and `w=(a,b,c)`, the dot product of v and w is `x*a+y*b+z*c`. The dot product is equal to the cosine of the angle between the vectors, divided by the product of their lengths.

*[double buffering]:  A graphics technique in which an image is drawn off-screen, in a region of memory called an off-screen buffer or "back buffer." When the image is drawn, it can be copied to the buffer that represents the contents of the screen, which is also known as the "front buffer." In true double buffering, the image doesn't have to be copied; instead, the buffers can be "swapped" so that the back buffer becomes the front buffer, and the front buffer becomes the back buffer.

*[drawing program]:  A computer program for creating images using vector-style graphics, where the user creates the image by specifying shapes that make up the image and their attributes.

*[Eclipse]:  An integrated development environment for writing programs in Java (and other programming languages). Eclipse is a free program that can be downloaded from <http://eclipse.org>.

*[emission color]:  A material property that represents color that is intrinsic to a surface, rather than coming from light from other sources that is reflected by the surface. Emission color can make the object look like it is glowing, but it does not illuminate other objects. Emission color is often called "emissive color."

*[environment mapping]:  A way of simulating mirror-like reflection from the surface of an object. The environment that is to be reflected from the surface is represented as a cubemap texture. To determine what point in the texture is visible at a given point on the object, a ray from the viewpoint is reflected from the surface point, and the reflected ray is intersected with the texture cube. Environment mapping is also called reflection mapping.

*[ES6]:  A version of JavaScript implemented by almost all modern web browsers. More formally known as ECMAScript 6 or ECMAScript 2015. ES6 introduced a large number of new features.

*[Euclidean transform]:  A transform that preserves distances and angles. A Euclidean transform represents a "rigid motion." That is, the transform of an object is an exact copy of the object, with the same size and shape. Any Euclidean transform can be represented as a composition of rotations and translations.

*[Euler angles]:  Express the rotation of an object in its own coordinate system, given as individual rotations about the x, y, and z axes in that coordinate system. The cumulative effect of rotations about the three coordinate axes depends on the order in which the rotations are applied.

*[extrusion]:  A technique for producing a solid from a 2D shape by moving the shape along a curve in 3D. The solid is the set of points through which the shape passes as it moves along the curve. The most common case is moving the shape along a line segment that is perpendicular to the plane that contains the shape. In practice, in computer graphics, the object that is produced by extrusion is just the surface of the extruded solid.

*[eye coordinates]:  The coordinate system on 3D space defined by the viewer. In eye coordinates in OpenGL 1.1, the viewer is located at the origin, looking in the direction of the negative z-axis, with the positive y-axis pointing upwards, and the positive x-axis pointing to the right. The modelview transformation maps objects into the eye coordinate system, and the projection transform maps eye coordinates to clip coordinates.

*[filling a shape]:  Drawing the interior of a shape, by coloring the pixels that lie inside the shape. Filling does not apply to shapes, such as lines, that have no interior.

*[fixed-function pipeline]:  A graphics processing pipeline with a fixed set of processing stages that cannot be modified by a programmer. Data for an image passes through a sequence of processing stages, with the image as the end product. The sequence is called a "pipeline." With a fixed-function pipeline, the programmer can enable and disable stages and set options that control the processing but cannot add to the functionality.

*[flat shading]:  A lighting computation for the faces of a polygon or polygonal mesh that uses the same normal vector at each point in the polygon, giving the polygon a flat or faceted appearance.

*[fragment shader]:  A shader program that will be executed once for each pixel in a primitive. A fragment shader must compute a color for the pixel, or discard it. Fragment shaders are also called pixel shaders.

*[framebuffer]:  In WebGL, a data structure that organizes the buffers for rendering an image, possibly including a color buffer, a depth buffer, and a stencil buffer. A WebGL graphics context has a default framebuffer for on-screen rendering, and additional framebuffers can be created for off-screen rendering.

*[frame buffer]:  A region of memory that contains color data for a digital image. Most often refers to the memory containing the image that appears on the computer's screen.

*[front face]:  One of the two sides of a polygon in 3D. A polygon has two sides. One is taken to be the front face, and the other is the back face. In OpenGL, the difference is determined by the order in which the vertices of the polygon are enumerated. The default is that, seen from the front, the vertices are enumerated in counterclockwise order around the polygon.

*[frustum]:  A truncated pyramid; that is, a pyramid from which the top has been cut off. In OpenGL 1.1, the view volume for a perspective projection is a frustum.

*[geometric modeling]:  Creating a scene by specifying the geometric objects contained in the scene, together with geometric transforms to be applied to them and attributes that determine their appearance.

*[geometric primitive]:  Geometric objects in a graphics system, such as OpenGL, that are not made up of simpler objects. Examples in OpenGL include points, lines, and triangles, but the set of available primitives depends on the graphics system. (Note that as the term is used in OpenGL, a single primitive can be made up of many points, line segments, or triangles.)

*[geometric primitives]:  Geometric objects in a graphics system, such as OpenGL, that are not made up of simpler objects. Examples in OpenGL include points, lines, and triangles, but the set of available primitives depends on the graphics system. (Note that as the term is used in OpenGL, a single primitive can be made up of many points, line segments, or triangles.)

*[geometric transform]:  A coordinate transformation; that is, a function that can be applied to each of the points in a geometric object to produce a new object. Common transforms include scaling, rotation, and translation.

*[glMatrix]:  An open-source JavaScript library for vector and matrix math in two and three dimensions.

*[global ambient intensity]:  In OpenGL, ambient light that is present in the environment independent of any light source. Total ambient light is the sum of the global ambient light plus the ambient light intensity of each enabled light source.

*[global illumination]:  The goal of 3D rendering algorithms that take into account all the interactions of light in a scene, including indirect illumination by light that bounces off other objects.

*[GLSL]:  OpenGL Shader Language, the programming language that is used to write shader programs for use with OpenGL.

*[GLTF]:  GL Transfer Format. A file format for 3D models. A GLTF file can contain complete 3D scenes, including objects, materials, lights, and even animations. The GLTF specification comes from the Khronos Group, which is also responsible for OpenGL, WebGL, and Vulkan.

*[GLU]:  The OpenGL Utility library. Defines several functions for use with older versions of OpenGL, including gluPerspective and gluLookAt. Not to be confused with GLUT. GLU is a standard part of OpenGL.

*[GLUT]:  The OpenGL Utility Toolkit. A platform-independent library for writing OpenGL applications. OpenGL does not include support for windows or events. GLUT adds such support. It also has functions for drawing 3D shapes such as spheres and polyhedra (not to mention a teapot). GLUT is written in the C programming language and is used with the C API for OpenGL. However, many GLUT functions are also available in JOGL, the Java API for OpenGL. A newer, and somewhat improved, version of the toolkit named "FreeGLUT" is commonly used in place of the original version.

*[GPU]:  Graphics Processing Unit, a computer hardware component that performs graphical computations that create and manipulate images. Operations such as drawing a line on the screen or rendering a 3D image are done in the GPU, which is optimized to perform such operations very quickly.

*[gradient]:  A pattern of color produced by assigning colors to certain reference points and computing color for other points by interpolating or extrapolating colors from the reference points. The effect is a color progression along line segments between reference points. Different rules for extending the colors beyond those lines produce different types of gradient, such as linear gradients and radial gradients.

*[grayscale]:  Refers to a color scheme or image in which each color is a shade of gray (where the term "shade of gray" here includes black and white). Typically, 256 shades of gray are used. Grayscale is also called "monochrome."

*[GUI]:  (Graphical User Interface.) A user interface for a program where the user interacts with the program using components such as windows, menus, buttons, and text-input boxes.

*[HDR image]:  A high dynamic range image. An HDR image has more color information than the usual eight bits per color channel per pixel. This makes it more suitable to uses that require calculation with the color values.

*[height map]:  An image in which the grayscale value represents a height, or elevation. Height maps can be used in displacement mapping to specify the amount of displacement.

*[hidden surface problem]:  The problem in 3D graphics of deciding which object is visible at each pixel in an image. When one object is behind another object from the point of view of the viewer, only the front object should appear in the image. A rendering algorithm for 3D graphics must satisfy this constraint. Algorithms that solve the hidden surface problem include the painter's algorithm and the depth test algorithm.

*[hierarchical modeling]:  Creating complex geometric models in a hierarchical fashion, starting with geometric primitives, combining them into components that can then be further combined into more complex components, and so on.

*[homogeneous coordinates]:  A way of representing n-dimensional vectors as (n+1)-dimensional vectors where two (n+1) vectors represent the same n-dimensional vector if they differ by a scalar multiple. In 3D, for example, if w is not zero, then the homogeneous coordinates (x,y,z,w) are equivalent to homogeneous coordinates (x/w,y/w,z/w,1), since they differ by multiplication by the scalar w. Both sets of coordinates represent the 3D vector (x/w,y/w,z/w)

*[HSL color]:  A color specified by three numbers giving the hue, saturation, and lightness of the component. The HSL color model is similar to the HSV color model. The main difference is that in HSL, pure spectral colors occur when L=0.5, while in HSV, they occur when V=1.

*[HSV color]:  A color specified by three numbers giving the hue, saturation, and value of the component. The hue represents the basic color. The saturation is the purity of the color, with a saturation value of zero producing a shade of gray, that is a color with no actual hue at all. The value represents the brightness of the color, with a value of zero giving black. (Value is also called brightness, and the name HSB is sometimes used instead of HSV.)

*[HTML]:  HyperText Markup Language. A language that is used for specifying the content of web pages. An HTML document is made up of text, along with "elements" for adding other content, such as images, and for defining the structure of the document. Because of nesting of elements, the document can be represented by a tree-like data structure.

*[HTML canvas]:  A canvas element on a web page. The canvas appears as a rectangular area on the page. The JavaScript programming language can use a canvas element as a drawing surface. HTML is a language for specifying the content of a web page. JavaScript is the programming language for web pages. The canvas element supports a 2D graphics API. In many browsers, it also supports the 3D graphics API, WebGL.

*[identity matrix]:  The n-by-n identity matrix is an n-by-n matrix which has ones on the diagonal and zeros elsewhere. Multiplication of any matrix B by the identity matrix, in either order, leaves B unchanged. Multiplication of an n-dimensional vector by the n-by-n identity matrix leaves the vector unchanged; that is, the identity matrix is the matrix for the identity transformation.

*[identity transform]:  A transform that has no effect on its argument. For example, the identity transform in 2D is given by the formula I(x,y) = (x,y). The identity transform I has the property that if T is any transform, then I followed by T is the same as T, and T followed by I is the same as T.

*[image texture]:  An image that is applied to a surface as a texture, so that it looks at if the image is "painted" onto the surface.

*[index buffer]:  In WebGPU, an index buffer is a GPU buffer that holds vertex indices for use with the drawIndexed(). A vertex index gives the position of a vertex in the list of vertices of a primitive.

*[indexed color]:  A color scheme in which colors are selected from a limited palette of colors. For example, if the palette contains 256 colors, then a color can be specified by an eight-bit integer, giving its position, or index, in the list of colors.

*[indexed drawing]:  In WebGPU, drawing a primitive using the drawIndexed() function. With that function, vertices are not generated in the order in which they are listed. Instead, a list of vertex indices in an index buffer determines the order of the vertices. Indexed drawing is used to render indexed face sets.

*[indexed face set]:  (IFS). A data structure that represents a polyhedron or polygonal mesh. The data structure includes a numbered list of vertices and a list of faces. A face is specified by listing the indices of the vertices of the face; that is, a face is given as a list of numbers where each number is an index into the list of vertices.

*[instanced drawing]:  The ability to render multiple versions of a primitive with a single function call. Each copy can have its own values for certain attributes, such as color or transformation.

*[intensity of a light source]:  A light source emits light at various wavelengths. The intensity of a light at a given wavelength is the amount of energy in the light at that wavelength. The total intensity of the light is its total energy at all wavelengths. The color of a light is determined by its intensities at all wavelengths.

*[interpolation]:  Given values for some quantity at certain reference points, computing a value for that quantity at other points by some kind of averaging applied to the values at the reference points.

*[invariant qualifier]:  In GLSL, a modifier that ensures that when the same expression is used to compute the value of a variable in two different shaders, the value will be the same in both shaders. This can be important for multi-pass algorithms, where several shader programs are applied in succession to render one image.

*[inverse transform]:  Given a transform T, the inverse transform of T is a transform that reverses the operation of T. For example, for a 2D transform, for R to be the inverse of T means that R(T(x,y)) = (x,y). Scaling by 0.5 is the inverse of scaling by 2. Translation by (-3,5) is the inverse of translation by (3,-5). Not every transform has an inverse. For example, scaling by a factor of zero has no inverse.

*[IOR]:  Index of Refraction. A property of a medium, such as air or glass, that transmits light. The refraction, or bending, of light rays that pass from one medium to another depends on the ratio of the IORs of the two media. The index of refraction of a medium depends on the speed of light in that medium.

*[JavaScript]:  A programming language for web pages. JavaScript code on a web page is executed by a web browser that displays the page, and it can interact with the contents of the web page and with the user. There are JavaScript APIs for 2D and for 3D graphics

*[JOGL]:  A Java implementation of OpenGL. JOGL is very complicated, since it attempts to support all versions of OpenGL in one programming system. JOGL integrates seamlessly with Java's Swing and AWT graphics.

*[JSON]:  (JavaScript Object Notation.) A syntax for representing JavaScript objects as strings, similar to the object literal syntax that is used in JavaScript. JSON objects cannot contain functions, but they can contain strings, numbers, and booleans. JSON has become a popular standard for storage and transmission of structured data.

*[keyframe animation]:  An animation technique in which the value of some quantity is given explicitly only at certain times during the animation. The times when the quantity is specified are called keyframes. Between keyframes, the value of the quantity is obtained by interpolating between the values specified for the keyframes.

*[Lambert shading]:  A technique for computing pixel colors on a primitive using a lighting equation that takes into account ambient and diffuse reflection. In Lambert shading, the lighting equation is applied only at the vertices of the primitive. Color values for pixels in the primitive are calculated by interpolating the values that were computed for the vertices. Lambert shading is named after Johann Lambert, who developed the theory on which it is based in the eighteenth century.

*[lathing]:  A technique for producing a surface by rotating a planar curve about a line that lies in the same plane as the curve. As each point rotates about the line, it generates a circle. The surface is the union of the circles generated by all the points on the curve. Lathing imitates shapes that can be produced by a mechanical lathe.

*[length of a vector]:  A vector is defined by its length and its direction, so length is a fundamental property. When a vector is represented as an arrow, its length is just the length of that arrow. For a 2D vector given by coordinates (x,y), the length is the square root of `x*x+y*y`. For a 3D vector given as (x,y,z), the length is the square root of `x*x+y*y+z*z`.

*[lighting]:  Using light sources in a 3D scene, so that the appearance of objects in the scene can be computed based on the interaction of light with the objects' material properties.

*[lighting equation]:  The equation that is used in OpenGL to compute the visible color of a point on a surface from the material properties of the surface, the normal vector for that point, the direction to the viewer, the ambient light level, and the direction and intensity of light sources.

*[linear algebra]:  The field of mathematics that studies vector spaces and linear transformations between them. Linear algebra is part of the essential mathematical foundation of computer graphics.

*[linear gradient]:  A color gradient pattern in which there is a color variation along a certain line, with constant color along lines perpendicular to that line.

*[linear transformation]:  A function from one vector space to another that preserves vector addition and multiplication by constants. Linear transformations can be represented by matrices. In computer graphics, they are used to implement geometric operations such as rotation and translation.

*[lossless data compression]:  A scheme for reducing the size of a dataset without losing any of the information in that dataset. The original data can be recovered exactly from the compressed data. The image formats GIF and PNG use lossless data compression to reduce the size of the image file.

*[lossy data compression]:  A scheme for reducing the size of a dataset in which some of the information in the dataset can be lost. The data that is recovered from the compressed data can differ from the original data. The image format JPEG use lossy data compression to reduce the size of the image file.

*[luminance]:  A quantity representing the perceived brightness of a color. For an RGB color, it is a weighted average of the red, green, and blue components of the color. The usual formula is `0.3*red + 0.59*green + 0.11*blue`.

*[magnification filter]:  An operation that is used when applying a texture to an object, when the texture has to be stretched to fit the object. For an image texture, a magnification filter is applied to compute the color of a pixel when that pixel covers just a fraction of a pixel in the image.

*[material]:  The properties of an object that determine how that object interacts with light in the environment. Material properties in OpenGL include, for example, diffuse color, specular color, and shininess.

*[matrix]:  A rectangular array of numbers. A matrix can be represented as a two-dimensional array, with numbers arranged in rows and columns. An N-by-N matrix represents a linear transformation from N-dimensional space to itself.

*[matrix mode]:  In OpenGL 1.1, a state variable that determines which one of several transformation matrices will be affected by functions such as glRotatef and glFrustum. The matrix mode is set with the function glMatrixMode. Possible values include GL_MODELVIEW, GL_PROJECTION, and GL_TEXTURE.

*[Metal]:  Apple's proprietary API for 3D graphics and computation on MacOS computers and iOS devices.

*[minification filter]:  An operation that is used when applying a texture to an object, when the texture has to be shrunk to fit the object. For an image texture, a minification filter is applied to compute the color of a pixel when that pixel covers several pixels in the image.

*[mipmap]:  One of a series of reduced-size copies of a texture image, of decreasing width and height. Starting from the original image, each mipmap is obtained by dividing the width and height of the previous image by two (unless it is already 1). The final mipmap is a single pixel. Mipmaps are used for more efficient mapping of the texture image to a surface, when the image has to be shrunk to fit the surface.

*[mipmaps]:  One of a series of reduced-size copies of a texture image, of decreasing width and height. Starting from the original image, each mipmap is obtained by dividing the width and height of the previous image by two (unless it is already 1). The final mipmap is a single pixel. Mipmaps are used for more efficient mapping of the texture image to a surface, when the image has to be shrunk to fit the surface.

*[modeling transformation]:  A transformation that is applied to an object to map that object into the world coordinate system or into the object coordinate system for a more complex, hierarchical object.

*[modelview transformation]:  In OpenGL 1.1, a transform that combines the modeling transform with the viewing transform. That is, it is the composition of the transformation from object coordinates to world coordinates and the transformation from world coordinates to eye coordinates. Because of the equivalence between modeling and viewing transformations, world coordinates are not really meaningful for OpenGL, and only the combined transformation is tracked.

*[multi-pass algorithm]:  A rendering algorithm that draws a scene several times and combines the results somehow to compute the final image. A simple example is anaglyph stereo, in which a left-eye and right-eye image of the scene are rendered separately and combined.

*[multisampling]:  A kind of antialiasing where the fragment shader is evaluated at several points in each pixel, and the results are averaged to get the color of the pixel.

*[NDC]:  Normalized Device Coordinates. In WebGPU, refers to the default xyz coordinate system in which x and y range from -1 to 1 and z ranges from 0 to 1. The x and y in NDC map linearly to device, or pixel, coordinates on the viewport.

*[nio buffer]:  A Java object belonging to the class java.nio.Buffer or one of its subclasses. Nio buffers are similar to arrays, but they are optimized for input/output operations. Nio buffers are used instead of arrays for certain purposes in Java's JOGL API for OpenGL.

*[normalized vector]:  The result of dividing a non-zero vector by its length, giving a unit vector, that is, a vector of length one. (Note that "normalized vector" and "normal vector" are, confusingly, unrelated terms!)

*[normal vector]:  A normal vector to a surface at a point on that surface is a vector that is perpendicular to the surface at that point. Normal vectors to curves are defined similarly. Normal vectors are important for lighting calculations.

*[norm of a vector]:  Another term for the length of the vector. For a 3D vector given as (x,y,z), the norm is the square root of `x*x+y*y+z*z`.

*[object coordinates]:  The coordinate system in which the coordinates for points in an object are originally specified, before they are transformed by any modeling or other transform that will be applied to the object.

*[off-screen canvas]:  My term for a segment of the computer's memory that can be used as a drawing surface, for drawing images that are not visible on the screen. Some method should exist for copying the image from an off-screen canvas onto the screen. In Java, for example, an off-screen canvas can be implemented as an object of type BufferedImage.

*[OpenGL]:  A family of computer graphics APIs that is implemented in many graphics hardware devices. There are several versions of the API, and there are implementations, or "bindings" for several different programming languages. Versions of OpenGL for embedded systems such as mobile phones are known as OpenGL ES. WebGL is a version for use on Web pages. OpenGL can be used for 2D as well as for 3D graphics, but it is most commonly associated with 3D.

*[orthographic projection]:  A projection from 3D to 2D that simply discards the z-coordinate. It projects objects along lines that are orthogonal (perpendicular) to the xy-plane. In OpenGL 1.1, the view volume for an orthographic projection is a rectangular solid.

*[painter's algorithm]:  A solution to the hidden surface algorithm that involves drawing the objects in a scene in order from back to front, that is, in decreasing order of distance from the viewer. A disadvantage is that the order is usually not well-defined unless some objects are decomposed into smaller sub-objects. Another issue is that the order of drawing has to change when objects move or when the point of view changes.

*[painting program]:  A computer program for creating images using raster-style graphics, where the user creates the image by controlling the colors of each pixel.

*[path tracing]:  A rendering algorithm based on the idea of computing all the paths that light could have followed to arrive at the position of a viewer from each direction. Since that is literally impossible, the algorithm traces a random sample of paths and averages the results. As the number of samples increases, the average converges to a very high-quality image.

*[pattern fill]:  Using copies of an image to fill the interior of a two-dimensional shape. The image can be repeated horizontally and vertically as necessary to cover the shape.

*[PBR]:  Physically Based Rendering. A general term encompassing a variety of techniques for rendering materials that look more physically realistic than the materials traditionally used in OpenGL and similar graphics APIs. The idea is to implement the actual physics of light and material more directly. PBR has become common in real-time graphics such as video games.

*[Perlin noise]:  A technique invented by Ken Perlin in 1983 that is used in the computation of natural-looking procedural textures. A Perlin noise function has numerical inputs (usually 2 or 3) and produces an output number in the range -1.0 to 1.0. The output is pseudo-random, but has some regularity, with features that are similarly sized and regularly distributed, and with variation on several scales.

*[per-pixel lighting]:  Doing lighting calculations at each pixel of a primitive, which gives better results in most cases than per-vertex lighting. Phong shading uses per-pixel lighting, with normal vectors interpolated from the vertices.

*[perspective projection]:  A projection from 3D to 2D that projects objects along lines radiating out from a viewpoint. A perspective projection attempts to simulate realistic viewing. A perspective projection preserves perspective; that is, objects that are farther from the viewpoint are smaller in the projection. In OpenGL 1.1, the view volume for a perspective projection is a frustum, or truncated pyramid.

*[per-vertex lighting]:  Doing lighting calculations only at the vertices of a primitive, and interpolating the results to get the colors of interior pixels. Per-vertex lighting is the standard in traditional OpenGL. Per-vertex lighting without specular reflection is Lambert shading.

*[Phong shading]:  A technique for computing pixel colors on a primitive using a lighting equation that takes into account ambient, diffuse, and specular reflection. In Phong shading, the lighting equation is applied at each pixel. Normal vectors are specified only at the vertices of the primitive. The normal vector that is used in the lighting equation at a pixel is obtained by interpolating the normal vectors for the vertices. Phong shading is named after Bui Tuong Phong, who developed the theory in the 1970s.

*[pipeline]:  A sequence of computational stages in a GPU that are applied to incoming data to produce some result. Some of the stages can be programmable shaders, such as vertex shaders, fragment shaders, and compute shaders. In a graphics rendering pipeline, the output is the colors of the pixels in an image.

*[pixel]:  A digital image is made up of rows and columns of small rectangles called pixels. To specify a digital image, a color is assigned to each pixel in the image.

*[pixels]:  A digital image is made up of rows and columns of small rectangles called pixels. To specify a digital image, a color is assigned to each pixel in the image.

*[point light]:  A light source whose light rays emanate from a single point. Also called a "lamp," since a lamp approximates a point source of light. Also called a positional light.

*[polygon]:  A multi-sided shape lying in a plane and specified by a list of points, called its vertices, and made up of the line segments from each point in the list to the next point in the list, plus a line segment from the last point in the list to the first point. All the points are required to lie in the same plane. Sometimes the term "polygon" includes the interior of the shape as well as its boundary.

*[polygonal mesh]:  A collection of polygons, where the polygons can be joined together along their edges. A polygonal mesh can represent a polyhedron, or can be used as an approximation for a curved surface. A polygonal mesh can be represented as an indexed face set.

*[polygon offset]:  A 3D graphics technique that slightly increases or decreases the depth of the pixels in a primitive as it is rendered. Polygon offset is used to avoid having several objects at exactly the same depth, a situation that is not handled well by the depth test.

*[polyhedron]:  A closed 3D figure whose faces, or sides, are polygons. Usually, it is assumed that the faces of a polyhedron do not intersect, except along their edges.

*[power-of-two texture]:  A texture image whose width and height are powers of two. In some graphics systems, this is a requirement of any image that is to be used as a texture.

*[precision qualifier]:  In GLSL, one of the following modifiers on a numeric variable declaration: lowp, mediump, or highp. A precision modifier specifies the minimum number of bits or range of values for the variable.

*[procedural texture]:  A texture for which the value at a given set of texture coordinates is computed as a mathematical function of the coordinates, as opposed to an image texture where the value is obtained by sampling an image.

*[programmable pipeline]:  A graphics processing pipeline in which some of the processing stages can or must be implemented by programs. Data for an image passes through a sequence of processing stages, with the image as the end product. The sequence is called a "pipeline." Programmable pipelines are used in modern GPUs to provide more flexibility and control to the programmer. The programs for a programmable pipeline are known as shaders and are written in a shader programming language such as GLSL.

*[projected]: A transformation that maps coordinates in 3D to coordinates in 2D. Projection is used to convert a three-dimensional scene into a two-dimensional image.

*[projection]:  A transformation that maps coordinates in 3D to coordinates in 2D. Projection is used to convert a three-dimensional scene into a two-dimensional image.

*[projection transformation]:  In 3D graphics, a transformation that maps a scene in 3D space onto a 2D image. In OpenGL 1.1, the projection maps the view volume (that is, the region in 3D space that is visible in the image) to clip coordinates, in which the values of x, y, and z range from -1 to 1. The x- and y-coordinates are then mapped to the image, while the z coordinate provides depth information.

*[promise (in JavaScript)]:  In JavaScript programming, a promise represents a result that might be available immediately or at some time in the future. A programmer can provide a function to be called if and when the promise is fulfilled (that is when the result becomes available). A programmer can also provide a function to be called when the promise is rejected (for example, if some error occurs). Promises are asynchronous since the function that handles success or failure will be called at some unpredictable time.

*[quad]:  A quadrilateral, that is a four-sided figure in the plane. OpenGL 1.1 has the primitives GL_QUADS and GL_QUAD_STRIP for drawing quads, but it assumes without checking that the vertices that are provided are in fact planar and define quadrilaterals that are convex.

*[quaternion]:  A vector in the quaternion algebra, which is a four dimensional vector space in which two vectors, in addition to being added, can be multiplied. In computer graphics, quaternions of length one are often used to represent rotations. An advantage is that in the quaternion representation, it is possible to smoothly interpolate between two rotations.

*[radial gradient]:  A color gradient pattern in which there are concentric circles, or sometimes ellipses, of constant color, with a color variation along the radius of the circles.

*[raster graphics]:  Pixel-based graphics in which an image is specified by assigning a color to each pixel in a grid of pixels.

*[rasterization]:  The process of creating a raster image, that is one made of pixels, from other data that specifies the content of the image. For example, a vector graphics image must be rasterized in order to be displayed on a computer screen.

*[ray casting]:  The process of following a ray (that is, half of an infinite line) starting at a given point and extending in a given direction, in order to find points of intersection of the ray with objects in a scene. Usually, only the intersection point that is closest to the starting point of the ray is of interest.

*[ray tracing]:  A recursive rendering algorithm that uses ray casting. A ray is cast from the viewpoint through a point in the image and into the scene, to determine what is seen at that point. To determine the color that is seen at that point, further rays are cast from the point, including a reflected ray (if the object has specular reflections), a refracted ray (if the object is translucent) and shadow rays towards light sources (to determine whether the object is illuminated by that light). Finding a color for a reflected or refracted ray can use a recursive application of the ray tracing algorithm.

*[real-time graphics]:  The type of computer graphics that is needed for computer animation or other applications where the images must be rendered quickly, at the time when they are viewed. For computer animation, real-time graphics generally requires the ability to render the scene sixty times per second.

*[reflection mapping]:  Another name for environment mapping.

*[reflectivity]:  The proportion or fraction of incident light that is reflected by an object. An object can have different reflectivities at different wavelengths. The color of an object is determined by its reflectivities at all wavelengths.

*[refraction]:  The bending of light as it passes from one transparent or translucent medium into another.

*[regular polygon]:  A polygon in which all the sides have the same length and all the angles between consecutive sides are equal. Usually the term is restricted to simple polygons, which have sides that do not intersect except at their endpoints.

*[regular polyhedron]:  A polyhedron in which each face is a regular polygon, and all the faces and angles are identical. There are only five regular polyhedra: the tetrahedron with 4 triangular faces, the cube with 6 square faces, the octahedron with 8 triangular faces, the dodecahedron with 12 pentagonal faces, and the icosahedron, with 20 triangular faces.

*[renderbuffer]:  In WebGL, a buffer (that is, a region of memory) that can be attached to a framebuffer for use as a color buffer, depth buffer, or stencil buffer.

*[rendering]:  The process of producing a 2D image from a 3D scene description.

*[render-to-texture]:  A technique in which the output of a rendering operation is written directly to a texture. In WebGL, render-to-texture can be implemented by attaching the texture as one of the buffers in a framebuffer.

*[RGBA color]:  An RGB color—specified by red, green, and blue component values—together with an alpha component. The alpha component is most often take to specify the degree of transparency of the color, with a maximal alpha value giving a fully opaque color.

*[RGB color]:  A color specified by three numbers giving the amount of red, green, and blue in the color.

*[right-handed coordinate system]:  A coordinate system on 3D space in which the x, y, and z-axes satisfy this property: If you point the thumb of your right hand in the direction of the positive z-axis, then your fingers will curl from the positive x-axis towards the positive y-axis.

*[right-hand rule]:  A rule that is used to determine the positive direction of rotation about an axis in 3D space: If you point the thumb of your right hand in the direction of the axis, then your fingers will curl in the direction of positive angles of rotation. Note that this assumes that the axis has a direction; in OpenGL, an axis of rotation is determined by the point (0,0,0) and another point (x,y,z), and the direction of the axis is from (0,0,0) towards (x,y,z).

*[rotation]:  A geometric transform that rotates each point by a specified angle about some point (in 2D) or axis (in 3D).

*[sampler variable]:  In GLSL, a variable in a shader program that can be used to do lookup in an image texture. The value of a sampler variable specifies the texture unit that will be used to do the lookup. In WebGL, sampler variables are of type "sampler2D" or "samplerCube."

*[sampling]:  The operation of mapping texture coordinates to colors from a texture, including using mipmaps if available and applying a minification or magnification filter if necessary.

*[scalar product]:  The product of a number and a vector. The scalar product of a number s and vector v is the vector obtained by multiplying each coordinate of v by s. In 3D, if s is a number and v=(x,y,z), then the scalar product of s times v is the vector (sx,sy,sz).

*[scaling]:  A geometric transform that multiplies each coordinate of a point by a number called the scaling factor. Scaling increases or decreases the size of an object, but also moves its points closer to or farther from the origin. Scaling can be uniform—the same in every direction—or non-uniform—with a different scaling factor in each coordinate direction. A negative scaling factor can be used to apply a reflection.

*[scene description language]:  A language that can be used to specify graphics images by stating what's in the image. That is, the scene is created "declaratively," by stating what it contains, as opposed to being created "procedurally," by a program. A document written in a scene description language can be used to generate a scene graph for the scene.

*[scene graph]:  A data structure that represents the objects in a scene, together with attributes of the objects and the modeling transformations that are applied to the objects. An image of the scene is created by traversing the scene graph data structure. A scene graph might exist only conceptually, or it might be an actual data structure in a program.

*[shader]:  A program to be executed at some stage of the rendering pipeline. OpenGL shaders are written in the GLSL programming languages. For WebGL, only vertex shaders and fragment shaders are supported. WebGPU also has compute shaders, which are used in compute pipelines.

*[shadow mapping]:  A technique for determining which parts of a scene are illuminated and which are in shadow from a given light source. The technique involves rendering the scene from the point of the view of the light source, but uses only the depth buffer from that rendering. The depth buffer is the "shadow map." Along a given direction from the light source, the object that is illuminated by the light is the one that is closest to the light. The distance to that object is essentially encoded in the depth buffer. Objects at greater distance are in shadow.

*[shadow ray]:  In the ray tracing algorithm, a ray that is cast from a point on object in the direction of a light source to determine whether that point is illuminated by that light source or is in shadow.

*[shear transform]:  A shear transformation in 2D leaves some line, L, fixed, and lines perpendicular to L are "tilted" relative to L by the same angle. Another description is that a line parallel to L is mapped to itself, but is moved by an amount proportional to its distance from L. In 3D, a shear transformation leaves some plane, P, fixed, and it maps a plane parallel to P to itself, but moved by an amount proportional to its distance from P.

*[shininess]:  A material property that determines the size and sharpness of specular highlights. Also called the "specular exponent" because of the way it is used in lighting calculations. In OpenGL, shininess is a number in the range 0 to 128.

*[single buffering]:  As opposed to double buffering, a graphics technique in which the image is drawn directly to the screen (that is, to the buffer that serves as the source for the screen image). The disadvantage of single buffering is that, for a complex image, the user can observe the process of drawing the image.

*[skybox]:  A large cube that surrounds a scene and is textured with images that form a background for that scene, in all directions.

*[smooth shading]:  A lighting computation for the faces of a polygon or polygonal mesh that uses a different normal vector at each vertex of the polygon. When two polygons share a vertex, both polygons use the same normal vector for that vertex, resulting in a smooth appearance at that vertex. Smooth shading is appropriate when a polygonal mesh is used as an approximation for a smooth surface.

*[specular color]:  A material property that represents the proportion of incident light that is reflected specularly by a surface.

*[specular exponent]:  A material property that determines the size and sharpness of specular highlights. Called "shininess" in OpenGL.

*[specular highlight]:  Illumination of a surface produced by specular reflection. A specular highlight is seen at points on the surface where the angle from the surface to the viewer is approximately equal to the angle from the surface to a light source.

*[specular reflection]:  Mirror-like reflection of light rays from a surface. A ray of light is reflected as a ray in the direction that makes the angle of reflection equal to the angle of incidence. A specular reflection can only be seen by a viewer whose position lies on the path of the reflected ray.

*[spotlight]:  A light that emits a cone of illumination. A spotlight is similar to a point light in that it has a position in 3D space, and light radiates from that position. However, the light only affects objects that are in the spotlight's cone of illumination.

*[stack]:  A data structure with the operations push() and pop(). Pushing an item onto a stack just adds that item to the stack. Popping from the stack will remove and return the item that was most recently pushed onto the stack.

*[storage buffer]:  In WebGPU, a general purpose buffer on the GPU, which can be used in compute shaders as well as in vertex and fragment shaders.

*[storage qualifier]:  In GLSL, one of the following modifiers on a variable declaration: uniform, attribute, varying, or const.

*[stroking a shape]:  Drawing the outline of a shape, as if a pen is dragged along the boundary of the shape. For a shape with no interior, such as a line segment, stroking the shape simply means dragging the pen along the shape.

*[subsurface scattering]:  A lighting effect in which light enters a slightly translucent object, is reflected internally one or more times, and then exits the object at a different point. Subsurface scattering contributes to the appearance of materials such as jade, milk, and skin.

*[SVG]:  Scalable Vector Graphics. An XML language for specifying 2D vector graphics. SVG is a scene description language. It is designed to integrate into web pages.

*[swizzler]:  In GLSL and WGSL, a notation such as v.yzx, where v is a vector and v.yzx represents the three-component vector made up of the y, z, and x components of v. Technically, any use of the dot notation with vectors is considered to be a swizzler.

*[texel]:  A pixel in a texture image.

*[texture]:  Variation in some property from point-to-point on an object. The most common type is image texture. When an image texture is applied to a surface, the surface color varies from point to point.

*[texture coordinates]:  Refers to the 2D coordinate system on a texture image, or to similar coordinate systems for 1D and 3D textures. Texture coordinates typically range from 0 to 1 both vertically and horizontally, with (0,0) at the lower left corner of the image. The term also refers to coordinates that are given for a surface and that are used to specify how a texture image should be mapped to the surface.

*[texture object]:  A data structure that can potentially be stored on the graphics card, and which can hold a texture image, a set of mipmaps, and configuration data such as the current setting for the minification and magnification filters. Using texture objects makes it possible to switch rapidly between textures without having to reload the data into the graphics card.

*[texture repeat mode]:  Determines how texture coordinates outside the range 0.0 to 1.0 are treated when sampling an image texture. The texture image itself has vertical and horizontal coordinates in the range 0.0 to 1.0. For coordinates outside that range, the texture repeat mode CLAMP or CLAMP_TO_EDGE, for example, clamps the coordinates to the range 0.0 to 1.0, essentially extending the color at the edge of the image indefinitely in all directions. Other repeat modes include REPEAT and MIRRORED_REPEAT.

*[texture target]:  In OpenGL, one of several kinds of texture, such as 2D image texture, 1D texture, and cube map texture. A texture target is specified by a constant such as GL_TEXTURE_2D or GL_TEXTURE_CUBE_MAP_POSITIVE_X. The texture target is a parameter to many OpenGL functions that work with textures.

*[texture transformation]:  A transformation that is applied to texture coordinates before they are used to sample data from a texture. The effect is to translate, rotate, or scale the texture on the surface to which it is applied.

*[texture unit]:  A hardware component in a GPU that does texture lookup. (Can also refer to an abstraction for such a component, whether or not it is actually implemented in hardware.) That is, it maps texture coordinates to colors from an image texture. This is the operation called "sampling," and texture units are associated with sampler variables in GLSL shader programs.

*[three.js]:  A JavaScript library for 3D graphics. The library implements an object-oriented scene graph API. While it is used primarily with WebGL, three.js can also render 3D scenes using the 2D canvas graphics API.

*[TMU]:  Texture Mapping Unit, another name for texture unit (perhaps with a stronger implication of actual hardware support). Also called a TPU (Texture Processing Unit).

*[torus]:  A 3D geometric object having the shape of a doughnut (or bagel).

*[translation]:  A geometric transform that adds a given translation amount to each coordinate of a point. Translation is used to move objects without changing their size or orientation.

*[two-sided lighting]:  An option in OpenGL that allows the back face of a polygon to have different material properties from the front face. Also, when this option is on, the normal vector that is used in lighting calculations for the back face is taken to be the negative of the vector for the front face. (The negative of a vector points in the opposite direction.)

*[typed array]:  In JavaScript, an array type that is limited to holding numerical values of a single type. For example, the type Float32Array represents arrays that can hold 32-bit floating point values, and Uint8Array arrays can hold only 8-bit integer values. Such arrays are more efficient than general JavaScript arrays for numerical calculations. The were introduced into JavaScript along with HTML canvas graphics and WebGL.

*[uniform scaling]:  A scaling transformation in which the scaling factors in all directions are the same. Uniform scaling changes the size of an object without distorting its shape.

*[uniform variable]:  Variables that represent input to a shader program in a programmable graphics pipeline. A uniform variable has the same value at every vertex and at every pixel of a primitive.

*[unit normal]:  A normal vector of length one; that is, a unit vector that is perpendicular to a curve or surface at a given point on the curve or surface.

*[unit vector]:  A vector of length one.

*[unsigned byte]:  A data type representing 8-bit non-negative integer values, taking values in the range from 0 to 255.

*[URL]:  Uniform Resource Locator. An address of some resource on the World Wide Web. For example, "<http://math.hws.edu/grahicsbook>".

*[VAO]:  Vertex Array Object. In WebGL 2.0, a region of memory, typically on the graphics card, that holds a collection of attribute settings such as enabled state and values of vertex attribute pointers. All of the settings can then be selected simply by binding the VAO.

*[varying variable]:  A variable that is used to communicate values from the vertex shader to the fragment shader in the WebGL or OpenGL ES 2.0 graphics pipeline. A varying variable is assigned a value in the vertex shader. The value of the variable in the fragment shader for a pixel in the primitive is obtained by interpolating the values from the vertices of the primitive. (In newer versions of GLSL, which support additional shader stages, the term "varying variable" is replaced by the more general terms "in variable" and "out variable," which refer to variables that are used for input to or output from a shader.)

*[VBO]:  Vertex Buffer Object. A block of memory that can hold the coordinates or other attributes for a set of vertices. A VBO can be stored on a GPU. VBOs make it possible to send such data to the GPU once and then reuse it several times. In OpenGL, VBOs are used with the functions glDrawArrays and glDrawElements.

*[vector]:  An element of a vector space. Elements of a vector space can be added and can be multiplied by constants. For computer graphics, a vector is just a list or array containing two, three, or four numbers. Vectors in that sense are often used to represent points in 2D, 3D, or 4D space. Properly, however, a vector represents a quantity that has a length and a direction; a vector used in this way can be visualized as an arrow.

*[vector graphics]:  Shape-based graphics in which an image is specified as a list of the shapes or objects that appear in the image.

*[vertex]:  One of the points that define a geometric primitive, such as the two endpoints of a line segment or the three vertices of a triangle. (The plural is "vertices.") A vertex can be specified in a coordinate system by giving its x and y coordinates in 2D graphics, or its x, y, and z coordinates in 3D graphics.

*[vertex array]:  In OpenGL, an array that is used to store coordinates or other attribute values for vertices, to be used with the functions glDrawArrays and glDrawElements. A vertex array exists on the "client side" of OpenGL, and it must be transmitted to the GPU to be used. In Java's JOGL API for OpenGL, nio buffers are used instead of arrays.

*[vertex buffer]:  In WebGPU, a vertex buffer is a GPU data structure that holds values to be used as input the vertex shader.

*[vertex shader]:  A shader program that will be executed once for each vertex in a primitive. A vertex shader must compute the vertex coordinates in the clip coordinate system. It can also compute other properties, such as color.

*[viewing]:  Setting the position and orientation of the viewer in a 3D world, which determine what will be visible when the 2D image of a 3D world is rendered.

*[viewing transformation]:  The transformation in 3D graphics that maps world coordinates to eye coordinates. The viewing transform establishes the position, orientation, and scale of the viewer in the world.

*[viewport]:  The rectangular area in which the image for 2D or 3D graphics is displayed. The coordinates on the viewport are pixel coordinates, more properly called device coordinates since they are actual physical coordinates on the device where the image is being displayed.

*[viewport transformation]:  In OpenGL 1.1, the final transformation from clip coordinates to device coordinates. The viewport transformation maps the clipping cube (the cube in 3D given by x, y, and z coordinates in the range from -1 to 1) to the viewport (the rectangle in the drawing surface where the image is rendered).

*[view volume]:  In OpenGL 1.1, the region is 3D space that is visible in the rendered image. For orthographic projections, the view volume is a rectangular solid. For perspective projection, the view volume is a frustum (truncated pyramid).

*[view window]:  As used in this book, the window, or view window, for 2D graphics is the rectangle in the xy-plane that contains the portion of the plane that will be displayed in the image. (The corresponding term in 3D graphics is "view volume.")

*[Vulkan]:  An open-source cross-platform API for 3D graphics and computation, designed as a more modern and efficient replacement for OpenGL.

*[WebGL]:  A 3D graphics API for use on web pages. WebGL programs are written in the JavaScript programming language and display their images in HTML canvas elements. WebGL is based on OpenGL ES, the version of OpenGL for embedded systems, with a few changes to adapt it to the JavaScript language and the Web environment.

*[WebGL extension]:  An optional capability in WebGL that is not available in all implementations. The WebGL API has a function for checking whether a given extension is available and, if so, activating it.

*[WebGPU]:  A new JavaScript graphics API, similar to WebGL, but designed to let web programs access modern GPU capabilities such as compute shaders.

*[WGSL]:  The WebGPU Shader Language, the programming language in which shaders for use in WebGPU are written.

*[winding number]:  The winding number of a path about a point that does not lie on the path is the number of times that the path winds around the point, counting each 360-degree rotation in the positive direction about the point as one and each 360-degree turn in the negative direction as minus one. To compute the winding number, draw a ray extending from the point to infinity. Each crossing of the ray by the path counts as 1 if it crosses the ray going in the positive direction and as negative 1 if it crosses in the negative direction.

*[wireframe]:  A style of drawing a polyhedron or polygonal mesh in which only the edges are drawn, resulting in an image made up of line segments.

*[world coordinates]:  The coordinate system in which a scene is defined. The image that is produced of the scene will show the contents of the world coordinate system that lie within some view volume (for 3D) or view window (for 2D). Objects are defined in their own object coordinate system. Modeling transformations are then applied to place objects into the scene; that is, they transform object coordinates to world coordinates.

*[XML]:  eXtensible Markup Language. Not a single language as such, but a class of languages that follow certain syntax rules. For example, SVG is an XML language because it follows those rules, but it also has further restrictions on its syntax that make it appropriate for specifying 2D graphics. XML documents, like HTML documents, have a tree-like structure defined by "elements." However, HTML is not an XML language since it does not follow all the syntax rules. XHTML is an alternative language for web pages that is similar to HTML but follows XML syntax rules.
