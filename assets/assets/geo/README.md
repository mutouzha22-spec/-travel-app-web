# 离线地点搜索数据

- `china_places.json` 由 `modood/Administrative-divisions-of-China` 的 `pca-code.json` 精简生成，包含省、市、区县三级名称与所属关系。原项目采用 WTFPL 许可，数据快照更新至 2023 年。
- `world_countries.json` 由 `mledoze/countries` 精简生成，只保留中文名、英文名、两位代码与代表坐标。原数据库采用 ODbL-1.0 许可。
- 运行 `tools/generate_location_catalog.py` 可重新生成这两份资源。
- App 不使用这些数据绘制政治地图；它们只用于离线搜索、地点归类与代表位置。
