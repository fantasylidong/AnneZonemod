# 此项目已archieve，不再维护，有需要的请使用 https://github.com/fantasylidong/CompetitiveWithAnne

# AnneZonemod

> 使用了Zonemod改图的Anne插件包，所有对抗插件都已更新到最新版本，Anne核心和原test分支，和电信服保持一致

## 项目结构介绍

本项目一共分为3个分支

main, mysql, Nomysql

### main分支

main分支只会有插件和源码，main分支更新稳定后会向mysql分支和Nomysql分支进行同步

### mysql分支

mysql分支为电信服当前使用代码，有数据库，但是配置文件默认的数据库是不对外开放的，你如果用这个分支，你需要自己根据此分支的mysql创表文件创建属于自己的数据库，而且需要在addons/configs/database.cfg文件中将数据库相关插件配置更改为你自己服务器的插件配置

### nomysql分支

顾名思义啊，这个分支就是没有数据库，如果你只打算开一个服务器，建议下载这个版本

## 插件包结构介绍

本插件包和原来的AnneServer插件包或者Sir的对抗插件包不一样。

你如果想添加自己的插件，去cfg/cfgogl/ownplugins.cfg这个文件中添加新加入插件的位置，这个文件基本上是在最后面被执行，所以要注意加载顺序。

如果想单独给某个配置添加新插件，去cfg/cfgogl/想修改的配置/shared_plugins.cfg内添加你想新添加的插件。

## 插件更新Log

### 9月插件

- ai_hunter_new 放宽了点垂直高度限制

- ai_charger_2 稍微修改了点属性，让牛连跳不那么激进，以此增加牛冲锋的概率

- ai_tank_2 修复了tank位于生还者下方可能使用纵云梯空中再次向上加速的情况，降低了tank跳砖的高度，增加了梯子检测方法，在距离tank 150单位如果能检测到梯子，tank将不会锁定视角，大大降低tank被梯子卡住的问题

- ai_hardsi_2 增加了tank低于50速的时，检测面前是否有门的情况，让克被门卡住的可能性大大降低

- text插件增加了版本控制能力，将切换模式乱七八杂的text作了整合，也方便投票某些功能时，老板text插件可能没有，比如多人运动

- hud插件适配新版leftdhooks

- veteran 时长控制插件已经稳定，删除debug信息

- 刷特插件稍微修改，适配新版left4dhooks，并增加特感不能和玩家不能在同一个nav区域，稍微增加分散度

- skill_detect 修复连跳装逼少了参数，修复

- pickup插件同步上游更新

- AnneTankTeleport修复传送tank后tank依旧往卡住点走的问题，且增加所有人都在tank flow前时，不触发跑男的惩罚（用于克卡住生还者前推的情况）

- 女巫派对增加一个生还者秒妹失败倒地后自动再生成一只witch的功能

- 修复了2、3人运动无法启用的问题

- 增加特感生成最低距离投票的功能（降低坐牢情况）

- Stripper修补了c2c5大部分卡克点，增加坐牢体验

## 插件包Changelog

2022-7-15 插件包初始发布
2022-7-21 2022-7月插件最终发布

2022-9-14 9月插件包更新
