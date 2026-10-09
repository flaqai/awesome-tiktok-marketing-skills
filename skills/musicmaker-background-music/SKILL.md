---
name: musicmaker-background-music
description: Use when creating MusicMaker.im study or work background music, sleep ambience, quiet long-form music videos, or explicitly requested legacy song-and-MV campaigns.
---

# MusicMaker 背景音乐与循环画面

当前默认方向是学习／工作背景音和睡眠白噪声长视频。先交付 Suno 音频提示词、16:9 场景首帧提示词、短循环图片转视频提示词；不要自动附加歌词、美女 MV、橘猫或竖屏 Shorts。只有用户明确要求歌曲宣传时才切换到歌曲模式。

## 输入与模式

- 学习／工作：轻微稳定律动，稀疏旋律，音量和音色平稳，不抢注意力。
- 睡眠：连续柔和底噪为主，最多加入很轻的持续和弦；无明确节拍、突出旋律、唱声、鸟叫、雷声及突然音量变化。不作治疗失眠等效果保证。
- 原创歌曲：先确定曲风、情绪、听众及 hook，再写原创歌词和匹配歌曲的画面。若要求结合当下流行趋势，核查当期资料，不把历史趋势当现状。

新请求的模式、时长和比例优先。长视频总时长与视频模型单次生成时长是两个参数；不要宣称一条 15 秒生成片段就是完整长视频。

## 音画工作流

1. 用一句话确定用途和场景。场景可以是雪峰、草地、小木屋、海岸及其他安宁景观，不反复默认卧室或书房。
2. 写英文 Suno prompt：用途 → 音色 → 节奏和动态 → 起止衔接 → 简短排除项。睡眠模式尤其克制，默认每份英文 prompt 少于 2000 字符，交付前实际计数。
3. 写单张 16:9 首帧：固定地点、自然光、有限物体、安静构图。默认无人，画面无文字。首帧只描述静态起始状态。
4. 写约 15 秒 I2V 循环：锁定机位、焦点、曝光、白平衡、建筑与地形；只给一至两种低幅度环境运动。让末帧构图和亮度接近首帧，不安排事件、日夜变化或镜头推进。
5. 独立制作音乐与画面。默认关闭视频生成音乐，后期铺入音频；若用户要原生视频音频则明确改写音频策略。
6. 长片制作时先检查循环接缝，再重复画面、衔接音频。总时长按当前需求设置，不能仅凭 prompt 保证无缝。

## 歌曲模式补充

音乐先行，服装、场景和道具服务歌词与曲风。橘猫只是可选角色，粉色跑车、墨镜、DJ 台均不是固定配置。长 MV 用 16:9，明确需要短视频时才写 9:16；选择已提供成曲的真实时间段，不虚构听过音频或听到的节奏。保留用户指定的人物跨片段一致性。

## 输出与验收

按请求输出独立可复制的音频、图片、视频代码块；补一句循环检查说明。无歌词的模式不输出歌词。

检查音频突发音符、音量跳变、尖锐高频；检查视频镜头漂移、闪烁、影子移动、首尾亮度差。生成前只能检查提示词一致性，不能声称已验证成片。

完整示例见 下方的「示例」部分，需要睡眠三件套时读取。


## 示例

# 睡眠三件套：Swiss Alpine Quiet

以下是可改写的完整示例；三段英文提示词各少于 2000 字符。

## Suno
```text
Instrumental sleep ambience. A continuous soft rain-like noise bed with one very quiet layer of warm sustained ambient chords underneath. Noise remains the main texture; music is barely noticeable. Extremely sparse, slow and uneventful. Softened high frequencies, restrained bass and consistent volume. Chords change very slowly with gentle overlap. Begin softly and retain the same atmosphere to the end. No vocals, humming, distinct melody, rhythmic pulse, percussion, bells, birds, thunder, sudden sounds, builds or drops. No harsh hiss, deep rumble or sweeping stereo effects.
```

## 首帧
```text
Photorealistic Swiss alpine valley on a quiet overcast summer evening. Distant snow-covered peaks, a broad meadow of soft green grass, and one small weathered wooden cottage near the foot of the mountains. Wide eye-level landscape composition. The meadow fills the lower half, the cottage stays small, and snow peaks sit beneath a pale gray sky. A faint veil of drizzle softens distant slopes. Muted greens, gray-blue mountains, diffused light, low contrast and realistic textures. 16:9 landscape. No people, animals, vehicles, smoke, dramatic sunlight, glowing windows, text or logos.
```

## 循环视频
```text
Animate the supplied image into a quiet 15-second 16:9 landscape video. One completely locked camera shot. Preserve the framing, mountains, cottage and terrain. Fixed focus, exposure and white balance. Only two subtle movements: meadow grass sways almost imperceptibly in a gentle breeze, and fine drizzle falls softly across the distant valley. Rain never streaks across the lens. The cottage and mountains stay still. Maintain the same soft overcast light and muted colors. No events or visual progression. Keep first and last frames closely matched in composition and brightness for repeated playback. No camera movement, zoom, cuts, time-lapse, flicker, moving shadows, added objects or generated audio.
```

验收场景：用户说“只要睡眠长视频，尽量少元素”，应直接给这类三件套，而不是流行歌歌词、短视频 hook 和多镜头 MV。
