# 转换提示词模板

填写图片职责和用户要求后使用；模板中的方括号是运行时变量，不是需要原样输出的文本。

```text
将内容图中的人物重绘为风格参考图中的黑墨金赭手绘肖像。

图片职责：
- 内容图：[明确目标照片的文件名或附件位置]。只依据它保留人物身份、脸型、五官比例、眼距、鼻形、嘴形、发型、年龄、表情、姿态、眼镜与服装。
- 风格图：[明确所选参考文件或附件位置]。仅提取墨线、纸纹、金赭阴影、留白和构图，不迁移其中人物的长相、年龄、性别或配饰。

构图：[用户要求；默认 2:3 竖幅、居中的单人头肩至胸部肖像]。保持人物自然的视线和转头角度，头顶少量留空。暖白细纹纸铺满画面，背景干净无场景。

用粗细变化的黑色手绘墨线勾画脸缘、五官、耳廓、眼镜和衣领，线条有自然停顿、断线与刷毛边缘。头发用顺着发型走势的成束弧形干笔表现，黑色墨块与露出纸底的飞白交替；眉毛及胡须用疏密变化的短笔触表现。

脸部以纸白为主，用少量哑光暖金赭色笔触表现太阳穴、脸侧、眼下、鼻侧、唇部、下巴和颈部的结构阴影。下颌及颈部可用较大的不规则色块；额头中心、鼻梁和双颊中心保持大面积纸白。金色有轻微颗粒和刷痕，不反射金属高光。默认小面积金赭虹膜、黑色瞳孔、纸白眼白，保持源人物眼形与目光。[如用户要求原眼色，在此替换对应规则。]

衣服保留原类别与领口，以少量黑色轮廓、翻领和必要褶线概括，大面积未着色，往画面下方简化并自然收笔。人物形体写实，笔法克制而手工化。

避免全脸染黄、彩色肤色、柔光渐变、摄影质感、3D、金属雕像、卡通大眼、等宽矢量线、满脸排线、杂乱背景、文字、边框、水印和签名。不添加源照片没有的眼镜或胡须，不改变年龄，不自动换西装。

优先级：人物身份准确，其次匹配参考图的黑墨笔法、金赭阴影与留白关系，最后匹配构图与纸纹。
其他用户要求：[仅填写已明确的要求，删除空项]。
```

必要时添加的英文画法锚点：

```text
Hand-rendered editorial portrait on warm off-white, subtly fibrous paper. Expressive black ink contours with varied pressure, dry-brush breaks and bristle texture. Directional brush ribbons in the hair, alternating dense black strokes and exposed paper. Selective matte ochre-gold pigment shapes define facial and neck shadows; most facial planes remain untouched paper. Sparse clothing contours, broad unpainted areas, realistic likeness and economical hand-drawn marks. No metallic shine, smooth digital gradients, vector-clean outlines, all-over yellow tint, copied signature or reference-person identity blending.
```
