*[像素]: 像素: 数字图像由称为像素的小矩形的行和列组成。为了指定数字图像，需要为图像中的每个像素分配一种颜色。

*[灰度]: 指一种颜色方案或图像，其中每种颜色都是灰色的一种色调（此处的“灰色色调(shade of gray)”包括黑色和白色）。通常使用256种灰度级别。灰度也称为“单色(monochrome)”。

*[索引色]: 一种颜色方案，其中颜色是从有限的调色板中选择的。例如，如果调色板包含256种颜色，则可以通过八位整数来指定颜色，给出其在颜色列表中的位置或索引。

*[帧缓冲区]: 包含数字图像的颜色数据的内存区域。通常指的是包含显示在计算机屏幕上的图像的内存。

*[光栅图形]: 基于像素的图形，在此类图形中，通过为像素网格中的每个像素分配一种颜色来指定图像。

*[矢量图形]: 基于形状的图形，在此类图形中，图像被指定为出现在图像中的形状或对象的列表。

*[属性]: 图形对象的属性，例如颜色。图像可以通过其包含的几何形状以及它们的属性来指定。

*[显示列表]: 包含图形基元和属性的列表，可以遍历以创建图像的全部或部分。一些早期的矢量图形硬件使用了显示列表。它们也在传统的OpenGL中可用。

*[绘画程序]: 一种使用光栅式图形创建图像的计算机程序，在此类程序中，用户通过控制每个像素的颜色来创建图像。

*[绘图程序]: 一种使用矢量式图形创建图像的计算机程序，在此类程序中，用户通过指定组成图像的形状及其属性来创建图像。

*[无损数据压缩]: 一种减小数据集大小而不丢失数据集中任何信息的方案。可以从压缩数据中精确地恢复原始数据。图像格式GIF和PNG使用无损数据压缩来减小图像文件的大小。

*[有损数据压缩]: 一种减小数据集大小的方案，其中数据集中的一些信息可能会丢失。从压缩数据中恢复的数据可能与原始数据不同。图像格式JPEG使用有损数据压缩来减小图像文件的大小。

*[坐标]: 一种将数值坐标分配给几何点的方法。在二维中，每个点对应一对数字。在三维中，每个点对应一组三个数字。

*[坐标系]: 一种将数值坐标分配给几何点的方法。在二维中，每个点对应一对数字。在三维中，每个点对应一组三个数字。

*[几何建模]: 通过指定场景中包含的几何对象，以及要应用于它们的几何变换和确定它们外观的属性来创建场景。

*[几何基元]: 图形系统中的几何对象，如OpenGL，它们不是由更简单的对象组成的。OpenGL中的示例包括点、线和三角形，但可用基元的集合取决于图形系统。（请注意，在OpenGL中使用的术语中，一个单独的基元可以由许多点(points)、线段(line segments)或三角形(triangles)组成。）

*[分层建模]: 以分层方式创建复杂的几何模型，从几何基元开始，将它们组合成组件，然后进一步将它们组合成更复杂的组件，依此类推。

*[几何变换]: 坐标变换；即可应用于几何对象中的每个点以产生新对象的函数。常见的变换包括缩放、旋转和平移。

*[缩放]: 一种几何变换，它将点的每个坐标乘以一个称为缩放因子的数。缩放增加或减少对象的大小，但也将其点移动到原点更近或更远的位置。缩放可以是均匀的——在每个方向上都相同——或非均匀的——在每个坐标方向上具有不同的缩放因子。可以使用负的缩放因子来应用反射。

*[旋转]: 一种几何变换，它围绕某个点（在2D中）或轴（在3D中）旋转每个点到指定角度。

*[平移]: 一种几何变换，它将点的每个坐标添加给定的平移量。平移用于移动对象而不改变其大小或方向。

*[材质]: 决定物体与环境中光线交互方式的属性。OpenGL中的材质属性包括漫反射颜色、镜面反射颜色和光泽度等。

*[纹理]: 在物体的点之间变化的某种属性。最常见的类型是图像纹理。当图像纹理应用于表面时，表面的颜色会从一个点到另一个点变化。

*[模拟光线]: 在3D场景中使用光源，以便基于光与物体的材质属性的相互作用来计算场景中物体的外观。

*[视图]: 设置观察者在3D世界中的位置和方向，从而确定渲染3D世界的2D图像时将可见的内容。

*[投影]: 将3D中的坐标映射到2D中的坐标的转换。投影用于将三维场景转换为二维图像。

*[光栅化]: 从指定图像内容的其他数据创建栅格图像的过程。例如，必须对矢量图形图像进行光栅化，以便在计算机屏幕上显示。

*[渲染]: 从3D场景描述生成2D图像的过程。

*[动画]: 一系列图像，当快速连续显示时，将产生连续运动或变化的印象。动画这个术语还指的是创建这样的图像序列的过程。

*[开放GL]: 计算机图形API系列，实现在许多图形硬件设备中。API有多个版本，并且有多种不同编程语言的实现或“绑定”。用于移动设备（如手机）的OpenGL版本称为OpenGL ES。WebGL是用于网页的版本。OpenGL可用于2D和3D图形，但通常与3D图形关联更多。

*[网页GL]: 用于网页的3D图形API。WebGL程序使用JavaScript编程语言编写，并在HTML画布元素中显示其图像。WebGL基于OpenGL ES，这是用于嵌入式系统的OpenGL版本，对其进行了一些改动以使其适应JavaScript语言和Web环境。

*[中央处理器]: 计算机中的中央处理单元，实际执行程序的组件。CPU从计算机的内存中读取机器语言指令并执行它们。

*[图形处理器]: 图形处理单元(Graphics Processing Unit), 执行创建和操作图像的图形计算的计算机硬件组件。诸如在屏幕上绘制直线或渲染3D图像之类的操作是在GPU中完成的，该组件被优化以非常快速地执行此类操作。

*[接口]: 应用程序编程接口。用于执行某项任务的相关类、函数、常量等的集合。API是一个“接口”，可以在不了解其功能实际实现方式的情况下使用它。

*[伏尔甘]: 用于3D图形和计算的开源跨平台API，设计为OpenGL的更现代和高效的替代品。

*[metal]: 苹果的专有API，用于MacOS计算机和iOS设备上的3D图形和计算。

*[direct3D]: 微软的专有API，用于Windows操作系统上的3D图形。

*[网页GPU]: 一种新的JavaScript图形API，类似于WebGL，但旨在让Web程序访问现代GPU功能，如计算着色器。

*[顶点缓冲对象]: 顶点缓冲对象。一块内存块，可容纳顶点集的坐标或其他属性。VBO可以存储在GPU上。VBO使得可以将此类数据一次性发送到GPU，然后多次重复使用。在OpenGL中，VBO与函数glDrawArrays和glDrawElements一起使用。

*[纹理对象]: 可以潜在地存储在图形卡上的数据结构，其中可以包含纹理图像、一组mipmap以及配置数据（例如当前设置的缩小和放大滤波器设置）。使用纹理对象可以在不必重新加载数据到图形卡的情况下快速切换纹理。

*[着色器]: 要在渲染管线的某个阶段执行的程序。OpenGL着色器是用GLSL编程语言编写的。对于WebGL，仅支持顶点着色器和片段着色器。WebGPU还具有计算着色器，用于计算管线中的计算。

*[顶点着色器]: 一个着色器程序，将在原语中的每个顶点上执行一次。顶点着色器必须计算剪辑坐标系统中的顶点坐标。它也可以计算其他属性，如颜色。

*[片段着色器]: 在原语中的每个像素上执行一次的着色器程序。片段着色器必须为像素计算颜色，或者丢弃它。片段着色器也称为像素着色器。

*[OpenGL着色语言]: OpenGL着色器语言(OpenGL Shader Language)，用于为OpenGL编写着色器程序的编程语言。

*[颜色模型]: 一种用数字指定颜色的方式。在颜色模型中，每种颜色都被分配了一个或多个数值组件值。例如，RGB颜色模型，其中颜色由三个数字表示，分别表示颜色的红色、绿色和蓝色分量。

*[抗混叠]: 一种用于减少使用像素绘制的对角线、文本和其他形状的锯齿或“阶梯”外观的技术。当一个像素仅被几何形状的一部分覆盖时，那么像素的颜色是几何形状的颜色和背景颜色的混合，混合程度取决于像素被几何形状覆盖的比例。

*[反锯齿]: A technique used to reduce the jagged or "staircase" appearance of diagonal lines, text, and other shapes that are drawn using pixels. When a pixel is only partly covered by a geometric shape, then the color of the pixel is a blend of the color of the shape and the color of the background, with the degree of blending depending on the fraction of the pixel that is covered by the geometric shape.

*[宽高比]: 矩形的宽度 w 与高度 h 的比率，表示为比率 w:h 或分数 w/h。

*[RGB颜色模型]: 由三个数字指定的颜色，分别表示颜色中红色、绿色和蓝色的量。

*[颜色分量]: 颜色模型中用于指定颜色的数字之一。例如，在 RGB 颜色模型中，一个颜色由三个颜色分量表示，分别代表颜色中红色、绿色和蓝色的量。

*[阿尔法]: 颜色模型中的额外组成部分（即用于指定颜色的数字之一），并不是实际颜色规范的一部分。阿尔法分量是额外信息。它通常用于指定颜色的透明度程度。

*[阿尔法混合]: 使用颜色的阿尔法分量将颜色与背景颜色混合，当颜色在背景颜色上绘制时。换句话说，像素的新颜色是通过将绘制颜色与当前颜色混合而获得的，混合程度取决于绘制颜色的阿尔法分量。阿尔法混合最常用于模拟透明效果。

*[布雷森汉姆线段绘制算法]: 一种用于确定要着色以表示几何线段的像素的特定算法，只使用整数运算。该算法可以在计算机硬件中非常高效地实现。

*[描边]: 绘制形状的轮廓，就像一支笔沿着形状的边界拖动一样。对于没有内部的形状，例如线段，描边形状只是沿着形状拖动笔。

*[填充]: 绘制形状的内部，通过着色位于形状内部的像素。填充不适用于没有内部的形状，例如线段。

*[绕数]: 关于不在路径上的点的路径的绕数是路径绕过该点的次数，每次以正方向围绕该点的360度旋转计为1，以负方向旋转的360度计为-1。要计算绕数，绘制一条从该点延伸到无限远的射线。射线与路径的每次交叉都计为1，如果以正方向交叉射线，则计为1，以负方向交叉则计为-1。

*[图案]: 使用图像的副本填充二维形状的内部。可以根据需要水平和垂直重复图像，以覆盖形状。

*[渐变]: 通过为某些参考点分配颜色，并通过对参考点的颜色进行插值或外推来计算其他点的颜色，从而产生的一种颜色模式。效果是在参考点之间的线段上的颜色渐变。通过不同的规则将颜色扩展到这些线段之外，可以产生不同类型的渐变，如线性渐变和径向渐变。

*[插值]: 在某些参考点上给定某个量的值，通过对参考点上的值进行某种平均来计算其他点上的该量的值。

*[线性渐变]: 一种颜色渐变模式，在某一条直线上有颜色的变化，而在与该直线垂直的线上保持恒定的颜色。

*[径向渐变]: 一种颜色渐变模式，其中有同心圆或椭圆的恒定颜色，沿着圆的半径有颜色的变化。

*[多边形]: 一个位于平面上的多边形形状，由一系列点（称为顶点）指定，并由从列表中的每个点到下一个点的线段组成，以及从列表中的最后一个点到第一个点的线段。所有点都需要位于同一平面上。有时术语“多边形”包括形状的内部和边界。

*[正多边形]: 所有边长相等且相邻边之间的角度相等的多边形。通常该术语仅适用于简单多边形，其边除了端点外不相交。

*[凸多边形]: 具有以下性质的凸几何形状：当两个点都包含在形状内时，连接这两个点的线段完全包含在形状内。

*[贝塞尔曲线]: 由参数多项式方程定义的两个点之间的平滑曲线。一个三次贝塞尔曲线段由其两个端点P1和P2以及两个控制点C1和C2定义。曲线在P1处的切线（方向和速度）由从P1到C1的线给出。曲线在P2处的切向量由从C2到P2的线给出。一个二次贝塞尔曲线由其两个端点和一个单一的控制点C定义。每个端点处的切线是该端点与C之间的线。

*[控制点]: 不位于曲线上，但用于帮助控制曲线形状的点。例如，贝塞尔曲线段的控制点用于指定曲线在端点处的切向量（方向和速度）。

*[世界坐标]: 定义场景的坐标系统。生成的场景图像将显示位于某个视图体积（对于3D）或视图窗口（对于2D）内的世界坐标系统中的内容。对象在其自己的对象坐标系统中定义。然后应用建模变换将对象放置到场景中，即将对象坐标转换为世界坐标。

*[视窗]: 在本书中,2D图形的窗口或视图窗口是包含将在图像中显示的平面部分的xy平面中的矩形。(在3D图形中,对应的术语是"视图体积"。)

*[视口]: 用于显示2D或3D图形图像的矩形区域。视口上的坐标是像素坐标，更准确地称为设备坐标，因为它们是在显示图像的设备上的实际物理坐标。

*[建模变换]: 应用于对象以将该对象映射到世界坐标系统或更复杂的分层对象的对象坐标系统的变换。

*[对象坐标]: 对象中的点的坐标最初在其中指定的坐标系统，然后通过应用于对象的任何建模或其他变换来转换这些坐标。

*[仿射变换]: 保持平行线的变换。也就是说，当变换应用于一对平行线时，结果变换后的线也是平行的。仿射变换T具有以下特性：点(x1,y1)和点(x2,y2)之间的线段的变换是点T(x1,y1)和点T(x2,y2)之间的线段。实际上，可以通过仅变换线段的两个端点来计算线段的变换。这使得仿射变换在计算机图形中非常高效。任何仿射变换都可以表示为旋转、平移和缩放的组合。

*[均匀缩放]: 缩放变换，所有方向上的缩放因子相同。均匀缩放改变对象的大小而不改变其形状。

*[剪切变换]: 在2D中，保持某条线L不变，与L垂直的线相对于L“倾斜”相同的角度。另一种描述是，平行于L的线被映射到其自身，但是移动的距离与其与L的距离成比例。在3D中，剪切变换保持某个平面P不变，并将平行于P的平面映射到其自身，但是移动的距离与其与P的距离成比例。

*[矩阵]: 数字的矩形数组。矩阵可以表示为二维数组，数字按行和列排列。一个N×N矩阵表示从N维空间到自身的线性变换。

*[向量]: 向量空间中的元素。向量空间的元素可以相加，并且可以乘以常数。对于计算机图形，向量只是包含两个、三个或四个数字的列表或数组。在这个意义上，向量通常用于表示2D、3D或4D空间中的点。然而，准确地说，向量表示具有长度和方向的数量；以这种方式使用的向量可以被可视化为箭头。

*[线性代数]: 研究向量空间及其之间的线性变换的数学领域。线性代数是计算机图形学的基本数学基础之一。

*[线性变换]: 从一个向量空间到另一个向量空间的函数，保持向量加法和常数乘法。线性变换可以用矩阵表示。在计算机图形中，它们用于实现旋转和平移等几何操作。

*[单位变换]: 对其参数没有影响的变换。例如，在2D中，单位变换由公式I(x,y) = (x,y)给出。单位变换I具有以下属性：如果T是任何变换，则先是I再是T等同于T，先是T再是I等同于T。

*[场景图]: 一种表示场景中对象的数据结构，包括对象的属性和应用于对象的建模变换。通过遍历场景图数据结构来创建场景的图像。场景图可能只存在于概念上，也可能是程序中的实际数据结构。

*[堆栈]: 一种具有push()和pop()操作的数据结构。将项目推入堆栈只是将该项目添加到堆栈中。从堆栈中弹出将删除并返回最近推入堆栈的项目。

*[逆变换]: 给定一个变换T，其逆变换是一个将T操作反转的变换。例如，在2D变换中，如果R是T的逆变换，则R(T(x,y)) = (x,y)。缩放0.5是缩放2的逆变换。平移(-3,5)是平移(3,-5)的逆变换。并非每个变换都有逆变换。例如，按零因子缩放没有逆变换。

*[离屏画布]: 我对计算机内存中的一部分的术语，该部分可用作绘图表面，用于绘制屏幕上不可见的图像。应该存在一种方法将图像从离屏画布复制到屏幕上。例如，在Java中，可以将离屏画布实现为BufferedImage类型的对象。

*[Typed Array]: JavaScript中的一种数组类型，其限制为只能容纳单一类型的数值。例如，Float32Array类型表示可以容纳32位浮点数值的数组，而Uint8Array数组只能容纳8位整数值。这些数组在数值计算方面比一般的JavaScript数组更有效率。它们与HTML画布图形和WebGL一起引入到JavaScript中。

*[SVG]: 可缩放矢量图形。一种用于指定2D矢量图形的XML语言。SVG是一种场景描述语言。它旨在集成到网页中。

*[场景描述语言]: 一种用于通过说明图像中包含什么来指定图形图像的语言。也就是说，场景是通过声明其包含的内容来“声明性”地创建的，而不是通过程序“过程性”地创建的。使用场景描述语言编写的文档可用于为场景生成场景图。

*[关键帧动画]: 一种动画技术，在动画过程中仅明确地在某些时间点指定某个量的值。指定量的时间点称为关键帧。在关键帧之间，该量的值通过在关键帧指定的值之间进行插值来获得。

*[无符号字节]: 表示8位非负整数值的数据类型，取值范围为0到255。

*[颜色缓冲区]: 在OpenGL中，保存图像颜色数据的内存区域。它充当了绘制表面，用于渲染图像。

*[隐藏表面问题]: 在3D图形中决定每个像素点处哪个对象可见的问题。当一个对象在观察者视角后面时，只有前面的对象应该出现在图像中。3D图形的渲染算法必须满足这个约束条件。解决隐藏表面问题的算法包括绘图者算法和深度测试算法。

*[绘图者算法]: 解决隐藏表面问题的一种方法，涉及按照从远到近的顺序绘制场景中的对象，即按照从观察者距离递减的顺序。一个缺点是除非某些对象被分解成更小的子对象，否则顺序通常不是明确定义的。另一个问题是当对象移动或视角变化时，绘制顺序必须改变。

*[深度测试]: 解决隐藏表面问题的一种方法，涉及跟踪图像中每个像素点当前可见对象的深度，即与观察者的距离。当在像素点处绘制新对象时，将新对象的深度与当前对象的深度进行比较，以决定哪个对象更靠近观察者。深度测试的优点是对象可以以任何顺序渲染。缺点是图像中只能表示有限范围的深度。

*[深度缓冲区]: 存储3D图形深度测试所需信息的内存区域，即图像中每个像素点的深度值。也称为“z缓冲区”。

*[右手坐标系]: 3D空间中的坐标系，其中x、y和z轴满足以下属性：如果将右手大拇指指向正z轴方向，则手指会从正x轴向正y轴弯曲。

*[眼坐标系]: 由观察者定义的3D空间中的坐标系。在OpenGL 1.1中，眼坐标系中，观察者位于原点，朝向负z轴方向，正y轴指向上方，正x轴指向右侧。模型视图变换将对象映射到眼坐标系，投影变换将眼坐标映射到裁剪坐标。

*[世界坐标系]: 定义场景的坐标系。所产生的场景图像将显示位于某个视图体积（对于3D）或视图窗口（对于2D）内的世界坐标系中的内容。对象在其自己的对象坐标系中定义。然后，应用建模变换将对象放置到场景中；即将对象坐标转换为世界坐标。

*[眼睛坐标]: 在OpenGL 1.1中定义的三维空间上的坐标系，由观察者确定。在OpenGL 1.1中的眼睛坐标中，观察者位于原点，朝着负z轴方向看，正y轴向上，正x轴向右。建模视图变换将对象映射到眼睛坐标系，投影变换将眼睛坐标映射到裁剪坐标。

*[观察变换]: 在三维图形中，将世界坐标映射到眼睛坐标的变换。观察变换确定了观察者在世界中的位置、方向和比例。

*[模型视图变换]: 在OpenGL 1.1中，将建模变换与观察变换结合的变换。也就是说，它是从对象坐标到世界坐标的变换和从世界坐标到眼睛坐标的变换的组合。由于建模和观察变换的等价性，世界坐标对于OpenGL并不真正有意义，只有组合变换才被跟踪。

*[视口]: 2D或3D图形显示图像的矩形区域。视口上的坐标是像素坐标，更确切地称为设备坐标，因为它们是图像显示的实际物理坐标。

*[视体积]: 在OpenGL 1.1中，是在渲染图像中可见的三维空间区域。对于正交投影，视体积是一个矩形立体。对于透视投影，视体积是一个截头锥体（截断的金字塔）。

*[裁剪坐标]: OpenGL中的默认坐标系。投影变换将三维场景映射到裁剪坐标。渲染图像将显示裁剪坐标系中的立方体内容，其中x、y和z值的范围为-1到1；任何超出该范围的内容将被“裁剪”掉。

*[投影变换]: 在三维图形中，将三维空间中的场景映射到二维图像的变换。在OpenGL 1.1中，投影变换将视体积（即图像中可见的三维空间区域）映射到裁剪坐标，其中x、y和z的值范围为-1到1。然后将x和y坐标映射到图像上，而z坐标提供深度信息。

*[设备坐标]: 在显示设备或渲染图像上使用的坐标系，通常以像素作为度量单位。

*[视口变换]: 在OpenGL 1.1中，从裁剪坐标到设备坐标的最终变换。视口变换将裁剪立方体（三维中由范围为-1到1的x、y和z坐标确定的立方体）映射到视口（图像渲染的绘制表面上的矩形）。

*[透视投影]: 从三维到二维的投影，沿着从视点射出的线投影对象。透视投影试图模拟真实视图。透视投影保留透视效果；也就是说，远离视点的对象在投影中更小。在OpenGL 1.1中，透视投影的视体积是一个截头锥体。

*[正交投影]: 从三维到二维的投影，简单地丢弃z坐标。它沿着与xy平面正交（垂直）的线投影对象。在OpenGL 1.1中，正交投影的视体积是一个矩形立体。

*[相机]: 在三维计算机图形中，将投影和观察变换组合成一个抽象，模拟物理相机或眼睛。

*[多面体]: 一个闭合的三维图形，其面或侧面是多边形。通常假定多面体的面不相交，除了沿其边缘。

*[多边形网格]: 多边形的集合，其中多边形可以沿其边缘连接在一起。多边形网格可以表示一个多面体，或者可以用作曲面的近似。多边形网格可以表示为索引面集。

*[索引面集]: （IFS）。表示多面体或多边形网格的数据结构。该数据结构包括顶点的编号列表和面的列表。面由列出面的顶点的索引指定；也就是说，一个面被给定为一个数字列表，其中每个数字是顶点列表中的索引。

*[直接 nio 缓冲区]: Java 对象，属于类 java.nio.Buffer 或其子类之一。Nio 缓冲区类似于数组，但它们针对输入/输出操作进行了优化。在 Java 的 JOGL API for OpenGL 中，Nio 缓冲区用于某些目的而不是数组。

*[显示列表]: 一组图形基元和属性的列表，可以遍历以创建全部或部分图像。显示列表曾在一些早期的矢量图形硬件中使用。它们也在传统的 OpenGL 中可用。

*[顶点缓冲对象]: 顶点缓冲对象。可以容纳一组顶点的坐标或其他属性的内存块。VBO 可以存储在 GPU 上。VBO 使得可以将此类数据发送到 GPU 一次，然后多次重用。在 OpenGL 中，VBO 与函数 glDrawArrays 和 glDrawElements 一起使用。

*[长度]: 向量由其长度和方向定义，因此长度是一个基本属性。当一个向量表示为箭头时，其长度就是该箭头的长度。对于由坐标 (x,y) 给出的二维向量，长度是 x*x+y*y 的平方根。对于由 (x,y,z) 给出的三维向量，长度是 x*x+y*y+z*z 的平方根。

*[范数]: 向量长度的另一种术语。对于由 (x,y,z) 给出的三维向量，范数是 x*x+y*y+z*z 的平方根。

*[单位向量]: 长度为一的向量。

*[normalize]: 将非零向量除以其长度得到的单位向量的结果，即长度为一的向量。注意，“归一化向量”和“法向量”是两个无关的术语！

*[标量乘积]: 数字和向量的乘积。数字 s 和向量 v 的标量积是通过将 v 的每个坐标乘以 s 而获得的向量。在三维空间中，如果 s 是一个数字，v=(x,y,z)，那么 s 乘以 v 的标量积是向量 (sx,sy,sz)。

*[点积]: 两个向量的点积是对应坐标的乘积之和。对于三维向量 v=(x,y,z) 和 w=(a,b,c)，v 和 w 的点积是 x*a+y*b+z*c。点积等于两个向量之间的夹角的余弦，除以它们的长度的乘积。

*[叉积]: 两个三维向量的向量积。向量 v 和 w 的叉积是一个垂直于 v 和 w 的向量，并且其长度等于 v 和 w 之间的夹角的正弦的绝对值。如果 v=(x,y,z) 和 w=(a,b,c)，那么它们的叉积是向量 (yc-zb,za-xc,xb-ya)。

*[法向量]: 在曲面上的一个点处，法向量是垂直于该点处曲面的向量。曲线的法向量类似定义。法向量对于光照计算非常重要。

*[单位法向量]: 长度为一的法向量；即，在曲线或曲面上的给定点处垂直于曲线或曲面的单位向量。

*[单位矩阵]: n 阶单位矩阵是一个 n 阶矩阵，其主对角线上为 1，其他位置为 0。任何矩阵 B 与单位矩阵的乘积，无论顺序如何，都会保持 B 不变。将 n 维向量乘以 n 阶单位矩阵会保持向量不变；也就是说，单位矩阵是恒等变换的矩阵。

*[齐次坐标]: 一种将 n 维向量表示为 (n+1) 维向量的方法，其中两个 (n+1) 维向量表示的同一个 n 维向量，如果它们之间相差一个标量倍数。例如，在三维空间中，如果 w 不为零，则同质坐标 (x,y,z,w) 等价于同质坐标 (x/w,y/w,z/w,1)，因为它们相差标量 w 的乘法。这两组坐标都表示三维向量 (x/w,y/w,z/w)。

*[ GLUT]: OpenGL实用工具包。用于编写OpenGL应用程序的跨平台库。OpenGL本身不包含对窗口或事件的支持。GLUT添加了这样的支持。它还具有用于绘制3D形状（如球体和多面体，更不用说茶壶了）的函数。GLUT用C语言编写，并与OpenGL的C API一起使用。然而，许多GLUT函数也在JOGL中可用，它是OpenGL的Java API。一种较新且稍有改进的工具包版本名为“FreeGLUT”，通常用于取代原始版本。

*[ JOGL]: OpenGL的Java实现。JOGL非常复杂，因为它试图在一个编程系统中支持所有版本的OpenGL。JOGL与Java的Swing和AWT图形无缝集成。

*[双缓冲]: 一种图形技术，图像绘制在屏幕之外的内存区域中，称为"后备缓冲区"或"后缓冲区"。当图像绘制完成后，它可以被复制到表示屏幕内容的缓冲区，也称为"前缓冲区"。在真正的双缓冲中，图像不必被复制；相反，缓冲区可以被"交换"，使得后缓冲区成为前缓冲区，而前缓冲区成为后缓冲区。

*[单缓冲]: 与双缓冲相反，一种图形技术，图像直接绘制到屏幕上（即绘制到用作屏幕图像源的缓冲区）。单缓冲的缺点是，对于复杂的图像，用户可能会观察到图像绘制的过程。

*[线框]: 一种绘制多面体或多边形网格的样式，只绘制边缘，结果是由线段构成的图像。

*[圆环体]: 一种3D几何对象，形状类似于一个甜甜圈（或贝果）。

*[实时图形]: 用于计算机动画或其他需要快速渲染图像的应用程序的计算机图形类型。对于计算机动画，实时图形通常需要能够每秒渲染场景六十次。

*[材质]: 决定物体如何在环境中与光互动的属性。OpenGL中的材质属性包括，例如，散射颜色、镜面颜色和光泽度。

*[镜面反射]: 从表面的类似镜子的光线反射。光线以反射角等于入射角的方向反射。只有当观察者的位置在反射光线的路径上时，才能看到镜面反射。

*[散射反射]: 从表面向所有方向反射入射光，使得表面的散射照明对所有观察者都可见，与观察者的位置无关。

*[镜面高光]: 由镜面反射产生的表面照明。在表面到观察者的角度大约等于表面到光源的角度的点上，可以看到镜面高光。

*[光泽度]: 决定镜面高光大小和清晰度的材质属性。也被称为"镜面指数"，因为它在照明计算中的使用方式。在OpenGL中，光泽度是一个在0到128范围内的数字。

*[散射颜色]: 表示从表面散射反射的入射光比例的材质属性。

*[镜面颜色]: 表示由表面镜面反射的入射光比例的材质属性。

*[环境光颜色]: 表示由环境中的散射光反射的材质属性。

*[环境光]: 存在于环境中但没有特定来源的无方向光。对于已经被反射了很多次以至于无法识别原始来源的光的近似。环境光平等地照亮场景中的所有对象。

*[自发光颜色]: 表示表面固有的颜色，而不是来自其他光源反射的光的颜色。自发光颜色可以使对象看起来像是在发光，但它不会照亮其他对象。自发光颜色通常被称为"发射颜色"。

*[点光源]: 从单一点发出光线的光源。也被称为"灯"，因为灯近似于点光源。也被称为位置光。

*[方向光]: 光线平行，都来自同一方向的光源。可以被认为是来自实际无限远的光源。也被称为"太阳"，因为太阳是方向光源的一个例子。

*[强度]: 光源在不同波长上发出光。在给定波长上的光的强度是该波长光的能量量。光的总强度是其在所有波长上的总能量。光的颜色由其在所有波长上的强度决定。

*[法向量]: 表面上某点的法向量是与该点表面垂直的向量。曲线的法向量定义类似。法向量对照明计算很重要。

*[单位法向量]: 长度为一的法向量；即，垂直于曲线或表面上给定点的单位向量。

*[平面着色]: 对多边形或多边形网格的面的照明计算，使用多边形中每一点的相同法向量，使多边形呈现平坦或多面的外观。

*[平滑着色]: 对多边形或多边形网格的面的照明计算，使用多边形的每个顶点的不同法向量。当两个多边形共享一个顶点时，两个多边形都使用该顶点的相同法向量，从而在该顶点处呈现平滑的外观。当多边形网格用作平滑表面的近似时，平滑着色是适当的。

*[纹理]: 物体上某一点到另一点在某些属性上的变化。最常见的类型是图像纹理。当图像纹理应用于表面时，表面颜色会因点而异。

*[图像纹理]: 应用于表面的图像，看起来就像是“画”在表面上。

*[二的幂纹理]: 宽度和高度都是二的幂的纹理图像。在一些图形系统中，这是用作纹理图像的要求。

*[纹理坐标]: 指应用于纹理图像的二维坐标系统，或用于1D和3D纹理的类似坐标系统。纹理坐标通常在垂直和水平方向上都从0到1变化，其中(0,0)位于图像的左下角。该术语还指赋予表面的坐标，用于指定如何将纹理图像映射到表面上。

*[缩放过滤]: 在将纹理应用于对象时使用的操作，当必须缩小纹理以适应对象时。对于图像纹理，缩放过滤被应用于计算像素的颜色，当该像素覆盖图像中的几个像素时。

*[纹理像素]: 纹理图像中的像素

*[Mipmaps]: 一系列逐渐缩小尺寸的纹理图像副本，宽度和高度逐渐减小。从原始图像开始，每个mipmap通过将前一个图像的宽度和高度除以二（除非已经是1）来获得。最后的mipmap是一个单一像素。Mipmaps用于更有效地将纹理图像映射到表面上，当图像必须缩小以适应表面时。

*[纹理目标]: 在OpenGL中，有几种类型的纹理，如2D图像纹理、1D纹理和立方体贴图纹理。纹理目标由常量指定，如GL_TEXTURE_2D或GL_TEXTURE_CUBE_MAP_POSITIVE_X。纹理目标是许多OpenGL函数的参数，这些函数用于处理纹理。

*[纹理变换]: 在用于从纹理中采样数据之前应用于纹理坐标的变换。效果是平移、旋转或缩放应用到其上表面的纹理。

*[逆变换]: 给定一个变换T，T的逆变换是一个逆转T操作的变换。例如，对于2D变换，R要是T的逆变换意味着R(T(x,y)) = (x,y)。缩放0.5是缩放2的逆变换。平移(-3,5)是平移(3,-5)的逆变换。不是每个变换都有逆变换。例如，缩放因子为零就没有逆变换。

*[纹理对象]: 可能存储在显卡上的数据结构，可以保存纹理图像、一组mipmaps以及配置数据，例如当前的缩放和放大过滤器设置。使用纹理对象可以快速切换纹理，而无需重新将数据加载到显卡中。

*[three.js]: 一个用于3D图形的JavaScript库。该库实现了面向对象的场景图API。虽然它主要用于WebGL，但three.js也可以使用2D画布图形API渲染3D场景。

*[欧拉角]: 在物体自己的坐标系中表示物体的旋转，给出在该坐标系中围绕x、y和z轴的单独旋转。围绕三个坐标轴的旋转的累积效应取决于旋转应用的顺序。

*[基于物理的渲染]: PBR，基于物理的渲染。这是一个涵盖各种技术的通用术语，用于渲染材料，使其看起来比OpenGL和类似图形API中传统使用的材质更具物理真实感。这个想法是更直接地实现光和材质的实际物理。PBR已经成为实时图形（如视频游戏）中的常见做法。

*[Lambert着色]: 使用考虑环境光和漫反射的照明方程在原语上计算像素颜色的技术。在Lambert着色中，照明方程仅在原语的顶点上应用。原语中像素的颜色值是通过插值计算顶点的值来计算的。Lambert着色以约翰·兰伯特命名，他在18世纪发展了其基础理论。

*[Phong着色]: 使用考虑环境光、漫反射和镜面反射的照明方程在原语上计算像素颜色的技术。在Phong着色中，照明方程应用于每个像素。法向量仅在原语的顶点处指定。在像素中用于照明方程的法向量是通过插值顶点的法向量获得的。Phong着色以Bui Tuong Phong命名，他在20世纪70年代发展了该理论。

*[定向光]: 光线平行的光源，都来自同一方向。可以被认为是一个在无限远距离的光源。也称为“太阳”，因为太阳是定向光源的一个例子。

*[点光源]: 从一个点发射光线的光源。也称为“灯”，因为灯近似于点光源。也称为位置光。

*[环境光]: 存在于环境中但没有特定来源的定向光。这是对已经被反射了很多次以至于无法识别原始来源的光的近似。环境光平等地照亮场景中的所有物体。

*[聚光灯]: 发出光锥的光源。聚光灯类似于点光源，因为它在3D空间中有位置，光从该位置辐射出来。然而，光只影响处于聚光灯照明锥内的物体。

*[衰减]: 指点光源或聚光灯的照明随着距离光源的距离而减少的方式。从物理上讲，照明应该随着距离的平方而减少，但计算机图形学通常使用线性衰减或根本没有衰减。

*[聚光灯]: 发出光锥的光源。聚光灯类似于点光源，因为它在3D空间中有位置，光从该位置辐射出来。然而，光只影响处于聚光灯照明锥内的物体。

*[车削]: 通过围绕与曲线在同一平面内的线旋转平面曲线来产生表面的一种技术。当曲线上的每个点围绕该线旋转时，它生成一个圆。表面是由曲线上所有点生成的圆的集合。车削模仿了机械车床可以产生的形态。

*[拉伸]: 通过沿着3D中的曲线移动2D形状来制作实体的技术。实体是形状沿着曲线移动时穿过的点集。最常见的情况是将形状沿着垂直于包含形状的平面的线段移动。在实践中，计算机图形学中通过拉伸产生的物体只是拉伸实体的表面。

*[四元数]: 四元数代数中的向量，这是一个四维向量空间，其中两个向量除了可以相加外，还可以相乘。在计算机图形学中，长度为一的四元数通常用于表示旋转。一个优点是，在四元数表示中，可以在两个旋转之间平滑插值。

*[GLTF]: GL传输格式。3D模型的文件格式。GLTF文件可以包含完整的3D场景，包括对象、材质、灯光甚至动画。GLTF规范来自Khronos Group，该组织也负责OpenGL、WebGL和Vulkan。

*[阴影映射]: 一种确定场景中哪些部分被照亮，哪些部分处于阴影中的技术。该技术涉及从光源的视角渲染场景，但只使用那次渲染的深度缓冲区。深度缓冲区是“阴影映射”。沿着从光源发出的给定方向，被光照亮的物体是离光最近的物体。到该物体的距离基本上编码在深度缓冲区中。更远距离的物体处于阴影中。

*[立方体贴图]: 由六个图像组成的纹理，每个方向一个，包括正x、负x、正y、负y、正z和负z。这些图像旨在包含从给定点可以看到的所有内容。立方体贴图用于环境映射和skybox。

*[skybox]: 一个围绕场景的大立方体，用图像纹理，形成该场景所有方向的背景。

*[环境映射]: 一种模拟物体表面类似镜面反射的方法。要从表面上反射的环境被表示为立方体贴图。为了确定纹理中哪个点在物体上的给定点可见，从视点反射到表面点的射线，并且与纹理立方体相交的反射射线。环境映射也称为反射映射。

*[折射]: 光线从一种透明或半透明介质进入另一种介质时的弯曲。

*[固定功能管线]: 一个具有固定处理阶段集的图形处理管线，程序员无法修改。图像数据通过一系列处理阶段传递，最终产品是图像。这个序列被称为“管线”。在固定功能管线中，程序员可以启用和禁用阶段，并设置控制处理的选项，但无法增加功能。

*[可编程管线]: 一个图形处理管线，其中一些处理阶段可以或必须由程序实现。图像数据通过一系列处理阶段传递，最终产品是图像。这个序列被称为“管线”。可编程管线在现代GPU中使用，为程序员提供更多的灵活性和控制。可编程管线的程序称为着色器，并使用GLSL等着色器编程语言编写。

*[着色器]: 在渲染管线的某个阶段执行的程序。OpenGL着色器使用GLSL编程语言编写。对于WebGL，仅支持顶点着色器和片段着色器。WebGPU还有计算着色器，用于计算管线。

*[顶点着色器]: 一个着色器程序，将为原语中的每个顶点执行一次。顶点着色器必须计算裁剪坐标系中的顶点坐标。它还可以计算其他属性，如颜色。

*[片段着色器]: 一个着色器程序，将为原语中的每个像素执行一次。片段着色器必须为像素计算颜色，或者丢弃它。片段着色器也称为像素着色器。

*[属性变量]: 表示可编程图形管线中顶点着色器的输入的变量。属性变量在原语中的每个顶点上可以有不同的值。

*[统一变量]: 表示可编程图形管线中着色器程序的输入的变量。统一变量在每个顶点和每个像素上都有相同的值。

*[变化变量]: 在WebGL或OpenGL ES 2.0图形管线中用于在顶点着色器和片段着色器之间通信值的变量。变化变量在顶点着色器中被赋值。原语中像素的片段着色器中变量的值是通过插值原语顶点的值来获得的。（在支持其他着色器阶段的较新版本的GLSL中，“变化变量”一词被更通用的“输入变量”和“输出变量”所取代，这些变量用于着色器的输入或输出。）

*[顶点数组对象]: 在WebGL 2.0中，顶点数组对象（VAO）是通常位于显卡上的一块内存区域，它保存了一系列属性设置，如启用状态和顶点属性指针的值。然后，所有设置都可以通过绑定VAO来选择。

*[实例化绘制]: 用单个函数调用来渲染多个版本的原语的能力。每个副本可以有自己的某些属性值，如颜色或变换。

*[Swizzling]: 在GLSL和WGSL中，一种表示法，如v.yzx，其中v是向量，v.yzx表示由v的y、z和x分量组成的三分量向量。技术上，任何使用点表示法的向量都被认为是swizzler。

*[列主序]: 二维矩阵元素的列主序排列；即，从第一列的元素开始，然后是第二列的元素，依此类推。OpenGL和GLSL中的矩阵使用列主序。

*[存储限定符]: 在GLSL中，变量声明的以下修饰符之一：uniform（统一）、attribute（属性）、varying（变化）或const（常量）。

*[精度限定符]: 在GLSL中，数值变量声明的以下修饰符之一：lowp（低精度）、mediump（中等精度）或highp（高精度）。精度修饰符指定变量的最小位数或值的范围。

*[不变量]: 在GLSL中，一个修饰符，确保当相同的表达式用于在两个不同的着色器中计算变量的值时，两个着色器中的值将是相同的。这对于多次通过算法很重要，在这种算法中，多个着色器程序连续应用于渲染一个图像。

*[多次通过算法]: 一种渲染算法，它多次绘制场景，以某种方式组合结果以计算最终图像。一个简单的例子是红蓝立体图像，其中场景的左眼和右眼图像分别渲染并组合。

*[纹理单元]: GPU中的一个硬件组件，用于进行纹理查找。（也可以指代这样一个组件的抽象，无论它是否实际在硬件中实现。）也就是说，它将纹理坐标映射到图像纹理的颜色上。这个操作被称为“采样”，纹理单元与GLSL着色器程序中的采样器变量相关联。

*[TMU]: 纹理映射单元，纹理单元的另一个名称（可能更强调实际的硬件支持）。也称为TPU（纹理处理单元）。

*[采样]: 将纹理坐标映射到纹理的颜色上的操作，包括如果可用则使用mipmap，并且在必要时应用缩放或放大滤波器。

*[采样器变量]: 在GLSL中，着色器程序中的一个变量，可以用来在图像纹理中进行查找。采样器变量的值指定了将用于进行查找的纹理单元。在WebGL中，采样器变量的类型为“sampler2D”或“samplerCube”。

*[WebGPU]: 一种新的JavaScript图形API，类似于WebGL，但设计上允许Web程序访问现代GPU功能，如计算着色器。

*[glMatrix]: 一个用于二维和三维向量和矩阵数学的开源JavaScript库。

*[逐顶点光照]: 仅在原语的顶点处进行光照计算，并通过插值结果来获取内部像素的颜色。逐顶点光照是传统OpenGL的标准。没有镜面反射的逐顶点光照是Lambert着色。

*[逐像素光照]: 在原语的每个像素上进行光照计算，这在大多数情况下比逐顶点光照得到更好的结果。Phong着色使用逐像素光照，法线向量由顶点插值得到。

*[过程纹理]: 在给定的纹理坐标集合上，其值作为纹理坐标的数学函数来计算的纹理，与通过采样图像获得值的图像纹理相对。

*[Perlin噪声]: Ken Perlin在1983年发明的一种技术，用于计算看起来自然的程序纹理。Perlin噪声函数有数值输入（通常是2或3），并产生一个介于-1.0到1.0范围内的输出数字。输出是伪随机的，但具有一定的规律性，具有大小相似、分布均匀的特征，并且在多个尺度上都有变化。

*[凹凸映射]: 使用纹理来修改表面上的法线向量，以在不实际修改表面几何体的情况下给出高度变化的外观。

*[帧缓冲区]: 在WebGL中，一个组织渲染图像缓冲区的数据结构，可能包括颜色缓冲区、深度缓冲区和模板缓冲区。WebGL图形上下文有一个用于屏幕渲染的默认帧缓冲区，并且可以为离屏渲染创建额外的帧缓冲区。

*[深度掩码]: 在WebGL中，一个设置，控制是否在渲染期间将深度值写入深度缓冲区。当深度掩码设置为false时，深度值将被丢弃，深度缓冲区保持不变。

*[颜色掩码]: 在WebGL中，一种设置，用于确定在渲染期间颜色缓冲区的哪些“通道”被写入。这些通道是颜色的RGBA组成部分：红色、绿色、蓝色和alpha。颜色掩码由四个布尔值组成，每个通道一个。一个false值会阻止对颜色缓冲区中相应颜色分量的任何更改。

*[多遍算法]: 一种渲染算法，它多次绘制场景，并以某种方式组合结果来计算最终图像。一个简单的例子是红蓝立体图像，其中场景的左眼和右眼图像分别被渲染并组合。

*[渲染到纹理]: 一种技术，将渲染操作的输出直接写入纹理。在WebGL中，通过将纹理附加为帧缓冲区的缓冲区之一，可以实现渲染到纹理。

*[渲染缓冲区]: 在WebGL中，一种缓冲区（即内存区域），可以附加到帧缓冲区用作颜色缓冲区、深度缓冲区或模板缓冲区。

*[WebGL扩展]: WebGL中的一个可选功能，在所有实现中都不可用。WebGL API有一个函数用于检查给定的扩展是否可用，如果是，则激活它。

*[各向异性过滤]: 一种更准确地采样纹理图像的技术，在正在纹理化的表面上的一个像素对应于纹理中的非矩形区域的情况下使用。在WebGL中，各向异性过滤作为可选扩展提供。

*[延迟着色]: 一种多遍渲染技术，其中第一个遍历处理几何体并保存相关数据，例如变换后的坐标、法线向量和材质属性。这些数据可以存储在纹理中，在这种情况下被称为“几何缓冲区”或“G缓冲区”。然后，可以在额外的遍历中使用预计算的几何缓冲区中的信息来计算光照和其他效果，而不是为每个遍历重新计算。

*[光线投射]: 从给定点开始，沿着给定方向追踪射线（即无限线的一半），以找到射线与场景中物体的交点的过程。通常，只有离射线起始点最近的交点才是感兴趣的。

*[阴影射线]: 在光线追踪算法中，从物体上的点向光源方向投射的射线，以确定该点是否被该光源照亮或是处于阴影中。

*[重心坐标]: 在三角形上的坐标系统，其中点被表示为三角形顶点的线性组合，即 a*A + b*B + c*C，其中 A、B 和 C 是顶点，a、b 和 c 是数字。三角形中的任何点都可以用这种形式表示，其中系数 a、b 和 c 的值在 0 到 1 范围内，且 a + b + c 等于 1。

*[光线追踪]: 一种递归渲染算法，使用光线投射。从视点通过图像中的点投射射线进入场景，以确定该点所看到的景象。为了确定在该点所看到的颜色，会从该点投射更多的射线，包括反射射线（如果物体具有镜面反射）、折射射线（如果物体是半透明的）以及向光源的阴影射线（以确定物体是否被该光源照亮）。为反射或折射射线找到颜色可以使用递归应用光线追踪算法。

*[折射率]: 光的传播介质（如空气或玻璃）的属性，其传播光。当光线从一种介质穿过另一种介质时，其折射或弯曲取决于两种介质的折射率比值。介质的折射率取决于光在该介质中的速度。

*[环境光遮蔽]: 一种渲染技术，考虑到环境光会根据不同程度地被场景中的其他几何体阻挡或“遮蔽”，从而不同程度地照亮不同的表面。环境光遮蔽是对基本环境照明的改进，但就像环境光本身一样，它不是一个实际的物理现象。

*[全局照明]: 3D 渲染算法的目标，考虑到场景中光线的所有相互作用，包括通过从其他物体上反射的间接照明。

*[路径追踪]: 一种基于计算所有可能的光到达观察者位置的路径的渲染算法。从每个方向来看，这实际上是不可能完成的，因此该算法追踪路径的一个随机样本，并平均结果。随着样本数量的增加，平均值会收敛到一个非常高质量的图像。

*[双向散射分布函数(BSDF)]: 在3D图形中“材质”概念的一种概括。双向散射分布函数给出了从某个方向到达空间某点的光线射线将以另一个方向离开该点的概率。这个概率是两个方向、点和光的波长的函数。其中一种散射是光从表面的反射。在这种情况下，使用双向反射分布函数(BRDF)这个术语。

*[次表面散射]: 一种光照效果，光线进入一个稍微半透明的物体，在其内部反射一次或多次，然后从物体的不同点退出。次表面散射有助于诸如玉石、牛奶和皮肤等材料的外观表现。

*[WebGPU]: 一种新的 JavaScript 图形 API，类似于 WebGL，但设计用于让网络程序访问现代 GPU 功能，如计算着色器。

*[WGSL]: WebGPU 着色器语言，是编写 WebGPU 使用的着色器的编程语言。

*[顶点缓冲区]: 在 WebGPU 中，顶点缓冲区是一种 GPU 数据结构，用于保存作为顶点着色器输入的值。

*[绑定组]: 一种数据结构，可以保存缓冲区、纹理和样本等资源，作为输入进入管线。

*[索引缓冲区]: 在 WebGPU 中，索引缓冲区是一种 GPU 缓冲区，用于保存与 drawIndexed() 一起使用的顶点索引。顶点索引给出了原语顶点列表中顶点的位置。

*[存储缓冲区]: 在 WebGPU 中，一种通用目的的 GPU 缓冲区，可以在计算着色器以及顶点和片段着色器中使用。

*[对齐]: 根据数据类型，内存中值的合法位置的限制。例如，在 WGSL 中，vec3f 变量的地址必须是 16 的倍数。

*[WGSL]: WebGPU 着色器语言，是编写 WebGPU 使用的着色器的编程语言。

*[归一化设备坐标]: 一种表示 n 维向量为 (n+1) 维向量的方法，其中两个 (n+1) 向量如果它们相差一个标量倍数，则表示相同的 n 维向量。例如，在 3D 中，如果 w 不为零，那么齐次坐标 (x,y,z,w) 与齐次坐标 (x/w,y/w,z/w,1) 等价，因为它们相差 w 的标量乘法。这两组坐标都表示 3D 向量 (x/w,y/w,z/w)。

*[采样]: 将纹理坐标映射到纹理中的颜色的操作，包括如果可用则使用 mipmap，并在必要时应用缩小或放大滤波器。

*[计算着色器]: GPU 管线中的一个阶段，它只进行纯粹的计算工作，而不是直接参与图形渲染。

*[Eclipse]: 一个用于编写 Java（和其他编程语言）程序的集成开发环境。Eclipse 是一个可以从 http://eclipse.org 下载的免费程序。

*[ES6]: 几乎所有现代网络浏览器实现的 JavaScript 版本。更正式地称为 ECMAScript 6 或 ECMAScript 2015。ES6 引入了大量的新特性。

*[promises]: 在 JavaScript 编程中，一个承诺代表一个可能立即可用或将来某个时候可用的结果。程序员可以提供一个函数，如果承诺实现（即结果可用时）或承诺被拒绝（例如，如果发生某些错误）时被调用。承诺是异步的，因为处理成功或失败的函数将在某个不可预测的时间被调用。

*[async functions]: 在 JavaScript 中，异步函数是可以使用 "await" 语句等待承诺结果的函数。当执行 await 语句时，异步函数的执行将暂停，直到承诺被实现或被拒绝，同时让其他 JavaScript 代码有机会在此期间运行。
