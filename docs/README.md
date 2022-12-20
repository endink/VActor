# VActor 

基于 Google Mediapipe , UnrealEngine 的动补、面补软件   


![screen](./images/screen_snapshot.jpg "screen")

> 本软件基于 UnrealEngine 插件 **[MediaPipe4U](https://github.com/endink/Mediapipe4u-plugin)** 制作。
---

**下载地址**

[奶牛快传 (2022-12-20)](https://cowtransfer.com/s/bab20c9d383c44)   
[OneDrive (2022-12-20)](https://1drv.ms/u/s!AkmROUeQfSBjzWm3q8idvIJpk5KM?e=MiDGkE)


**功能**

- VRM 模型加载
- RGB摄像头实时动补
- RGB摄像头实时面补（实验性）
- Arkit面补支持
- 虚拟摄像头
- 预制灯光效果
- 动画数据导出（BVH 格式）
- 自定义渲染效果

**视频介绍合集：**

[B站](https://space.bilibili.com/481665211/channel/collectiondetail?sid=810148)

---   
**特别感谢**

感谢 **[Noesis GUI](https://www.noesisengine.com/)** 为本软件提供了个人免费授权。

---   
**Third Party License**

The software contain components from Google MediaPipe, VRM4U, CryptoPP, NoesisGUI, GStreamer (dynamic link). These components are governed by separate agreements and their respective product support policies, but if separate license terms for these components are included directly in the installation directory, those license terms shall control.

## 更新日志
## 12月20日
-[new]半身模式加入头部算解器，头部旋转使用 face mesh 计算
-[improve]改善肘部过度扭曲问题（限制旋转）
-[improve]脊柱链式旋转（优化旋转效果）

### 12月09日
- [new]半身动补时支持手放时手腕、手指自动回到初始姿态
- [new]半身动补脊柱二次平滑（曲线插值），可以在弱光环境消除身体抖动
- [fix]手腕扭曲校正开启后，手腕计算错误
- [fix]渲染参数重置到默认值界面没刷新
- [fix]位移计算侧身时深度错误
- [fix]半身动补和全身动补切换时，可能加载错误的配置参数
- [improve]没有开启虚拟摄像头时渲染性能提升30%，大幅度提升 FPS
- [improve]VRM强制开启材质双面（two side）渲染，防止不规范的模型衣服出现漏光
- [improve]VRM记载Loading界面
- [improve]VRM文件加载出错提示
- [improve]优化位移计算方法，位移计算更加准确
- [improve]脚踝计算改进，加入角度约束，防止脚踝过度翻转
- [improve]微调 Lumen 设置，提高渲染效果

### 12月09日
- [fix]修复纹理流送 BUG（不确定这是不是一个 BUG，见 #5）
- [fix]脊柱锁定设置不生效 BUG
- [new]位移标定计时板显示
- [new]位移锁定（可以控制是否计算/垂直/水平/前后位移）
- [new]渲染效果控制（实验性：shader 参数调整，支持动态切换 lit,sss,unlit 等效果）

### 12月06日

- [new]BVH 动画数据导出支持
- [new]视频动补时间进度条拖动支持

