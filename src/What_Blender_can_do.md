# Blender可以做什么 {#firstHeading}

Blender是一套完整的集成了3D内容创作的套件，全面提供了必要的创作工具包括 建模, 渲染, 动画, 视频编辑, 特效后期, 合成, 制作贴图, 骨骼蒙皮, 多种多样的 物理模拟, 以及 游戏制作 。

尽管多数Blender制作出的最终产品都是平面上的2D位图，这些图像还是被称为“3D”，因为它们都有着深度错觉，看到图片的人能轻松看出哪部分更近，哪部分更远。

**示例**

这里有个现成的用Blender创建的图片。

![&quot;A Lonely House&quot;,Mayqel制作](./images/400px-Lone_House.jpg)![](/images/400px-Lone_House.jpg)

仔细观察图中的建筑。

* 因为它挡住了绿树成荫的山坡，你可以看出山坡在建筑物之后，而非相反。
* 另外，正面墙壁的上下边沿，在靠近树的一边似乎靠得更拢，你能据此判断出墙与你的视角间的角度。
* 你的意识会将墙较暗的部分当作是阴影，让你估计出光线从哪边照来，尽管太阳在画面之外。

尽管2D绘图软件（或者画笔）也能手动的做出深度错觉，但Blender提供了一个容易得多的方法。

或许这座孤独的房子从来只存在于艺术家的想像之中。不需要在德国的乡村建一座，等待正确的光照，然后拍照，只要在虚拟的3D世界（在一台电脑里）中创建一个场景，然后他或她就能用Blender渲染这个场景（把它转成2D图片）。

**建模的步骤**

在3D计算机图像中，模型是一个可用于渲染的物体或场景的抽像版本。而建模则是制作模型的过程。

要创建“A Lonely House”的3D场景大约需要以下几步：

* **物体建模**（描述物体的形状，如鸟、树，在三维空间中）
* **上色shading**（设定每个物体的颜色、贴图的模式）
* **设定灯光lighting**（描述光源的强度、颜色、方向等）
* **Modelling,**which is the creation of your miniature 3D world, also known as a **model** or **scene** This involves defining the geometry of the objects, 使它看起来像他们是用特殊材料制作的, 设置灯光和定义摄像头视口
* **Rendering,**which is the actual generation of the image of the world from the viewpoint of the camera \(taking a “photograph” of the scene, if you like\), for your audience to enjoy.

如果“A Lonely House”要做成一段视频，还另外需要几步来完成场景的animating（描述它如何随时间改变）：

* **绑定\(Rigging\)**（描述生物的一部分——如鸟的翅膀——如何相对其他部分移动）
* **布景\(Posing\)**（编排物体和他们的部分在不同时间中于3D场景里所处的位置）

Blender能很好的胜任以上所有步骤。

* **Rigging**— setting up a rig, namely a way of deforming \(changing the shape of\) a character in various repeatable ways to convincingly mimic joint movements, facial expressions and other such actions of real-life people or animals.

* **Posing **— choreographing the positions of the objects and their parts in the 3D scene over time, using the previously-created animation rigs
* Rendering now involves creating a whole sequence of frames representing movement over time, rather than just a single still frame.

But that’s not all. There are frequently additional processes to embellish the results of the above, to make them look more realistic:

* Sculpting
  — a more organic form of modelling objects by shaping them as though they were made out of clay. This produces more complicated, irregular shapes which mimic real objects found in nature, as opposed to clean, simple, geometrical ones which mostly only exist in the world of mathematics.
* Texture painting
  — You’re probably familiar with programs that let you paint an image on a 2D digital canvas. Such programs are commonly used in 3D production, to create
  textures
  which are “wrapped” around the surfaces of 3D objects to give them a more interesting appearance. 3D programs also often allow direct painting on the surfaces of those objects, so the effect of the design can be observed immediately, instead of having to go through a separate paint-on-a-flat-surface-then-wrap sequence of steps.
* Physical modelling
  — simulating the behaviour of real-world objects subject to real-world forces, for example hard balls colliding, soft cloth draping itself over an obstacle under gravity, water flowing and pouring. Mathematical formulas are available for these that give results very close to real life, all you need is the computing power to calculate them.
* Motion capture
  , or
  mocap
  : producing convincing animations, particularly ones that look like the movements of real people \(walking, running, dancing etc\) can be hard. Hence the technique of capturing the motions of live actors, by filming them with special markers attached to strategic points on their bodies, and doing computer processing to track the movements of these markers and convert them to corresponding movements of an animation rig.
* Compositing
  — this is where 3D renders are merged together with real photographic/live-action footage, to make it look like a rendered model is in the middle of a real-world scene, or conversely a real live actor is in the middle of a rendered scene. If done with proper skill, in particular due care to matching the effects of lights and shadows, the viewer becomes unable to tell what is real and what is not!

And just to add another complication to the mix, there are two kinds of rendering:

* Real-time
  rendering is rendering that has to happen under tight time constraints, typically for interactive applications like video gaming. For example, most gamers nowadays consider that the screen has to be updated 60 times per second in order to render smooth motion and respond quickly enough to player actions. These time constraints impose major limitations on the kinds of rendering techniques that can be used.
* Non-real-time rendering is where the time constraints are not so tight, and quality is the overriding factor. For example, when producing a single still frame, it may not matter so much that it takes minutes or hours to do so, because the beauty and detail of the final image is worth it. When rendering a Hollywood-quality movie, it may still take hours per frame, but the use of a
  renderfarm
  of hundreds or thousands of machines, all working on different frames at the same time, allows the entire sequence to complete in just a few weeks.

**But wait, there’s more:**There are also some areas, which might be considered to be stepping outside of traditional 3D production work, where Blender provides functionality:

* **Video editing**
  — having rendered your animation sequences and shot your live-action footage, you will want to combine them in a properly-timed linear sequence to tell a coherent story.
* [**3D printing**](https://en.wikipedia.org/wiki/3d_printing)
  — Though still in its early days yet, many people are already experimenting with creating objects using 3D printers. The shape data may be obtained from real objects with 3D scanning, or it may be created from scratch using 3D modelling, or you can even combine both processes.

Blender is a capable tool for every single one of these processes. There’s quite a lot there, isn’t there? But don’t be too intimidated: this Wikibook will take things step by step, and you will be able to produce some fun stuff from early on.

