# Nordics road traffic data

The purpose of this repository is to include the source code to produce an Origin-Destination matrix for the nordic countries.

## Installation

Developed and tested in
```sh
Python 3.7.4
```
Probably will work with almost any version of Python 3

1. (Optional) Create a Python virtual environment before starting.

2. Install numpy since we need it to link and compile the C++ code.
```sh
pip install -r requirements.txt
```

## Files in this repository

- `road_traffic_data.ipynb`: Python notebook with the source code necessary to produce the O-D matrix.
- `fin_province_info.json`: Auxiliary file used by the Python notebook to get the results.
- `traffic_fin.csv`: Basic information of the sensors located on the border of Finland. The file was elaborated manually.
- `traffic_nor.csv`: Basic information of the sensors located on the border of Norway. The file was elaborated manually.
- `/map_data`: Folder with maps for the nordic regions.

## Sources of information

- [Vegvesen](https://www.vegvesen.no/trafikkdata/start/kart?lat=64.85003449662187&lon=19.157035747455456&trafikanttype=vehicle&trpids=49453V930259&zoom=3). Traffic road authority in Norway. [API](https://www.vegvesen.no/trafikkdata/start/om-api)
- [Fintraffic](https://liikennetilanne.fintraffic.fi/kartta?lang=fi). Traffic road authority in Finland. [API](https://www.digitraffic.fi/en/road-traffic/#restjson--apis)
- [Trafikverket](https://www.trafikverket.se/trafikinformation/vag/?TrafficType=personalTraffic&map=1%2F363003.87%2F6892656.39%2F&Layers=TrafficSituation%2bRoadCondition%2b). Traffic road authority in Sweden. [API](https://api.trafikinfo.trafikverket.se/)
