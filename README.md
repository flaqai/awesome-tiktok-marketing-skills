# Awesome TikTok Marketing Skills

从实际 AI 视频账号制作与提示词迭代中整理的 9 个可复用技能。覆盖 TikTok、YouTube Shorts、Reels 等短视频创作，以及 MusicMaker 背景音乐长视频。正文以中文说明工作流，提示词示例按场景使用中文或英文。

每个目录包含独立的 `SKILL.md`（触发条件、角色规则、流程、纠错与验收），并在文末内附可改写示例。这些是内容生产技能，不是自动运营或自动发布程序。

## 技能目录

| 技能 | 用途 | 默认输出 |
|---|---|---|
| [MusicMaker 背景音乐](skills/musicmaker-background-music/SKILL.md) | 学习、工作、睡眠背景音；按需保留歌曲 MV 模式 | Suno prompt + 16:9 首帧 + 循环视频 prompt |
| [AITryOn 真人奇观](skills/aitryon-cinematic-videos/SKILL.md) | 固定成年女主、艺术世界穿越、真人游戏 | 参考图片 prompts + 视频时间线 |
| [Seaimagine 虚拟女主](skills/seaimagine-influencer-videos/SKILL.md) | 金发女主舞蹈、随手拍、运动与真人游戏 | 首帧／参考图 + 中文视频 prompt |
| [VideoWeb 布偶猫](skills/videoweb-ragdoll-videos/SKILL.md) | 单猫舞蹈、双猫斗舞、猫咪短剧 | 9:16 首帧；短剧另配参考图与时间线 |
| [Fylia 动作喜剧](skills/fylia-dramatic-video-director/SKILL.md) | 固定成年女主、连续夸张特技与音乐卡点 | 首帧提示词 + 时间轴视频 prompt；附导演参考资料 |
| [Seevido 浣熊短剧](skills/seevido-raccoon-stories/SKILL.md) | 可爱浣熊、多角色情绪喜剧、POV 互动 | 角色／场景参考图 + 中文视频 prompt |
| [Flaq AI／UGC Maker 展示](skills/flaq-ugc-model-showcase/SKILL.md) | 模型对比、视觉爆点、自然品牌植入 | 统一对比素材或品牌视频方案 |
| [Heydream 宝宝舞蹈](skills/heydream-baby-dance/SKILL.md) | 单宝宝、双宝宝斗舞、多样成年观众 | 写实手机风格 9:16 场景图 |
| [Flyne AI 白博美](skills/flyne-pomeranian-dance/SKILL.md) | 蓝眼白博美舞蹈、新衣帽与动物观众 | 适合 motion control 的 9:16 首帧 |

## 使用方式

把需要的整个技能目录放入所用助手支持的技能目录；也可直接让助手读取对应的 `SKILL.md`。不用一次加载全部九个技能。

示例请求：

```text
使用 flyne-pomeranian-dance。以我上传的博美图片锁定身份，制作新的明亮 cool 场景，换衣服和观众。只要首帧图片提示词。
```

```text
使用 flaq-ugc-model-showcase，为 Flaq AI 做 15 秒模型对比。两个模型使用相同参考图和剧情。请给参考图片提示词、中文视频提示词和对比检查点。
```

```text
使用 musicmaker-background-music，做睡眠白噪声长视频。场景选雪峰草地，声音极简，每份英文提示词少于 2000 字符。
```

## 共同约定

- 当前请求及最新确认的身份图优先。示例中的服装、人数、场景不是永久规则。
- 首帧图、身份参考图、分镜表的用途不同；不要把角色拼贴自动当作第零秒画面。
- 历史上需要的原始人物参考图、视频与音频不包含在本仓库。使用者自行提供素材；缺少图片时只能近似外观，不能保证复现同一身份。
- 模型名称、输入限制和可用功能需要按实际平台核对。图片／视频 prompt 不等于生成结果，写好文案不等于发布成功。
- 不附带账号凭据、个人路径、原始聊天记录或第三方案例媒体；不保证流量、转化或模型效果。

## 整理依据与版本差异

本次整理依据以下九个工作对话及其中指向的已有草稿，采用已读取的后期明确修正：

| 来源对话 | 提炼重点 |
|---|---|
| Musicmaker VIdeos | 新增学习／睡眠长视频默认路线，歌曲 MV 改为按需 |
| AITryOn Videos New | 参考图职责、30 秒艺术片、游戏镜头压力与动作反馈 |
| Seaimagine Video | 固定金发身份、真实手机感、运动因果、游戏动作节奏 |
| Videoweb Videos | 自然双足站立、裸爪、不同观众、斗舞露脸、非舞蹈故事 |
| Fylia AI Videos New | 连续动作升级、夸张受力、背景音乐与接触音效 |
| Seevido raccoon video | 多只浣熊计数、POV 路线、情绪与事件因果 |
| flaq ai/ugc maker | 品牌区分、模型对比、确定性 prompt、实体品牌承载 |
| Heydream Baby dance | 单人／斗舞／并排路由、主角露脸、分体童装、多样观众 |
| flyne ai dog | 最新蓝眼身份、短手短腿、正常站立裸爪、场景与衣帽变化 |

示例经过整理和改写，用于说明工作流，并非原聊天逐字导出。Fylia 新版默认配合 `seedance-2-5-video-director` 做 Seedance 2.5 模型适配；该配套技能未收入本仓库。其他模型或缺少配套技能时，Fylia 技能仍可编写模型中性的导演稿。

## 版本选择

每个账号保留一个面向视频制作的技能。Fylia 使用 2026-10-09 新建的 `fylia-dramatic-video-director`，取代 2026-09-20 的 `fylia-comedy-stunts`；其余八个技能沿用 2026-09-20 整理版。Flaq AI 和 UGC Maker 共用一个技能，按品牌分别处理。

## License

[MIT](LICENSE)，沿用仓库原有许可证。
