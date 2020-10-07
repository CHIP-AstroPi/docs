[**Astropi**](https://astro-pi.org/) Phase 1: Design

<!-- omit in toc -->
# /* NOME TEAM */  

- [1. Introduction](#1-introduction)
- [2. Technical](#2-technical)
  - [2.1. Real-time elaboration](#21-real-time-elaboration)
  - [2.2. Post-Izzy elaboration](#22-post-izzy-elaboration)
  - [2.3. Satellite imagery parsing](#23-satellite-imagery-parsing)
- [3. Expected results](#3-expected-results)
- [4. References](#4-references)

## 1. Introduction
Global warming is the main actor of many environmental disasters, such as sea-level rise, frequent wildfires resulting in heavy deforestation, drought and desertification, glacier retreat, etc.

We'll analyze the pysical effects that such disasters had in the past over the environmet and compare them with the change in global temperature over the years.

The final objective is to create an algorithm able to predict the impact that various scenarios of global heating will have to the environment.
 
## 2. Technical
The technical procedure is made of two phases: 
- Real-time elaboration, on the "Izzy" pc
- Post-Izzy elaboration

> Graphic representation of the tasks separation<br>
![](./img/tasks_separation.png)


### 2.1. Real-time elaboration
We'll collect data mainly from the near-infrared camera. We plan to [parse](#23-satellite-imagery-parsing) in real-time the collected imagery and store them with the extracted data.

### 2.2. Post-Izzy elaboration
We'll run the parsing process on historic satellite imagery and use the obtained data, with the ones coming from the "Izzy" real-time elaboration, to elaborate a statistic model able to "predict" the future impact.

### 2.3. Satellite imagery parsing
Our program will run various classification and detection algorithms on the captured images.
Some example of algorithm we expect to apply on near-infrared imagery:

|            Algorithm | "Element" detected  | References                |
| -------------------: | :-----------------: | ------------------------- |
|                 NDVI | forests and deserts |
|                 NDWI |  rivers and lakes   |
| Coastlines detection |     coastlines      | [10.15244/pjoes/64160][1] |

If no IR historic dataset can be found we'll detect elements with custom ML models.

## 3. Expected results

## 4. References
[1]: [Maras, Erdem & Caniberk, Mustafa & Maras, Hadi. (2016). Automatic Coastline Detection Using Image Enhancement and Segmentation Algorithms. Polish Journal of Environmental Studies.](https://www.researchgate.net/publication/308125872_Automatic_Coastline_Detection_Using_Image_Enhancement_and_Segmentation_Algorithms)