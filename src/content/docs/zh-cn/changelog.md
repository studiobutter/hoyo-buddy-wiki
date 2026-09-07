---
title: "更新日志"
---

## v1.16.23

### 新功能

- (`/search hsr`) 新增敌人分类。
- (`/challenge hsr`) 混沌回忆、虚构叙事及末日幻影卡片新增星启模式。
- (`/challenge zzz`) 危局强袭战卡片新增困难模式。
- (`/gacha-log import`) 《绝区零》的HoYoLAB账号现可一键导入抽卡记录，无需提供链接。
- (`/mimo`) 新增积分历史记录查看。
- (`/accounts`) 显示所选账号各项自动任务的状态与最后执行时间。
- (`/profile zzz`) 新增Sigrid的卡片数据。

### 功能优化

- (`/search`) 拆分为 `/search genshin` 与 `/search hsr` 子指令，与 `/profile` 保持一致。
- (`/gacha-log import`) 导入时仅获取新记录，不再每次重新获取完整历史。
- (`/gacha-log view`) 自动更新常驻卡池物品列表，确保限定物品加入常驻池后50/50胜率统计依然准确。
- (`/challenge hsr`) 即使未通关星启关卡，也会显示星启队伍。
- (`/challenge genshin stygian`) 恢复敌人弱点与强度信息。
- (`/accompany`) 在角色界面中显示自动陪伴开关。
- (`/notes`) 移除《崩坏：星穹铁道》的委托栏位与委托提醒，因游戏中已不再有委托功能。
- 自动任务的私信通知若在排队期间被关闭设置，将不再发送，并在每条通知中显示操作发生的时间。
- 将最多10条自动任务通知合并为一条私信，并丢弃超过12小时的成功通知。

### Bug修复

- (`/gacha-log view`) 修复了《绝区零》S级角色在其自身UP卡池中抽出时被计为50/50失败的问题。

## v1.16.22

### 新功能

- (`/accompany`) 新增指令：可查看HoYoLab陪伴角色、设置个人陪伴角色，开启自动签到。
- (`/settings`) 新增陪伴角色自动签到相关设置项。
- (`/profile genshin`) 新增原神Enka卡片风格。
- (`/profile hsr`) 更新了《崩坏：星穹铁道》角色卡片数据，包括姬子SP。
- (`/profile zzz`) 更新了《绝区零》角色卡片数据。
- (`/profile zzz`) 新增「流明」属性支持。
- (`/card-settings`) 新增了《原神》和《崩坏：星穹铁道》Enka样式卡片副词条强化档次展示开关。

### 功能优化

- (`/card-settings`) 重新设计了图片设置，统一并入卡片设置中；移除了 `/profile` 图片设置的独立按钮。
- (`/card-settings`) 在所有模板上支持自定义图片设置，若所选模板不支持，则会弹出警告。
- (`/card-settings`) 根据卡片所用立绘展示官方原画预览。
- (`/card-settings`) 因对应第三方接口已失效，自定义Pixiv图源支持已移除。
- (`/profile genshin`) 移除了hattvr卡片样式；原有配置迁移至Enka卡片样式。
- 优化《原神》《崩坏：星穹铁道》指令内角色名称自动补全的速度与准确度。

### Bug修复

- (`/profile`) 修复了参数传入旅行者时预选角色异常问题。
- (`/profile zzz`) 修复了音擎部分无副词条时报错的问题。
- (`/profile zzz`) 修复了维琳娜皮肤ID错误问题。
- (`/card-settings`) 修复了不同游戏角色ID冲突造成程序崩溃的问题。
- (`/card-settings`) 修复了图片选择器无法停留在当前图片分页的问题。
- (`/characters zzz`) 修复了当筛选阵营选项超过25个时崩溃的问题。
- (`/characters genshin`) 修复了筛选条件为空提交时报错的问题。
- (`/challenge`) 当期无数据时，正常展示历史记录。
- (`/challenge genshin`) 修复了部分榜单无数据时，深境螺旋伤害信息消失的问题。
- (`/events`) 修复了活动奖励稀有度未知时报错的问题。
- (`/search`) 修复了测试服物品名称自动补全异常的问题。
- 修复了文档链接打开语言不匹配的问题。

## v1.16.21

### 新增功能

- (`/profile hsr`) 补充了《崩坏：星穹铁道》4.3版本角色卡片数据。
- (`/profile zzz`) 补充了《绝区零》3.0版本角色卡片的数据。
- (`/profile`) 新增了《崩坏：星穹铁道》和《绝区零》Enka样式的卡片。
- (`/profile zzz`) 新增了风属性适配支持。
- (`/characters zzz`) 展示音擎等级和技能等级。

### 优化内容

- (`/profile`) 缓存缩放图片，提升卡片渲染速度。
- (`/characters`) 缓存已渲染界面，切换页面更流畅。
- (`/events`) 对于没有活动日历的游戏，会显示一条明确的“功能暂不支持”提示信息。
- (`/notes`) 移动端推送通知时显示备忘提醒文字。

### 问题修复

- (`/challenge hsr`) 修复了末日幻影、忘却之庭、虚构叙事层数数据不全时程序报错的问题。
- (`/profile`) 修复了原神伤害加成默认词条误显示成风元素伤害加成的问题。
- (`/profile`) 修复了原神由于缺失属性、角色立绘数据而导致卡片渲染异常的问题。
- (`/profile zzz`) 修复了绝区零3.0角色卡片样式2图片错位的问题。
- (`/card-settings`) 修复了当配置《原神》旅行者时校验错误的问题。
- (`/search`)修复了当打开无语录/故事的对应角色页面报错的问题。
- (`/redeem`) 优化了对于兑换错误的处理逻辑。
- 修复了关闭通知设置不生效，导致自动兑换私信骚扰推送的问题。
- 当设置中未设置语言时，将会自动读取Discord客户端语言作为备选。

## v1.16.20

### 新功能

- (`/profile zzz`) 新增了《绝区零》2.8版本角色卡片的数据。
- (`/profile zzz`) 新增了星见 雅皮肤卡片的数据

### 改善

- (`/profile hsr`) 优化配装面板属性展示逻辑，包括欢愉伤害加成。

### Bug 修复

- (`/profile zzz`) 修复了《绝区零》新角色意象影画图片丢失的问题。
- (`/profile`) 保留传入角色参数的原有顺序。
- (`/gacha-log`) 抽卡物品丢失时会用占位符图片展示。

## v1.16.19

### 新功能

- (`/challenge hsr anomaly`) 现在可获取最新三期记录。
- (`/mimo`) 新增了对完成原神视频任务支持。
- (`/notes`) 新增了《云·绝区零》国际服打开游戏的按钮选项。
- (`/profile hsr`) 搜索开拓者时，由显示元素改为显示命途。

### 改善

- (`/profile`) 新增对《崩坏：星穹铁道》新角色的支持（开拓者：欢愉）
- (`/challenge zzz shiyu`) 在新版卡片布局中隐藏通关时间文本。

### Bug 修复

- (`/challenge hsr anomaly`) 修复了空白字符块的图标位置的问题。
- (`/profile zzz`) 修复了爱苪和南宫羽造型图片位置错误或丢失的问题。

## v1.16.18

### 新功能

- (`/profile`) 新增对《绝区零》2.7版本和《崩坏：星穹铁道》4.1版本角色的支持。

### Bug修复

- (`/characters zzz`) 修复了角色过多时的性能问题。
- (`/events hsr`) 修复了下拉菜单时异相仲裁显示错误问题。
- (`/card-settings`) 修复了绝区零无效查询错误的问题。
- (`/notes`) 修复了在UI切换账号时的错误问题。
- (`/search`) 修复了在《崩坏：星穹铁道》查询书籍时的错误问题。
- (`/profile zzz`) 修复了爱苪图片在队伍卡片中显示不恰当的问题。
- (`/profile zzz`) 修复了潘引壶造型卡片数据丢失的问题。

## v1.16.17a

### 优化

- “你知道吗？”提示信息更新 - 2026年4月1日

## v1.16.17

### 新功能

- (`/profile hsr`) 新增对崩坏：星穹铁道 4.0 新角色的支持，包括全新的欢愉命途。
- (`/challenge zzz shiyu`) 新增对式舆防卫战 v2 的支持。
- (`/profile zzz`) 新增 ZZZ 2.6 角色的卡片数据。

### 问题修复

- (`/challenge zzz shiyu`) 修复卡片渲染问题，并处理获取式舆防卫战数据时的错误。
- (`/characters hsr`) 修复命途角色数量缺失时筛选器崩溃的问题。
- (`/events zzz`) 修复武器对象解析错误。
- (`/profile hsr`) 修复顶尖配置排名百分比格式错误的问题。
- (`/notes`) 修复崩坏3缺少体力提醒间隔的问题。
- 修复 zh-CN 及其他语言的本地化换行问题。

## v1.16.16

### 新功能

- (`/profile zzz`) 新增 ZZZ 2.5 角色卡片数据，包括简·杜的皮肤。
- (`/profile hsr`) 新增对欢愉命途类型的初步支持。
- (`/gacha-log`) 新增对 ZZZ 新卡池类型的支持（仅官方导入）。
- (`/build zzz`) 在攻略概览中显示攻略作者和最后更新日期。

### 优化

- (`/build zzz`) 改善了攻略章节的间距和可读性。

### 问题修复

- (`/gacha-log upload`) 修复了 UIGF v4.1 导入无法正常工作的问题。
- (`/notes`) 允许将实时便笺通知时间设置为提前 0 小时（即恰好到时通知）。
- (`/mimo`) 禁用原神旅行 Mimo 的自动抽奖功能。
- (`/mimo`) 处理获取原神旅行 Mimo 任务时的 -510001 错误。

## v1.16.15

### 新功能

- (`/build zzz`) 新增显示绝区零角色面板的指令。
- (`/profile hsr`) 新增大丽花的卡片数据。
- (`/mimo`) 重新启用原神旅行 Mimo 支持。
- (`/mimo`) 新增对新的原神旅行 Mimo 任务类型的支持。
- 优化了字体检测以更好地处理阿拉伯语和其他非拉丁文字。

### 优化

- (`/profile hsr`) 优化了大丽花的卡片颜色。
- 实现零停机更新，机器人在代码更新期间将不会下线。

### 问题修复

- (`/profile genshin`) 修复转换 HoYoLAB 原神角色时的 KeyError 错误。
- (`/gacha-log view`) 修复崩坏：星穹铁道和绝区零抽卡记录中缺少物品图标的问题。
- (`/gacha-log view`) 修复小屏幕设备上的 UI 问题。
- 修复开关切换按钮未正确返回 `False` 的问题。
- 修复多个内部部署和调度问题。

## v1.16.14

### 新功能

- (`/profile`) 新增对绝区零新角色的支持。
- (`/exploration`) 添加新区域。
- (`/events`) 新增对绝区零的支持。

### 改善

- (`/characters`) 默认用等级为角色排序。
- (`/characters`) 在卡片背景添加了角色稀有度的微光标识。
- (`/about`) 对用户链接使用Discord协议URL。
- 新增了假设置按钮，引导用户去使用 `/settings` 命令。

### Bug 修复

- (`/challenge genshin`) 修复了幽境危战和幻想真境剧诗卡片文本溢出的问题。
- (`/challenge genshin theater`) 修复了当语言为越南语时，圣牌挑战不显示的问题。
- (`/challenge hsr anomaly`) 修复了季度名字的文本溢出问题。
- (`/settings`) 修复了旅行Mimo设置里不能选择账户的问题。
- (`/settings`) 修复了所有账户能访问通知设置的问题。
- (`/profile hsr`) 修复了构建卡片的跟踪位置。
- (`/profile hsr`) 修复了特定角色词条图标丢失的问题。
- (`/search`, `/profile zzz`) 修复了在自动补充时角色丢失问题，比如艾莲、「11号」。
- (`/settings`) 修复了当点击兑换通知开关时，设置错误更改的问题。
- (`/profile zzz`) 修复了丽娜的图像与队伍卡片中心不对齐的问题。
- 将UID掩码字符从“*”更改为“x”，以避免标记问题。

## v1.16.13

### 新功能

- (`/profile`) 新增了对《崩坏：星穹铁道》和《绝区零》新角色的支持。
- (`/challenge genshin theater`) 新增了对圣牌挑战的支持。
- (`/profile hsr`) 对HoYoLAB/米游社角色新增了光锥词条显示。
- (`/challenge hsr anomaly`) 新增了对异相仲裁的支持。
- (`/profile genshin`) 新增了对奇偶 • 男性和奇偶 • 女性的支持。
- (`/gacha-log`) 新增了对千星奇域抽卡记录的支持。
- (`/settings`) 改进了设置命令的UI界面。

### 改善

- (`/gacha-log view`) 改善了抽卡日志查看器的性能。
- 改善了自动签到、自动兑换、自动旅行Mimo任务的性能。
- 改善了机器人的整体性能。

### Bug 修复

由于太多，请参阅[完整更新日志](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.13)。

## v1.16.12

注：该版本的原神旅行 Mimo 由于被 HoYoLab 移除而关闭。该功能在原神旅行 Mimo 回归后重新启用。

### 新功能

- (`/profile`) 新增对《绝区零》和《崩坏：星穹铁道》新角色的支持。
- (`/gacha-log import`) 使用我们的 [自製脚本](https://github.com/studiobutter/gacha-stuff) 导入抽卡日志。
- (`/challenge zzz shiyu`) 最快通关时长更替为总通关时长。
- (`/challenge genshin stygian`) 新增了敌人弱点和敌人优势的相关信息。
- 添加了对挪德卡莱的支持。

### 改善

- (`/profile`) 为 Enka Network 接口请求添加了更强的错误处理。
- (`/profile`) 为 Enka Network 角色配置接口请求添加了错误处理。
- (`/profile`) 为第三方卡片生成接口添加了错误处理。
- (`/accounts`) 解决了 Discord OAuth2 接口错误问题。
- (`/notes`) 在通知设置界面中添加了对不同输入的描述。
- 由于 Discord 的一个漏洞，WEBP 图片无法复制，因此我们现在将信息图表改为以 PNG 格式发送。

### Bug修复

- (`/gacha-log view`) 修复了自选常驻角色未被计入大保底的问题。
- (`/gacha-log view`) 修复了对于一些《绝区零》物品的错误稀有度问题。
- (`/search`) 修复了在自动补全中出现《绝区零》未公开角色的问题。
- (`/challenge zzz shiyu`) 解决了没有总通关时长的情况。
- (`/upload`) 修复了图片上传问题。
- (`/challenge genshin stygian`) 修复了一些敌人的文本溢出问题。
- (`/challenge zzz assault`) 修复了访问过去挑战的邦布图标的问题。
- (`/gacha-log view`) 解决了无效输入卡池问题。
- (`/challenge`) 修复了选择挑战期数下拉菜单长度超过25个时出错的问题。

## v1.16.11

### 新功能

- (`/search`) 添加了冰开拓者。
- (`/accounts`) 为邮箱登录添加了设备标识符，便于在Hoyoverse账号中心查看到 Hoyo Buddy 的设备。

### Bug 修复

- (`/profile zzz`) 更新了enka.py以匹配新的API格式。
- (`/profile`) 修复了Enka结果始终以英文返回的问题。
- (`/exploration`) 修复了部族声望等级文本溢出的问题。
- 修复了en-GB语言环境的翻译问题。

## v1.16.10

### 新功能

- (`/profile hsr`) 支持新角色：海瑟音和刻律德菈。
- (`/gacha-log upload`) 当账号游戏记录与导入的游戏记录不一时，会显示错误了。

### 改进

- (`/gacha-log import`) 改善了导入性能。
- 缓存经常使用的数据，像设置和卡片设置，以优化性能。
- 模糊的UID位数从3位更改至5位。

### Bug修复

- (`/profile zzz`) 修复了生成队伍卡片时自定义图片丢失的问题。
- (`/profile zzz`) 修复了爱丽丝夏装数据丢失的问题。
- (`/profile zzz`) 修复了由自定义数据造成的错误。
- (`/profile zzz`) 修复了有时 Enka Network 配置不能展示的问题。
- (`/search`) 修复了在正常搜索自动补齐时的未公开内容显示的问题。

## v1.16.9

### 新功能

- (`/profile zzz`) 添加了对Enka Network的支持。
- (`/about`) 为此命令添加了更多链接。
- 新增了`/changelog`、`/invite`、`/help`命令。
- 添加了简体中文和西班牙语的文档支持。
- 添加了可检查该机器人状态的[状态页](https://status.seria.moe/?catagory=Hoyo%20Buddy)。

### 改进

- (`/settings`) 此命令现在以短暂消息回应。

### Bug修复

- (`/accounts`) 修复了账号登录问题。
- (`/gacha-log manage`) 修复了绝区零导出时物品稀有度错误问题。
- (`/gacha-log view`) 修复了物品名字为“？？？”问题。
- (`/profile genshin`) 修复了当数据源为HoYoLab时玩家预览不显示的问题。

## v1.16.8

### 新功能

- (`/challenge zzz shiyu`) 添加通关时间。
- (`/challenge hsr`) 隐藏快速通关。
- (`/challenge hsr`) 添加「显示 UID」选项。
- (`/gacha-log`) 支持星穹铁道联动卡池。
- (`/profile zzz`) 添加对新角色的支持：Alice 和 Yuzuha。
- (`/profile zzz`) 添加对代理人服装的支持。
- 机器人在代码更新期间不会再离线。

### 优化

- (`/profile hsr`) 改善样式 2 的文字位置。
- (`/events`) 改善亮色模式的色彩对比度。
- (`/gacha-log view`) 当更改卡池类型时更改网页应用程序链接。
- (`/search`) 星穹铁道角色故事现在以更清晰的方式显示。
- 通过更好的缓存改善图片生成性能。
- 保存图片为 webp 格式而非 png 以减少文件大小。

### 错误修复

- (`/redeem`) 修复小写兑换码未计算为已兑换的问题。
- (`/characters genshin`) 修复文字位置问题。
- (`/characters genshin`) 修复某些角色图片样式不同的问题。
- (`/profile hsr`) 修复样式 2 中光锥名称的字体问题。

## v1.16.7

### 新功能

- 新增阿拉伯语支持。
- (`/challenge genshin`) 新增「幽境危战」卡片生成。
- (`/profile zzz`) 为样式 4 的「闪能自动累积」新增缩写。

### 优化

- (`/accounts`) 获取帐号时显示一个页面。
- (`/accounts`) 更新米游社登录的 APK 文件 URL。
- (`/accounts`) 新增用于添加米游社帐号的 aaid 输入字段。
- 利用多个 CPU 核心加快图片生成速度。
- 图片中的文字位置更精确。

### 问题修复

- (`/profile zzz`) 修复仪玄在样式 1 中的图片位置。
- (`/profile zzz`) 修复样式 4 中「穿透值」数值未被翻译的问题。
- (`/search`) 停用深境螺旋分类。
- (`/search`) 修复驱动盘分类没有自动完成选项的问题。

## v1.16.6

### 新功能

- (`/profile zzz`) 新增 ZZZ 2.0 新角色卡片数据。

- (`/profile zzz`) 新增对命破代理人和贯穿力数值的支持。

- (`/gacha-log import`) 处理 authkey 异常。

- 新增可关闭的周年庆公告。

### 优化

- (`/profile zzz`) 移除背景代理人名称中的空格。

### 问题修复

- (`/characters genshin`) 处理无属性角色的问题。

- (`/challenge genshin theater`) 处理无效角色 ID 的问题。

## v1.16.5

### 新功能

- (`/profile hsr`) 新增 v3.3 新角色卡片数据。
- (`/profile hsr`) 新增对忆念命途角色使用 StarRailCard 模板的支持。
- (`/profile`) 处理 Enka Network API 请求超时错误。
- (`/search`) 启用「未发布内容」搜索分类。

### 问题修复

- (`/redeem`) 移除指令中的 'user' 参数。
- (`/mimo`) 移除自动 mimo 任务嵌入中的 UID 模糊处理。
- (`/upload`) 处理过大的图片文件。
- (`/search`) 修复角色和光锥属性计算公式错误的问题。
- (`/accounts`) 修复当用户拥有超过 25 个账户时「下一页」选项无法正常工作的问题。

## v1.16.4

### 新功能

- (`/profile genshin`) 支持无元素旅行者。
- 添加印地语字体。

### 优化

- (`/profile`) 移除角色数据缓存。
- 为抽卡记录过滤器添加约束条件。

### 问题修复

- (`/events`) 修复无法找到卡池公告的问题。
- (`/challenge genshin theater`) 修复幻想真境剧诗数据不显示的问题。
- (`/profile`) 修复与 Enka Network 面板的兼容性问题。
- (`/mimo`) 修复米游社用户能够访问该命令的问题。
- (`/notes`) 进行实时便笺检查时忽略游戏维护错误。
- (`/lb view`) 移除崩坏3的成就排行榜。
- (`/farm reminder`) 修复物品名称显示为"..."的问题。

## v1.16.3

### 新功能

- (`/profile zzz`) 新增薇薇安和雨果的卡片数据。
- 新增葡萄牙语 (巴西) 翻译。
- 新增日语翻译。

### 优化

- (`/profile zzz`) 调整了部分角色的图片位置。
- (`/profile zzz`) 改善了卡片模板的图片层级。

### 问题修复

- (`/notes`) 修复了质变仪通知无法正常运作的问题。
- (`/gacha-log upload`) 修复了某些 ZZZ 导入方法导致的错误物品稀有度。

## v1.16.2

### 新功能

- (`/profile hsr`) 新增遐蝶和那刻夏的卡片数据。

### 问题修复

- (`/profile zzz`) 修复波可娜的图片在卡片样式 2 中位置错误的问题。
- (`/build genshin`) 修复用户应用中圣遗物位置表情符号显示错误的问题。

## v1.16.1

### 新功能

- (`/gacha-log upload`) 新增对 [Starward 启动器](https://github.com/Scighost/Starward) 的绝区零部分导入抽卡记录的支持。
- (`/redeem`) 新增通知设置。
- (`/accounts`) 新增获取 aaid 的说明，方便用户添加米游社账号。
- 新增「隐藏 UI」按钮，适用于按钮数量较多的指令。

### 优化

- (`/search`) 移除「未发布内容」分类，详情请参见[这条消息](https://discord.com/channels/1000727526194298910/1042428379120545873/1346411349999357973)。
- (`/characters`) 允许在筛选器中不选择任何项目。
- 提升自动任务的性能。

### 问题修复

修复了多个问题，详情请查阅[完整更新日志](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.1)。

## v1.16.0  

[给技术宅们](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.0)  

### 新增功能  

- (`/profile`) 在卡片设置中新增模板预览。  
- (`/profile`) 在卡片模板下拉菜单中显示自定义图片的可用性。  
- (`/notes`) 将《星穹铁道》开拓力上限提升至 300。  
- (`/notes`) 新增「打开游戏」按钮。  
- (`/search zzz`) 新增核心技能等级选择器。  
- (`/gacha-log import`) 导入祈愿记录时，对比输入的 UID 与当前账号的 UID。  
- 自动根据 Discord 客户端的语言设置新用户的语言。  

### 优化  

- (`/redeem`) 改进用户体验，修复兑换已兑换礼包码时无响应的问题。  
- (`/gacha-log`) 设置账号参数为必填，避免混淆。  
- 为「缺少权限」和「消息被 AutoMod 阻止」的错误提供更明确的提示。  
- 简化账号设置过程中的提示文字。  

### 问题修复  

修复了多个错误并进行了一些改进。  

## v1.15.7  

### 新增功能  

- (`/web-events`) 新增命令来查看正在进行中的网页活动，并设置通知器以提醒您有新活动。  
- (`/notes`) 为《绝区零》（ZZZ）新增悬赏委托和 Ridu 每周点数通知器。  
- (`/about`) 新增更新日志按钮。  

### 优化  

- (`/gacha-log view`) 修复缓存问题，提升祈愿记录页面的性能。  
- (`/about`) 移除最新 Git 变更的显示。  
- (`/mimo`) 在自动购买时，将旅行伙伴 Mimo 商店物品按照价格从高到低排序。  
- 改进其他语言的本地化。

### 问题修复  

- (`/characters genshin`) 修复因无属性旅行者导致的 `KeyError` 问题。  
- (`/characters genshin`) 修复神里绫华天赋等级显示错误的问题。  
- (`/stats`) 修复 ZZZ 中「未找到记录卡片」的错误。  
- (`/build genshin`) 修复「没有可绘制的阻止列表」的错误。  
- (`/gacha-log view`) 修复错误的 50/50 胜率计算。  
- (`/gacha-log view`) 修复 Web 应用中的 422 验证错误。  
- (`/gacha-log view`) 处理无效的大小输入。  
- (`/gacha-log import`) 处理导入祈愿记录时的无效卡池类型问题。  
- (`/gacha-log import`) 修复 UIGF 导入功能。  
- (`/mimo`) 在发送通知前确认任务完成状态。  
- (`/mimo`) 在完成任务之间新增休眠间隔以避免触发限速。  
- (`/mimo`) 移除任务名称中的 HTML 标签。  
- (`/mimo`) 修复购买物品后的错误。  
- (`/profile`) 修复不同游戏的卡片设置混合的问题。  
- (`/profile genshin`) 修复队伍卡片中显示多余天赋的问题。  
- (`/profile genshin`) 修复与 Mavuika 相关的验证错误。  
- (`/search`) 修复 W-engine 精炼选择器未更新所选值的问题。  
- (`/notes`) 修复《崩坏3》中的验证错误。  
- (`/challenge zzz assault`) 修复增益图标未显示的问题。  

## v1.15.6

### 新增功能

- (`/mimo`) 新增旅行 Mimo 对于原神的支持（活动在撰写时已经结束）。
- (`/mimo`) 新增自动抽奖功能。
- (`/challenge zzz`) 新增对于「危局强袭战」游戏模式的支持。
- (`/profile hsr`) 新增卡片样式 2。
- (`/notes`) 新增对于绝区零悬赏委托及丽都周记任务信息的显示。

## 优化

- (`/check-in`) 减少重复的签到 API 请求。

## 问题修复

- (`/mimo`) 修复当没有完成任何任务或获取任何积分时仍发送通知的问题。
- (`/mimo`) 修复有价值物品判断方式的问题。
- (`/mimo`) 处理 -510001 错误。
- (`/mimo`) 修复在星穹铁道中，有价值物品被误认为装饰品的问题。
- (`/mimo`) 当达到上限时禁用抽奖按钮。
- (`/challenge zzz`) 修复卡片中错误的邦布图片。
- (`/events`) 修复深渊进度错误的问题。
- (`/gacha-log view`) 修复错误的「距离上一稀有度的抽取次数」。
- 修复静态图片文件夹创建逻辑。

## v1.15.5  

### 新增功能  

- (`/mimo`) 自动完成需要在帖子下留言的任务。  
- (`/mimo`) 自动完成需要关注主题的任务。  
- (`/mimo`) 新增抽奖功能。  
- (`/mimo`) 新增通知设置。  
- (`/profile zzz`) 新增图片设置，允许在构建卡中使用「Mindscape 3」的美术图。  
- (`/profile zzz`) 新增春政 (Harumasa) 和雅 (Miyabi) 卡片数据。  
- (`/search`) 在某些公会中隐藏「未发布内容」分类。  

### 优化  

- (`/mimo`) 在某些任务中显示任务进度。  
- (`/mimo`) 在通知中显示已完成任务的名称。  
- (`/mimo`) 提升自动任务执行性能。  
- (`/challenge zzz shiyu`) 更新卡片布局。  
- (`/challenge zzz shiyu`) 避免重复抓取代理人数据。  
- 在错误嵌入的页脚显示 Discord 服务器邀请链接。  
- 在错误情况下解除项目加载状态。  
- 在切换按钮上新增开/关标签。  
- 改进代理 API 请求逻辑。  
- 改善自动任务的错误处理逻辑。  

### 问题修复  

- (`/mimo`) 在兑换 Mimo 奖励礼包码后新增休眠间隔。  
- (`/mimo`) 修复任务清单中遗漏的任务。  
- (`/mimo`) 修复留言任务未被完成的问题。  
- (`/mimo`) 修复当没有完成任何任务时仍发送通知的问题。  
- (`/mimo`) 自动完成中仅显示 HoYoLAB 账号。  
- (`/mimo`) 修复自动任务中的 `QuerySetError` 问题。  
- (`/mimo`) 修复帖子留言未被删除的问题。  
- (`/mimo`) 处理旅行伙伴 Mimo 不可用于某些游戏的情况。  
- (`/profile zzz`) 修复副属性高亮未显示在卡片上的问题。  
- (`/profile zzz`) 修复代理人被误认为已缓存的问题。  
- (`/characters zzz`) 修复代理人总数显示错误的问题。  
- (`/gacha-log upload`) 修复 zzz.rng.moe 导入时的问题。  
- (`/redeem`) 修复 Miyoushe 账号出现在账号自动完成选项中的问题。  
- (`/build genshin`) 处理某些角色缺失使用率的情况。  
- (`/events`) 修复 HSR 未来卡池未显示为「尚未发布」的问题。  
- 适配新的 ZenlessData 键值。  
- 修复 Hakushin API 的相关问题。  
- 捕获 `dm_user` 方法中的一般异常情况。  

## v1.15.4  

### 新增功能  

- (`/build genshin`) 显示角色队伍配置的相关信息。  
- (`/mimo`) 新增指令来管理旅行 Mimo。  

### 优化  

- (`/build genshin`) 改善卡片设计。  
- (`/notes`) 使用事件日历 API 检查位面分裂事件。  

### 问题修复  

- (`/build genshin`) 修复一些 UI 问题。  
- (`/events`) 修复导致指令无法使用的问题。  
- (`/gacha-log upload`) 修复使用 UIGF 数据时的 `ValidationError` 问题。  
- (`/gacha-log upload`) 修复 UIGF 版本低于 3.0 时的 `KeyError` 问题。  
- (`/search`) 修复重复的自动完成选项问题。  

## v1.15.3  

先前版本中的错误代码导致部分用户在登录时看到「请求次数过多」错误，请参阅[本文](./too-many-requests.md) 以了解更多信息。

### 新增功能  

- (`/profile zzz`) 新增选择器，可选择想要突出的副属性。  
- (`/profile hsr`) 新增 Fugue 和 Sunday 卡片数据。  

### 优化  

- (`/redeem`) 使用礼包码本身掩盖兑换链接。  
- (`/challenge genshin theater`, `/challenge genshin abyss`) 在卡片中显示旅行者的元素属性。  
- (`/accounts`) 对「请求过多」错误显示自定义错误信息。  

### 问题修复  

- 修复指令未被翻译为其他语言的问题。  
- 修复超时的弹窗未正确关闭的问题。  
- 修复 API 重试逻辑与错误处理逻辑。  
- 修复某些指令的 `ValueError` 问题。  
- 修复弹窗超时时间过短的问题。  
- 处理 Web 服务器重定向端点的 `KeyError` 问题。  
- (`/profile`) 处理从 Enka Network API 获取数据时的 `EnkaAPIError` 问题。  
- (`/profile`) 更优雅地处理 Enka Network API 网关超时错误。  
- (`/profile`) 修复生成 AI 图像时的 `BadRequestError` 问题。  
- (`/upload`) 修复上传图片时的 `BadRequestError` 问题。  

## v1.15.2 及以下

先前版本的更新日志写在 [Discord 服务器](https://link.seria.moe/hb-dc) 内的 #更新 频道中。
