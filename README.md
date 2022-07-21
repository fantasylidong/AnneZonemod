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

## 插件包Changelog

2022-7-15 插件包初始发布
2022-7-21 2022-7月插件最终发布
