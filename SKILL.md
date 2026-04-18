---
name: wechat-layout
description: 微信公众号专业排版规范。提供信息分层设计、3色原则、内联样式模板，确保手机端阅读体验。适用于所有公众号内容创作场景。
version: 1.0.0
author: Jarrett
license: MIT
---

# 微信公众号专业排版 Skill

> 基于信息分层设计的公众号排版规范，让你的文章在手机端拥有专业级阅读体验。

## 核心原则

### 1. 信息分层设计

通过不同的视觉符号，帮读者快速区分"标题 / 章节 / 重点 / 正文 / 行动项"，哪怕在白底模式下，也能一眼抓住节奏。

### 2. 3色原则

- **正文**：#333333（深灰，护眼不刺眼）
- **主色**：#00a3a4（青色，用于强调和标题）
- **注释**：#999999（浅灰，用于辅助信息）

全文颜色不超过3种，拒绝花哨。

### 3. 手机优先

所有尺寸和间距都针对手机端优化，确保在小屏幕上的可读性。

## 排版规范

### 字体参数

```
正文：15px、#333333、行高1.75、字间距0.5px
段落间距：15px
标题：18px、#1a1a1a、加粗、左侧4px青色竖线
```

### 3种高亮方式

#### 1. 浅黄背景块（核心观点/金句）

```html
<section style="background: #fffbf0; padding: 15px; margin: 15px 0; border-radius: 6px;">
<p style="margin: 0; color: #1a1a1a; font-size: 15px; line-height: 1.75; font-weight: 600;">核心观点文字</p>
</section>
```

**适用场景**：文章中最重要的结论、金句、核心观点

#### 2. 浅青色块+左侧竖线（对比句/关键结论）

```html
<section style="background: #f0fafa; padding: 15px; margin: 15px 0; border-radius: 6px; border-left: 3px solid #00a3a4;">
<p style="margin: 0; color: #00a3a4; font-size: 15px; line-height: 1.75; font-weight: 600;">关键结论文字</p>
</section>
```

**适用场景**：对比性观点、关键结论、重要提示

#### 3. 浅蓝圆角块（结尾总结，居中）

```html
<section style="background: #f0f5ff; padding: 15px; margin: 20px 0; border-radius: 8px; text-align: center;">
<p style="margin: 0; color: #1a1a1a; font-size: 15px; line-height: 1.75; font-weight: 600;">总结文字</p>
</section>
```

**适用场景**：文章结尾总结、互动问句、行动号召

### 标题样式

```html
<h2 style="font-size: 18px; color: #1a1a1a; margin: 30px 0 15px; font-weight: 700; padding-left: 12px; border-left: 4px solid #00a3a4;">章节标题</h2>
```

**特点**：左侧青色竖线，视觉层次清晰

### 正文段落

```html
<p style="margin: 0 0 15px 0; color: #333333; font-size: 15px; line-height: 1.75;">正文内容</p>
```

### 关键词强调

```html
<strong style="color: #00a3a4; font-weight: 600;">关键词</strong>
```

### 列表样式

```html
<p style="margin: 0 0 8px 0; color: #333333; font-size: 15px; line-height: 1.75; padding-left: 20px;">
<span style="color: #00a3a4; font-weight: bold;">●</span> 列表项内容
</p>
```

**特点**：青色圆点，左侧缩进20px，项间距8px

### 分割线

```html
<p style="border-top: 1px solid #e8e8e8; margin: 30px 0;"></p>
```

**特点**：细线条，上下留白30px

### 图片

```html
<img src="图片URL" style="width: 100%; border-radius: 4px; display: block; margin: 15px 0;">
```

**特点**：100%宽度自适应，圆角4px，上下间距15px

### URL 链接

```html
<code style="background: #f5f5f5; padding: 2px 6px; border-radius: 3px; font-size: 14px; color: #00a3a4;">https://github.com/xxx/xxx</code>
```

**特点**：
- 使用 `<code>` 标签包裹，防止被微信自动分词
- 浅灰背景 #f5f5f5，区分普通文本
- 圆角 3px，内边距 2px 6px
- 青色主题色 #00a3a4，保持视觉统一
- 字号 14px，略小于正文

**⚠️ 重要**：不要用 `<span>` 或 `white-space: nowrap`，会导致字符间空格更明显

### 结尾固定格式

```html
<section style="text-align: center; color: #999999; font-size: 14px; margin-top: 40px; padding-top: 20px; border-top: 1px solid #e8e8e8;">
<p style="margin: 0;">今天的分享就到此结束，咱们下回见；<br>如果觉得文章对你有帮助，记得点赞、转发、收藏喔 👋</p>
</section>
```

## 完整示例

```html
<p style="margin: 0 0 15px 0; color: #333333; font-size: 15px; line-height: 1.75;">这是一段正文，介绍文章的背景和引入话题。</p>

<section style="background: #fffbf0; padding: 15px; margin: 15px 0; border-radius: 6px;">
<p style="margin: 0; color: #1a1a1a; font-size: 15px; line-height: 1.75; font-weight: 600;">这是核心观点，用浅黄背景块突出显示。</p>
</section>

<p style="border-top: 1px solid #e8e8e8; margin: 30px 0;"></p>

<h2 style="font-size: 18px; color: #1a1a1a; margin: 30px 0 15px; font-weight: 700; padding-left: 12px; border-left: 4px solid #00a3a4;">第一个章节</h2>

<p style="margin: 0 0 15px 0; color: #333333; font-size: 15px; line-height: 1.75;">这是章节下的正文内容，可以包含<strong style="color: #00a3a4; font-weight: 600;">关键词强调</strong>。</p>

<p style="margin: 0 0 8px 0; color: #333333; font-size: 15px; line-height: 1.75; padding-left: 20px;">
<span style="color: #00a3a4; font-weight: bold;">●</span> 列表项1
</p>
<p style="margin: 0 0 8px 0; color: #333333; font-size: 15px; line-height: 1.75; padding-left: 20px;">
<span style="color: #00a3a4; font-weight: bold;">●</span> 列表项2
</p>

<section style="background: #f0fafa; padding: 15px; margin: 15px 0; border-radius: 6px; border-left: 3px solid #00a3a4;">
<p style="margin: 0; color: #00a3a4; font-size: 15px; line-height: 1.75; font-weight: 600;">这是关键结论，用浅青色块+左侧竖线强调。</p>
</section>

<img src="https://example.com/image.jpg" style="width: 100%; border-radius: 4px; display: block; margin: 15px 0;">

<section style="background: #f0f5ff; padding: 15px; margin: 20px 0; border-radius: 8px; text-align: center;">
<p style="margin: 0; color: #1a1a1a; font-size: 15px; line-height: 1.75; font-weight: 600;">这是结尾总结，用浅蓝圆角块居中显示。</p>
</section>

<section style="text-align: center; color: #999999; font-size: 14px; margin-top: 40px; padding-top: 20px; border-top: 1px solid #e8e8e8;">
<p style="margin: 0;">今天的分享就到此结束，咱们下回见；<br>如果觉得文章对你有帮助，记得点赞、转发、收藏喔 👋</p>
</section>
```

## 重要提醒

### ⚠️ 必须使用内联样式

微信公众号不支持 `<style>` 标签，所有样式必须写在标签的 `style` 属性里。

### ✅ 避坑清单

- ❌ 纯黑正文（#000000）
- ❌ 颜色超过3种
- ❌ 长段超过5行
- ❌ 首行缩进（手机端不适用）
- ❌ 满屏无留白
- ❌ 图片尺寸不一、无圆角
- ❌ 过度装饰（花边框、动效、杂乱符号）
- ❌ URL 不用 `<code>` 标签包裹（会被自动分词）

### ✅ 最佳实践

- ✅ 每段2-4行，一句话15-25字
- ✅ 段落间空1行（15px）
- ✅ 图片统一圆角4px
- ✅ 左右留边，不贴满屏幕
- ✅ 重点内容用高亮块，不超过3处/屏
- ✅ 列表项间距8-12px

## 使用场景

- 公众号文章排版
- 长文内容创作
- 干货类文章
- 教程类文章
- 观点类文章

## 效果预览

使用本排版规范后，你的文章将具备：

- 📱 手机端完美适配
- 👁️ 视觉层次清晰
- 🎨 配色专业统一
- 📖 阅读体验流畅
- ⚡ 重点一目了然

## License

MIT License

## 作者

Jarrett

## 贡献

欢迎提交 Issue 和 Pull Request 改进本规范。

---

**如果这个 Skill 对你有帮助，欢迎 Star ⭐**
