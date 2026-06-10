# Animal Crossing Style Image Prompt

这个仓库用于开源和维护 Codex / Claude Code Skill。每个 skill 放在 `skills/<skill-name>/` 下。

当前包含：

- `animal-crossing-style-prompt`：生成动物森友会原版游戏实况截图风格的图片提示词

## 安装

先克隆仓库：

```bash
git clone https://github.com/Isaacocu/animal-crossing-style-prompt.git
```

安装到全局 Claude Code skills：

```bash
mkdir -p ~/.claude/skills
cp -R animal-crossing-style-prompt/skills/animal-crossing-style-prompt \
  ~/.claude/skills/animal-crossing-style-prompt
```

或安装到当前项目：

```bash
mkdir -p .claude/skills
cp -R animal-crossing-style-prompt/skills/animal-crossing-style-prompt \
  .claude/skills/animal-crossing-style-prompt
```

安装后重启 Claude Code，让 skill 被重新扫描。

## 使用

在 Claude Code 里直接提出需求：

```text
使用 animal-crossing-style-prompt，帮我写一个北京故宫的动森风格图片提示词，不用出图。
```

skill 会输出可直接交给图片生成模型的最终提示词代码块。

拿到 prompt 后复制到任意生图工具即可出图。**建议使用 GPT Image 2**（ChatGPT 图片生成），对动森游戏截图风格的还原度最高。其他支持的工具：Midjourney、通义万相、即梦等。

> 提示：默认画面比例为 16:9 横图，与 Switch 实机截图一致。在生图工具中选择横版（landscape）尺寸效果最佳。

## 示例效果

输入：`帮我写一个上海外滩夜景的动森风格提示词`

输出：

```text
动物森友会原版游戏实况截图复刻
画风：任天堂 Switch 集合啦！动物森友会实机游戏截图风格；不要写实摄影、不要电影 CG、不要赛璐珞动画、不要像素风、不要水彩手绘
玩家角色 + 同行动物邻居：岛民默认造型，杰克同行

岛屿区域：上海·外滩万国建筑群
画面要素：圆润矮胖欧式小楼群、黄浦江河畔、串灯纸灯笼、石板江堤步道、钟楼
生活时刻：玩家角色与杰克沿江堤漫步欣赏夜景，休闲状态

动森元素：Nook商店欧式变体、木质路灯、告示牌、长椅、喷泉、露天咖啡座
季节与时段：秋·夜晚
岛名 UI 文字：右下角小字「外滩岛」；按原版登岛画面风格呈现，白色无衬线小字、半透明、不加边框底纹
UI 界面：按 ACNH 原版游戏实况自然出现，不堆满
文字：所有可读 UI 使用中文，按键提示只用中文动词
```

## 灵感来源

本项目的 skill 结构和提示词工程方法参考了 [@林克漫游](https://github.com/xiaoTN) 的 [zelda-style-image-prompt](https://github.com/xiaoTN/zelda-style-image-prompt)，感谢开源分享。

## 声明

本仓库只包含提示词写作规则和参考文档，不包含任何游戏素材、图片、模型、字体、音频或任天堂资源。

本项目与 Nintendo、Animal Crossing、集合啦！动物森友会或其权利方没有关联、授权、赞助或背书关系。项目中出现的游戏名称、角色名称和商标仅用于描述提示词风格与兼容场景。

使用本仓库中的 skill 生成、发布或商用任何内容时，请自行确认是否符合相关平台规则、模型服务条款和知识产权要求。

## License

MIT
