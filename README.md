# AirPoluionData
这里是使用爬虫于2017年在空气质量监测平台 www.aqisudy.cn 所抓取的数据。

这个 Repos 包含了一份爬虫代码，一份数据集合，一份简单的数据分析代码（使用 Python `Pandas` 进行分析）

## 数据抓取与存储
数据抓取使用 requests 与 多线程进行，以各个市级监测点的地名作为表名称，使用 `sqlite` 存储在 **dataset** 文件夹下
数据分为两个部分：3年天单位190城市监测点数据 + 5个月小时单位380监测点数据

## 数据分析
涵盖了一份简单的数据分析例程，分析结果以 `matplotlib` 导出为图片存储在 **result** 文件夹下
对数据库的分析数据存储在 `Analysis.db` 数据库中，导出结构在 `Analysis.txt` 文件内
`CityList.info` 文件包含 190 个地级市的所有监测点名称

## 其他
需要注意的是，数据和代码均是我于 2017 年抓取创建，所以无法保证数据的时效性以及完全准确性。
项目创建之后即归档，仅用作查询使用。