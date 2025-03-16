# L_BlenderPlugin_1

本插件基于 blender 4.27 LTS 版本编写。

脚本需求文档如下：

1. 先清空场景
2. 添加灯光和若干物体到场景中（内置的任何网络物体），并使物体随机移动，形成动画
3. 添加若干个摄像头，比如4个。用这4个摄像头从不同角度同时渲染输出
4. 为摄像机添加移动旋转。随机/固定路线移动不限，须包含平移和旋转
5. 输出内容须包括
    - RGB通道
    - ID通道
    - 像素和摄像机平面的垂直距离
    - 像素和摄像机的距离

6. 输出为exr格式，分辨率1920x1080或更小
7. 渲染引擎用EEVEE和CYCLES，支持两种引擎全局开关切换
8. 实现插件GUI
