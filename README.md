# ModFGO

> ~~修改有风险，使用需谨慎。~~  
> 号没了别怪我

## 如何使用

- 这是一个`Magisk`模块，需要启用`zygisk`功能
- 如果没听说过`Magisk`，那么可以关闭页面了

## 修改了什么

### Battle

- 从者替换
- 宝具无释放限制
- 移除助战刷新时间和确认对话框
- 技能等级固定 10
- 宝具等级固定 5
- 掉落物提示
- 所有攻击暴击
- 小兵去质器（一半敌人 hp/2）
- 自动选卡
- 战斗时 4 倍速
- 宝具跳过按钮

### Misc

- 移除 Debug 输出日志
- 移除证书校验
- 禁止首次进入时播放动画
- 窗口动画快进 30%

### MasterDataReplace && FigureReplace

- 立绘和文本替换，`FGOAssetReplace`拆分自这里

## 变更

- 移除 HP&ATK \* 2
- 移除攻击暴击
- 移除功能菜单
- 从者默认添加被动技能`黑暗之衣`
- 更新`Il2CppApi`以取代固定地址偏移（说人话就是不随游戏版本更新而失效，而随引擎版本更新失效）

## 说明

### 从者替换

可以完全自定义修改队伍中前三个从者。需要自己配置好`Servants.json`并放置在新建目录`/sdcard/Android/data/com.placeholder/files/Mod`，可以参考我的例子。数据可以在[这个网站](https://apps.atlasacademy.io/db/CN/servants)找到。

### 配置

下载`ModConfig.json`放置在`/sdcard/Android/data/com.placeholder/files/Mod`即可，部分功能可以在菜单中配置。

```json
{
  "EnableReplaceSvt": true,
  "EnableAutoSelectCard": true,
  "CardColor": 2,
  "SvtId": [2500700, 500800, 500800]
}
```

完整的文件树：

```
/sdcard/Android/data/com.placeholder/files/Mod/:
|---ModConfig.json
|---Servants.json
```

### 其他

大概就这些 ᕕ( ᐛ )ᕗ
