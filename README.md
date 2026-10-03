# 第五人格桌宠 · Identity V Desktop Pets

把喜欢的《第五人格》角色带到桌面上。这里收录非官方同人动画桌宠、安装包与动作预览，也欢迎大家投稿喜欢的角色、时装和不同画风的作品。

当前提供支持 **v2 精灵图** 的 Codex 本地桌宠包，每款包含 9 组动作和 16 个注视方向。其他客户端的适配也欢迎一起补充。

## 下载与预览

| 角色 · 时装 | 版本 | 下载 | 预览 |
| --- | --- | --- | --- |
| 幻灯师 · 于此岸赴宴 | 标准版 | [下载 ZIP](downloads/幻灯师·于此岸赴宴.zip) | [动作总览](preview/幻灯师·于此岸赴宴/contact-sheet.png) · [左跑](preview/幻灯师·于此岸赴宴/running-left.gif) |
| 幻灯师 · 于此岸赴宴 | Q版 | [下载 ZIP](downloads/幻灯师·于此岸赴宴%20Q版.zip) | [动作总览](preview/幻灯师·于此岸赴宴%20Q版/contact-sheet.png) · [左跑](preview/幻灯师·于此岸赴宴%20Q版/running-left.gif) |
| 机械师 · 锁芯 | 标准版 | [下载 ZIP](downloads/机械师·锁芯.zip) | [全部动作](preview/机械师·锁芯/all-states.gif) · [动作总览](preview/机械师·锁芯/contact-sheet.png) |
| 机械师 · 锁芯 | Q版 | [下载 ZIP](downloads/机械师·锁芯%20Q版.zip) | [全部动作](preview/机械师·锁芯%20Q版/all-states.gif) · [MP4](preview/机械师·锁芯%20Q版/all-states.mp4) · [动作总览](preview/机械师·锁芯%20Q版/contact-sheet.png) |

### 幻灯师 · 于此岸赴宴

标准版与 Q版可独立安装、并存使用。

![幻灯师·于此岸赴宴](preview/幻灯师·于此岸赴宴/idle.gif)
![幻灯师·于此岸赴宴 Q版](preview/幻灯师·于此岸赴宴%20Q版/idle.gif)

### 机械师 · 锁芯

修长精致的标准版，保留紫晶锁瞳与非对称机械臂，可与 Q版独立安装。

![机械师·锁芯](preview/机械师·锁芯/idle.gif)

[全部动作](preview/机械师·锁芯/all-states.gif) · [16 方向注视](preview/机械师·锁芯/look-loop.gif)

### 机械师 · 锁芯 Q版

保留猫耳帽、紫晶锁瞳、非对称机械臂与裙摆细节的 Q版机械师。此次发布包含调整后的左跑与跳跃动作。

![机械师·锁芯 Q版](preview/机械师·锁芯%20Q版/idle.gif)

[向左跑](preview/机械师·锁芯%20Q版/running-left.gif) · [向右跑](preview/机械师·锁芯%20Q版/running-right.gif) · [跳跃](preview/机械师·锁芯%20Q版/jumping.gif) · [待机与跳跃衔接](preview/机械师·锁芯%20Q版/idle-jump-idle.gif) · [16 方向注视](preview/机械师·锁芯%20Q版/look-loop.gif)

## 安装到 Codex

适用于支持本地自定义宠物及 **v2 精灵图** 的 Codex 桌面客户端。这里提供的是本地文件包；GitHub ZIP 不是 ChatGPT Work 的一键领养链接。尚未对其他客户端或所有客户端版本做安装测试。

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
  机械师·锁芯/
    pet.json
    spritesheet.webp
    spritesheet.png
    layout.json
  机械师·锁芯 Q版/
    pet.json
    spritesheet.webp
    spritesheet.png
    layout.json
```

`pet.json` 沿用现有 v2 宠物的配置字段：`id`、`displayName`、`description`、`spriteVersionNumber`、`spritesheetPath`。各版本使用不同的 `id`，可并存。`layout.json` 仅用于说明图集布局，不是客户端安装配置。

## 欢迎投稿

欢迎提交新的角色、时装、不同风格的桌宠，也欢迎修复动作、完善安装说明和补充客户端适配。

- 有想看的角色、遇到问题或还没有完整作品，可以直接提 [Issue](https://github.com/YinL-k/identity-v-lanternist-feast-on-this-shore-codex-pet/issues)
- 已有作品可以提交 [Pull Request](https://github.com/YinL-k/identity-v-lanternist-feast-on-this-shore-codex-pet/pulls)，附上预览，注明原作者和来源
- 不要求提交授权证明；请尊重原作者明确标注的使用限制，署名本身不代替授权

简单的目录、图集要求和投稿说明见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 素材与验证

每款均含原始 PNG 和像素一致的无损 WebP，运行时配置指向 WebP。精灵图为透明背景，1536 × 2288 像素，8 列 × 11 行，每格 192 × 208 像素，共 73 个有效帧。

前九行动作为待机、向右跑、向左跑、挥手、跳跃、失败反应、等待、工作、复核；帧数依次为 `6, 8, 8, 4, 5, 8, 6, 6, 6`。最后两行包含 16 个视线方向，从正上方开始按顺时针每隔 22.5° 排列。未使用的 15 格保持透明。

已发布图集通过 v2 结构检查，WebP 解码后的 RGBA 与对应 PNG 完全一致。各动作 GIF 从发布图集生成；预览时长不代表所有客户端的运行时播放策略。文件校验值见 [SHA256SUMS.txt](SHA256SUMS.txt)。

本次补充机械师·锁芯标准版；Q版与用户指定图集逐像素一致，保留现有素材与安装包。已有两个幻灯师版本的素材与安装包保持不变。早期版本仍可从普通 Git 历史中恢复。

## 声明与署名

本项目为非官方同人作品，仅供个人学习、展示和非商业使用。《第五人格》及相关角色、时装、名称、原始设计和素材的权利归各自权利人所有。本项目与网易游戏无隶属、赞助或官方认可关系。

- 角色与时装原始设计：网易游戏《第五人格》
- 当前桌宠制作与整理：[YinL-k](https://github.com/YinL-k)，使用 AI 辅助制作
- 社区投稿：在对应作品说明中保留原作者、贡献者与来源

仓库不包含原始参考视频、参考图片、私人制作记录或源素材归档。详见 [NOTICE.md](NOTICE.md)。
