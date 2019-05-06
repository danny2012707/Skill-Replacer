# skill-replacer
Replace your skill and make this TERA great again<br>
<br>
rs on/off to enanbe and disable<br>
rs reload for reload config after edit<br>

# Issue
It's will ghost when you out of mana<br>
It's not full macros so don't hope for autoRepeat function<br>

https://github.com/OverImagine/Skill-Replacer/

Skill-Replacer 忍者火焰术 - 无查克拉消耗(即 无限喷火) 等...
======

# 功能简介

- Lv.65 忍者 原始 [标枪连射VIII] 技能被替换为 [火焰术VII]

- 拳师觉醒技能 颱風連打 无限释放

- config.json 中默认配置了更多其他职业的技能 没时间全部测试...

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/01.png)

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/02.png)

/8频道 键入命令 | 效果说明
--- | ---
sr on | 开启模组
sr off | 关闭模组

------

bug修复 - 支持客户端 v81.03

------

# 由于此JavaScript经过作者混淆加密 所以反混淆之后只能修改编辑到部分代码

首先我们来看一下报错提示

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/03.png)

很显然只是一个def的版本使用错误导致

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/04.png)

- S_LOGIN.12.def 的使用区间为 v77 到 v81

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/05.png)

- S_LOGIN.13.def 可应用于 v81 以上版本

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/06.png)

复制整个index.js代码至格式化功能网页 从新排版

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/07.png)

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/08.png)

通过简易反混淆从新获取源代码(转换全文: 16进制字符串 16进制数值)

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/09.png)

注意此段代码 这样的格式是否跟这种常见的很像 (别问我为什么知道 常做mod的人一看就眼熟)

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/10.png)

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/11.png)

现在可以去源代码上修改了

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/12.png)

将

al[b('0xf8', '\x40\x28\x6f\x44')](am[b('0xf9', '\x43\x55\x46\x44')], 0xc, bd => {

去掉空格后 在index.js中查询

al[b('0xf8','\x40\x28\x6f\x44')](am[b('0xf9','\x43\x55\x46\x44')],0xc,bd=>{

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/13.png)

0xc 代表16进制数 C 转10进制即为 12

0xd 代表什么不用我多说了

![screenshot](https://github.com/zc149352394/Skill-Replacer/blob/master/screenshot/13.png)
