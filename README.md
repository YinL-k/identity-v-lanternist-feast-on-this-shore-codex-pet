# 幻灯师·于此岸赴宴

《第五人格》幻灯师「于此岸赴宴」的非官方同人动画宠物，提供两个独立版本：

| 版本 | 下载 | 预览 |
| --- | --- | --- |
| 幻灯师·于此岸赴宴 | [下载 ZIP](downloads/幻灯师·于此岸赴宴.zip) | [动作总览](preview/幻灯师·于此岸赴宴/contact-sheet.png) · [左跑](preview/幻灯师·于此岸赴宴/running-left.gif) |
| 幻灯师·于此岸赴宴 Q版 | [下载 ZIP](downloads/幻灯师·于此岸赴宴%20Q版.zip) | [动作总览](preview/幻灯师·于此岸赴宴%20Q版/contact-sheet.png) · [左跑](preview/幻灯师·于此岸赴宴%20Q版/running-left.gif) |

![幻灯师·于此岸赴宴](preview/幻灯师·于此岸赴宴/idle.gif)
![幻灯师·于此岸赴宴 Q版](preview/幻灯师·于此岸赴宴%20Q版/idle.gif)

## 安装到 Codex

适用于支持本地自定义宠物及 **v2 精灵图** 的 Codex 桌面客户端。这里提供的是本地文件包；GitHub ZIP 并不是 ChatGPT Work 的一键领养链接。尚未对其他客户端或所有客户端版本做安装测试。

1. 下载所选版本 ZIP，在 GitHub 文件页面点击 **Download raw file**。
2. 解压，将完整宠物文件夹放入 `$CODEX_HOME/pets/`；未设置 `CODEX_HOME` 时，默认目录为 `~/.codex/pets/`。Windows 默认位置为 `%USERPROFILE%\.codex\pets\`。
3. `pet.json` 与 `spritesheet.webp` 必须位于同一文件夹。不要覆盖已有同名文件夹；保留配置中的 `spriteVersionNumber: 2`。
4. 重启 Codex，然后在客户端的宠物选择界面选用对应名称。若客户端不支持 v2 或未显示本地宠物，请先确认客户端支持情况。

目录示例：

```text
~/.codex/pets/
  幻灯师·于此岸赴宴/
    pet.json
    spritesheet.webp
    spritesheet.png
    layout.json
  幻灯师·于此岸赴宴 Q版/
    pet.json
    spritesheet.webp
    spritesheet.png
    layout.json
```

`pet.json` 使用本机已安装 v2 宠物的配置字段：`id`、`displayName`、`description`、`spriteVersionNumber`、`spritesheetPath`。两个版本使用不同的 `id`，可并存。`layout.json` 仅用于说明图集布局，不是客户端安装配置。

## 素材与验证

每个版本均含当前已安装素材的原始 PNG 和像素一致的无损 WebP。运行时配置指向 WebP。精灵图为透明背景，1536 × 2288 像素，8 列 × 11 行，每格 192 × 208 像素。

前九行动作为待机、向右跑、向左跑、挥手、跳跃、失败反应、等待、工作、复核；帧数依次为 `6, 8, 8, 4, 5, 8, 6, 6, 6`。最后两行包含 16 个视线方向，从正上方开始按顺时针每隔 22.5° 排列。未使用的 15 格保持透明。

两份 PNG 及两份 WebP 均通过 Pets v2 结构验证，包括尺寸、必需帧、透明背景与空白格检查。WebP 解码后的 RGBA 与对应 PNG 完全一致。各动作 GIF 从发布图集生成；预览播放时长不代表所有客户端的运行时播放策略。文件 SHA256 见 [SHA256SUMS.txt](SHA256SUMS.txt)。

仓库当前仅提供以上两个版本；早期版本仍可从普通 Git 历史中恢复。

## 声明与署名

本项目为非官方同人作品，仅供个人学习、展示和非商业使用。《第五人格》、幻灯师、于此岸赴宴及相关角色、名称、原始设计和素材的权利归各自权利人所有。本项目与网易游戏无隶属、赞助或官方认可关系。

请勿将本项目用于商业用途。仓库不包含原始参考视频、参考图片、私人制作记录或源素材归档。详见 [NOTICE.md](NOTICE.md)。
