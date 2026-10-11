# Y111Plugins

FFXIV（国服 Dalamud）自定义插件源。

## 添加插件源

游戏内 `/xlsettings` → `Experimental` → `Custom Plugin Repositories`，添加下面的地址：

```
https://raw.githubusercontent.com/yyyyyyyy8/Y111Plugins/main/pluginmaster.json
```

保存后打开插件安装器，搜索 **Map Gather** 即可安装 / 更新。

## 插件列表

### Map Gather

自动挖藏宝图，上架。

- 按角色列表顺序自动挖藏宝图，可拖拽调整顺序
- 自动回家、传唤铃选雇员，按本服最低价减降价上架
- 支持「指定模式」与「按当前服务器最高价藏宝图」模式
- 每个角色可单独指定藏宝图与采集职业（采矿工 / 园艺工）
- 支持坐骑选择、`/stylist` 幻化、雇员已有藏宝图改价、挖图额度与背包满检查

依赖：

| 插件 | 是否必需 | 说明 |
| --- | --- | --- |
| Lifestream | 必需 | 跨图传送、`/li auto` 回城 |
| vnavmesh | 必需 | 寻路 / 飞行 |
| DailyRoutines | 推荐 | 市场最低价查询（缺少时用历史成交价兜底） |
| Stylist | 可选 | `/stylist gatherer` 幻化预设 |

## 文件说明

- `pluginmaster.json`：Dalamud 自定义插件源描述文件
- `MapGather/`：本插件的最新构建产物（`MapGather.dll` / `MapGather.json` / `MapGather.deps.json`）
- 也可以直接从 [Releases](../../releases/latest) 下载 `MapGather.zip`

## 版本

| 插件 | 内部名 | 版本 |
| --- | --- | --- |
| Map Gather | MapGather | 1.2 |
