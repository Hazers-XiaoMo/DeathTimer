# DeathTimer

A plugin allows you to customize the behavior after player's death timer over.

Support PlaceHolderAPI.

## Commands

+ `/dt`or`/deathtimer`
    + `/dt reload`
    + `/dt revive`
    + `/dt clear <player>`

## Configs

### config.yml

```yml
#语言文件（在locals目录下）
lang: "zh_CN"
#死亡后计时
cooldown: 10
#时间单位: HOUR MINUTE SECOND
unit: "SECOND"
```

### locals/zh_CN.yml

```yml
command:
  without_permission: "[DeathTimer] §c你没有权限!"
  non_console: "[DeathTimer] §c控制台无法使用此命令!"
  non_player: "[DeathTimer] §c找不到此玩家!"
  wrong_usage: "[DeathTimer] 命令好像输错了! 请输入 /dt help 了解所有命令"
  reload:
    reloaded: "[DeathTimer] 插件已重置"
  revive:
    revived: "[DeathTimer] 已复活"
    time_left: "[DeathTimer] §c时候未到..."
  clear:
    cleared: "[DeathTimer] 已清除冷却时间"
    usage: "[DeathTimer] /dt clear <玩家名称>"
  help: |
    Asyncraft团队——DeathTimer死亡计时器：在死亡之后做点什么!
    -----------------------------------------------------
    §e/dt §f或 §e/dt help §f: 获得DeathTimer的帮助
    §e/dt reload §f: 重载插件
    §e/dt revive §f: 复活
    §e/dt clear <玩家名称> §f: 清空某玩家的死亡冷却

actionbar:
  cooldown:
    # elapse: ""
    end: "§a输入 /dt revive 就地复活"

debug:
  loaded: "插件已加载"
  disabled: "插件已卸载"
  config_error: "配置文件错误,卸载插件..."
  placeholder_api:
    hooked: "PlaceholderAPI前置已接入"
    not_found: "PlaceholderAPI前置未找到"
```

### dead.yml

is not a config file  
just use as a data file

DO NOT EDIT IT

## LICENSE

MIT