# MGPK-TC
## Dataset
The processed Manhattan dataset is available at the following link：https://pan.baidu.com/s/1SnxSQLRWSCEh9um6pe5FpA?pwd=0714 

## Dataset file description
#### z_scored_temporal_data.h5:
数据包含：涵盖2017曼哈顿地区每小时的气温、气压、湿度、能见度、露点温度、风速、海平面气压，以及每种类型的POI在该时刻的时间知识。已经过Z-scored归一化处理

The data contains: hourly temperatures, barometric pressure, humidity, visibility, dew point temperature, wind speed, sea level barometric pressure covering the 2017 Manhattan area, and temporal knowledge of each type of POI at that moment in time. It has been Z-scored normalized.

#### z_scored_spatial_data.h5：
数据包含：曼哈顿地区每条道路的道路ID、长度、宽度和道路类型(如桥梁、普通公路)、每种类型的POI数量以及空间知识。已经过Z-scored归一化处理

The data contains: road ID, length, width and road type (e.g., bridge, general highway), number of POIs of each type, and spatial knowledge for each road in Manhattan. It has been Z-scored normalized.

#### road_network.gpickle：
数据包含：曼哈顿地区道路图

The data contains: Road map of Manhattan area.

#### 2017_flow_MTH.h5
数据包含：2017年曼哈顿地区每条道路每小时的车流量

The data contains: contains: hourly traffic volume on every roadway in Manhattan in 2017.

#### 07_12_accident.h5
数据包含：2017年曼哈顿地区7至12月交通事故数。已生成了负样本

The data contains: number of traffic accidents from July to December 2017 in the Manhattan area. A negative sample has been generated.

## Data soures
The data sources for this dataset include:
- Road network data: Downloaded from NYC website(https://data.cityofnewyork.us/City-Government/NYC-Street-Centerline-CSCL-/exjm-f27b).
- Traffic crash data: Downloaded from NYC website(https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95/about_data).
- Traffic flow volume data: This dataset uses taxi trip records as aproxy for traffic flow volume,obtainedby searching for the keyword "2017 Taxi Trip Data" on NYC website(https://opendata.cityofnewyork.us).
- POI data: A total of 20 datasets of various sizes are obtained by searching keywords such as "points of interest", "businesses", “restaurants”, and "schools" on the NYC website((https://opendata.cityofnewyork.us)) and merged by their categories.
- Weather data: This dataset collects hourly updated meteorological information from https://rp5.ru.

