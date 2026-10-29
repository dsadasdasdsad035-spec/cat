# 第一集 AI 镜头生成提示词

只生成镜头 01–06。镜头 07–12 用实拍。蓝光做在真实眼睛素材上，不要另生成一只蓝眼狸花。

角色外观以 [`../猫咪真实参考照片/`](../猫咪真实参考照片/README.md) 里的实拍为准，优先用：
- [`../猫咪真实参考照片/微信图片_20261028100547_35_213.jpg`](../猫咪真实参考照片/微信图片_20261028100547_35_213.jpg)（眼睛与脸）
- [`../猫咪真实参考照片/微信图片_20261028095726_27_213.jpg`](../猫咪真实参考照片/微信图片_20261028095726_27_213.jpg)（白袜与虎斑）
- [`../猫咪真实参考照片/微信图片_20261028095723_26_213.jpg`](../猫咪真实参考照片/微信图片_20261028095723_26_213.jpg)（白手套前爪）

棚拍拼图 [`../猫咪真实参考照片/a_clean_studio_style_collage_photography_montage.png`](../猫咪真实参考照片/a_clean_studio_style_collage_photography_montage.png) 只能辅助花纹。它本身是 AI 图，眼睛比实拍更金，不要单独拿它当眼睛颜色标准。

## 角色一致性
同一只猫：young brown and black tabby, yellow-green to amber eyes, cream muzzle, white chest, white front and back paws, natural cat anatomy, realistic fur。可以比家里的成猫更小、毛尖带雨，但虎斑位置、白爪和白胸要能对上。不要新生未睁眼的奶猫，也不要换成另一只猫。

铲屎官没有真人参考图。雨夜只拍手、鞋和蹲下的身体，不生成可识别的人脸，也不要用某张真人照片去套脸。

## 统一负面提示
cartoon, anime, illustration, extra legs, extra paws, extra toes, deformed face, deformed hands, changing fur pattern, blue eyes, heterochromia, collar, clothing on cat, blood, wounds, graphic suffering, scruffing, grabbing, text, subtitles, timestamp, watermark, logo, news overlay, oversaturated neon

若工具把负面提示写进正文，就在主提示末尾加上：no text, no watermark, no blue irises, no injuries。

## AI-01：睁眼（镜头 01，约 4 秒）
**Prompt**

9:16 vertical cinematic photorealistic close-up, a young brown and black tabby kitten with yellow-green amber eyes, cream muzzle and white whiskers slowly opens its eyes in near darkness. A distant car headlight briefly crosses the pupils. Wet fur tips, no blood, no wounds, no collar. Camera almost on the ground, slight downward angle, shallow depth of field, restrained documentary realism, natural anatomy, no text.

## AI-02：干燥凹处（镜头 02–03，约 7 秒，可拆成全景和爪部两条）
**Prompt**

9:16 vertical cinematic photorealistic night scene at kitten eye level. The same young brown and black tabby with white chest and white paws crouches in a dry recessed corner beside an urban drainage channel, under a step or wall, not standing in water. Rain, wet pavement, distant warm streetlights in puddles, low cautious posture, ears lowered, white paws tucked at the chest. Natural fur, realistic rain, no injury, no blood, no text, no collar.

爪部特写在同一提示后加：side close-up of the white front paws and white chest, belly low to the dry ground.

## AI-03：鞋停住，手停住（镜头 04–06，约 16 秒，按三个镜头分别生成）
**镜头 04 Prompt**

9:16 vertical photorealistic shot from a kitten's ground-level point of view. Human legs and shoes look tall in the frame, walk through rain, then stop. The young tabby kitten pulls back into shadow until only its yellow-green eyes remain. No recognizable human face. Wet street, distant traffic, natural anatomy, no text.

**镜头 05 Prompt**

9:16 vertical photorealistic side view at kitten height. An adult in plain home clothes crouches to become smaller and extends one open hand, palm relaxed, fingers still, about an arm's length away. The same young brown tabby with white paws watches the hand, whiskers forward, then draws them back. The hand does not grab. Rainy background soft, natural lighting, no sudden movement, no recognizable face, no text.

**镜头 06 Prompt**

9:16 vertical photorealistic close-up of the same young tabby face. The open human hand stays where it is and does not come closer. The kitten breathes, body still, ears low, yellow-green eyes wary. No lifting, no scruffing, no carrier, no bag. Rain beginning to fall out of focus, restrained emotion, no text.

## 不要用 AI 重做的镜头
- 镜头 07–09、11：家里的真实狸花、黄色织物、放碗、看向门口。
- 镜头 10 和 12 的蓝光：用镜头 10 的实拍眼睛做后期，不要重新生成整张猫脸。

## 蓝光后期（镜头 10，余像用于镜头 12）
做在实拍眼部素材上：
- 只加在瞳孔高光旁边的一小点冷蓝，建议从 `#7EC8FF`、透明度约 20%–35% 试起。
- 竖屏手机全屏时要能看出「不对劲」，近看仍像高光，不像发光眼睛。宁可短，不要亮。
- 大约 8–12 帧，然后恢复原来的高光。眨眼时蓝光一起灭掉。
- 虹膜保持黄绿色到琥珀色，不要铺满，不要改成白猫那种蓝眼睛。
- 镜头 12 只用更弱的一闪，当作余像，接着淡出黑场。
- 不加界面、不加「人类视觉模式」、不加扫描框。那些是第5集的事。

## 生成顺序
1. 先用实拍照出一张静态关键帧，确认白爪、白胸、虎斑和眼睛颜色。
2. 关键帧通过后，再按镜头单独做图生视频。不要一次生成整集。
3. 手、爪、眼睛多出几条候选，废掉多指、多爪和花纹漂移的版本。
4. 雨夜整体偏冷、略降饱和、带细颗粒；溶进室内后改回实拍的暖色。冷暖差别就是回忆和家的分界。
5. 字幕、角标都在后期加。不要让模型自己写字。
