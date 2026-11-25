# NYC Evictions 2019–2020：数据来源与文件说明

本目录保存课程项目所需的原始来源文件，以及便于后续 R 分析的轻量版本。原始来源文件保留用于复现；分析版省去了不需要的个人/案件字段。

## 文件

- `evictions_2019_2020.csv`：NYC Open Data 的原始记录筛选版，执行日期为 2019-01-01 至 2020-12-31，共 22,135 条（2019 年 18,713 条；2020 年 3,422 条，含住宅与商业）。
- `evictions_residential_2019_2020.csv`：仅住宅记录，共 20,100 条（2019 年 17,036 条；2020 年 3,064 条）。保留执行日期、类别、坐标、行政区和 BBL 等分析字段；移除了公寓号、执法官姓名、法院案号和完整地址。
- `pluto_20v1_csv.zip`：NYC Department of City Planning 的 PLUTO 20v1 属性表、数据字典和说明文件。此压缩包是表格属性数据，不含 MapPLUTO 地块几何。
- `pluto_20v1_housing_fields.csv.gz`：从 PLUTO 20v1 表中抽出的 24 个住房与地块字段，共 859,172 个唯一 BBL，可与驱逐数据按 BBL 连接。
- `tl_2019_36_tract.zip`：美国人口普查局 2019 年纽约州 Census tract 边界原始压缩包。
- `tiger2019_extract/`：上述 ZIP 的解压副本。
- `nyc_tracts_2019.gpkg`：从 2019 TIGER 边界中筛选纽约市五个县（005、047、061、081、085）的 2,167 个 tract，并转换为 EPSG:2263。`GEOID` 为 11 位字符，可与 ACS 表连接。
- `acs_2015_2019_nyc_tracts.csv`：ACS 2015–2019 五年期 tract 估计值及相应误差范围（MOE），共 2,167 个 NYC tract。包括租户家庭数、租金负担、贫困、种族/族裔和家庭收入中位数；同时提供计算好的贫困率及租金收入负担达到 30% 以上的比例。
- `20195ny*.zip`、`g20195ny.csv`、`g20195ny.txt`、`acs_2019_sequence_lookup.txt`：ACS Summary File 的原始序列和地理标识文件，用于复现 ACS CSV。此方法无需 Census API key。

## 来源

- Evictions：NYC Open Data dataset 6z8x-wfk4，Department of Investigation。下载时按 `executed_date` 筛选 2019–2020 年。https://data.cityofnewyork.us/d/6z8x-wfk4
- ACS 2015–2019：U.S. Census Bureau 2019 ACS 5-year Summary File，表 B03002、B17001、B19013、B25003、B25070；按 NYC 五县和 Census tract geography 汇编。说明页：https://www.census.gov/programs-surveys/acs/data/summary-file/sequence-based.2019.html
- TIGER/Line 2019 tract 边界：https://www2.census.gov/geo/tiger/TIGER2019/TRACT/tl_2019_36_tract.zip
- PLUTO 20v1：https://www.nyc.gov/assets/planning/download/zip/data-maps/open-data/nyc_pluto_20v1_csv.zip

## 初步核对

- ACS 表与 NYC tract 边界各有 2,167 条，GEOID 完全匹配。
- 住宅驱逐记录中有 1,384 条缺少经纬度；1,411 条缺少 BBL。按 BBL 与 PLUTO 连接后，18,610 条住宅事件匹配到 PLUTO，后续空间点分析和 BBL 分析应分别报告可用样本量。
- 当前 NYC Open Data 下载按字段筛选后，2020 年有 3,064 条住宅记录，2019 年有 17,036 条；NYC Office of Civil Justice 年度报告分别列 3,035 和 16,996。两套统计尚未完全对齐，正式报告前应检查重复记录、更新版本和计数口径，并把差异作为数据评估内容。
- ACS 的收入、租金负担和贫困数据是五年期估计，不是某个单独年份的实测值。租金负担比例按 B25070 的 30% 及以上各档估计值之和，除以总数扣除“未计算”记录后计算。
- PLUTO 表是地块属性而非建筑级租户记录；其 `UnitsRes` 是地块住宅单元估计，不代表该地块实际租户户数。避免将其直接当作精确租户分母。
