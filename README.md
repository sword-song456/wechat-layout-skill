# 微信公众号专业排版 Skill

> 基于信息分层设计的公众号排版规范，让你的文章在手机端拥有专业级阅读体验。

## 特性

- 📱 **手机优先**：所有尺寸针对手机端优化
- 🎨 **3色原则**：正文#333、主色#00a3a4、注释#999
- 📐 **信息分层**：3种高亮方式区分不同重要级别
- ✅ **开箱即用**：复制粘贴即可使用的HTML模板
- 🚀 **专业级排版**：参考头部公众号排版标准

## 快速开始

### 基础段落

```html
<p style="margin: 0 0 15px 0; color: #333333; font-size: 15px; line-height: 1.75;">
正文内容
</p>
```

### 核心观点（浅黄背景块）

```html
<section style="background: #fffbf0; padding: 15px; margin: 15px 0; border-radius: 6px;">
<p style="margin: 0; color: #1a1a1a; font-size: 15px; line-height: 1.75; font-weight: 600;">
核心观点文字
</p>
</section>
```

### 关键结论（浅青色块）

```html
<section style="background: #f0fafa; padding: 15px; margin: 15px 0; border-radius: 6px; border-left: 3px solid #00a3a4;">
<p style="margin: 0; color: #00a3a4; font-size: 15px; line-height: 1.75; font-weight: 600;">
关键结论文字
</p>
</section>
```

### 章节标题

```html
<h2 style="font-size: 18px; color: #1a1a1a; margin: 30px 0 15px; font-weight: 700; padding-left: 12px; border-left: 4px solid #00a3a4;">
章节标题
</h2>
```

## 完整文档

查看 [SKILL.md](./SKILL.md) 获取完整排版规范和示例。

## 效果预览

使用本排版规范后，你的文章将具备：

- 📱 手机端完美适配
- 👁️ 视觉层次清晰
- 🎨 配色专业统一
- 📖 阅读体验流畅
- ⚡ 重点一目了然

## 使用场景

- 公众号文章排版
- 长文内容创作
- 干货类文章
- 教程类文章
- 观点类文章

## 避坑清单

❌ 不要做：
- 纯黑正文（#000000）
- 颜色超过3种
- 长段超过5行
- 首行缩进
- 满屏无留白

✅ 应该做：
- 每段2-4行
- 段落间空1行
- 图片统一圆角
- 左右留边
- 重点用高亮块

## License

MIT License

## 作者

Jarrett

## 贡献

欢迎提交 Issue 和 Pull Request 改进本规范。

---

**如果这个 Skill 对你有帮助，欢迎 Star ⭐**
