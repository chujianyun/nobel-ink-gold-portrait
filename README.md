# 诺贝尔黑墨金赭手绘肖像

把人物照片转换成诺贝尔获奖者头像参考中的手绘画风：暖白纸纹、黑色干笔墨线、局部金赭色阴影，以及大面积留白。

这是一个可安装的 Agent Skill。它提供风格规范、转换提示词和 8 张风格参考；出图时保留新照片中的人物长相、年龄、眼镜、表情和姿势。

## 效果展示

下面展示原照片的墨镜版本与实际转绘结果。转绘时保留了人物的微笑、抱臂姿势和手表。

<table>
  <tr>
    <th>原始照片（墨镜展示版）</th>
    <th>黑墨金赭手绘肖像</th>
  </tr>
  <tr>
    <td align="center"><img src="assets/examples/portrait-original.jpg" width="320" alt="将透明眼镜替换为墨镜的原始人物照片展示版"></td>
    <td align="center"><img src="assets/examples/portrait-ink-gold.png" width="320" alt="保留人物身份与姿势的黑墨金赭手绘效果"></td>
  </tr>
</table>

也可以按头像上传要求调整为 **1:1 方图**。下面这个示例为 **1254 × 1254 像素，PNG 格式，约 2.24 MB**，保留完整人物并扩展两侧纸纹背景。

<img src="assets/examples/portrait-square.png" width="400" alt="1:1 方形黑墨金赭肖像示例">

## 安装

需要 Git，以及支持读取本地 Skills 的 Agent。出图还需要环境提供图像编辑工具，优先使用内置 imagegen；仅安装本技能不会自动安装或配置图片模型。

克隆仓库，并将其中的技能文件放入 `~/.agents/skills/nobel-ink-gold-portrait/`：

```bash
git clone https://github.com/chujianyun/nobel-ink-gold-portrait.git
mkdir -p ~/.agents/skills/nobel-ink-gold-portrait
cp nobel-ink-gold-portrait/SKILL.md ~/.agents/skills/nobel-ink-gold-portrait/
cp -R nobel-ink-gold-portrait/agents nobel-ink-gold-portrait/references nobel-ink-gold-portrait/assets ~/.agents/skills/nobel-ink-gold-portrait/
```

以上命令适用于首次安装。已有同名技能时，先检查并备份本地修改，再更新。安装后如当前会话未发现技能，开启新会话加载。

## 使用

上传一张清晰的人物照片，然后输入：

```text
使用 $nobel-ink-gold-portrait，将这张照片转换为黑墨金赭手绘肖像。
保留人物长相、眼镜、表情和姿势。
```

其他常用请求：

```text
按诺贝尔获奖者头像的画风重绘这张照片。
```

```text
生成 1:1 方图，PNG 格式，5 MB 以内，保留完整人物。
```

```text
只给我这套画风的转换提示词，不出图。
```

默认使用 2:3 竖幅，也支持明确指定方图、其他画幅或裁切。新照片负责人物身份，风格参考负责画法；不会把参考人物的长相或年龄套到新照片中。效果由生成模型和原照片共同决定，不保证每次完全一致。

## 风格要点

- **纸底**：微暖白色，细微纤维纹理，背景留空。
- **墨线**：粗细变化，头发带干笔、飞白与刷痕。
- **金赭**：选择性地表现脸侧、眼下、鼻侧、下颌和颈部阴影，呈哑光颜料感。
- **留白**：脸部大面积保留纸白，衣服以少量轮廓线概括。
- **人物**：形体写实、笔法简练，保留五官比例和识别特征。

完整执行说明见 [SKILL.md](SKILL.md)，详细画法见 [视觉规范](references/visual-style.md)。

## 作者

**悟鸣**

- 浙江省人工智能专家服务团专家
- 杭州市人工智能学会入口专家
- 千问办公大使
- Qoder 企业培训大使

## 联系方式

关注公众号，或扫码添加微信交流。

<table>
  <tr>
    <th>公众号</th>
    <th>微信</th>
  </tr>
  <tr>
    <td align="center"><img src="assets/contact/official-account-qr.jpg" width="220" alt="公众号二维码"></td>
    <td align="center"><img src="assets/contact/wechat-qr.png" width="220" alt="微信联系二维码"></td>
  </tr>
</table>
