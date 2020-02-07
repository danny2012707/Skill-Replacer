# skill-replacer
Replace your skill and make this TERA great again<br>
<br>
rs on/off to enanbe and disable<br>
rs reload for reload config after edit<br>

# Issue
It's will ghost when you out of mana<br>
It's not full macros so don't hope for autoRepeat function<br>

https://github.com/OverImagine/Skill-Replacer/

---以上为作者留下的 说明文档---

Skill-Replacer
======

# 功能简介

一个有趣的模组, 能将[1个施法技]能替换为[另1个施法技能]

config.json 中有详细的配置[替换技能]的说明

------

/8频道 键入命令 | 效果说明
--- | ---
sr on | 开启模组
sr off | 关闭模组
sr reload | 重新载入config.json配置文档

------

举个例: 想要改忍者的[普通攻击]技能

- Job ID -->>这里填13职业的分类编号: 11

  0-warrior-双刀 1-lancer-枪骑 2-slayer-大剑

  3-berserker-斧头 4-sorcerer-魔道

  5-archer-弓箭 6-priest-祭师 7-mystic-元素

  8-reaper-飞镰 9-gunner-魔工 10-brawler-拳师

  11-ninja-忍者 12-valkyrie-月光

  查询技能表:

  1xxxx	Common	Common	Ninja	連續攻擊I	True	Side 	icon_skills.c12_meleecombo

  150732	Common	Common	Ninja	多重分身火焰術	False		icon_skills.c12_flamebreath_awaken

- Skill ID with Floor(ID/10000) -->>这里填[原始技能]头部编号(技能编号/1000): 1

- Just noted -->>这里填 文字说明信息

- Full skill id for replace -->>这里填[替换技能]完整的编号: 150732

- autoRepeat -->>这里填 true 代表[自动循环]这个技能, false 则只释放1次

------

更多职业技能参考: https://github.com/neowutran/TeraDpsMeterData/tree/master/skills skills-TW.tsv

------

提供1个编辑好的版本 config_edit.json 重命名并替换 config.json
