# 离线地点搜索数据

- `china_places.json` 由 `modood/Administrative-divisions-of-China` 的 `pca-code.json` 精简生成，包含省、市、区县三级名称与所属关系。原项目采用 WTFPL 许可，数据快照更新至 2023 年。
- `world_countries.json` 由 `mledoze/countries` 精简生成，只保留中文名、英文名、两位代码与代表坐标。原数据库采用 ODbL-1.0 许可。
- `china_destinations.json` 合并文化和旅游部国家 5A 景区与国家级旅游度假区、四川省文旅厅 A 级景区名录、Wikidata CC0 坐标、OpenStreetMap ODbL 坐标，以及人工核验的重点目的地。它只保存搜索所需的名称、别名、归属、坐标和排序信息。
- 运行 `tools/generate_location_catalog.py` 可重新生成这三份资源。下载过程使用 `tmp/location_catalog_cache` 缓存，缓存不进入源码存档。
- App 不使用这些数据绘制政治地图；它们只用于离线搜索、地点归类与代表位置。
