# Natural Tourism Knowledge Graph
*by Lucía Trillo Carreras and Marina Bueno García*

This project is created for the Knowledge Graph subject at University of Trento, using the [iTelos methodology](https://unitn-kdi-2021.github.io/unitn-kdi-2021-website/material/slides/W2.L2.M2.T4.1.iTelosPrinciples.pdf), in collaboration with [Datascientia Foundation](https://datascientiafoundation.github.io/LiveData-KGE/datasets/) and the [KnowDive Research group](http://knowdive.disi.unitn.it).


## Materials
### Code
The GitHub repository can be found [here](https://github.com/mbueno-g/KGE---Tourism-in-Trento)

### Report
The report of this project can be found by clicking [here](https://github.com/mbueno-g/KGE---Tourism-in-Trento/Documentation/report.pdf)

### Presentation slides
The presentation slides of can be found [here](https://pitch.com/v/trentino-territory-tourism-facilities-9iz672)


## Introduction

The Trentino region of Italy is incredibly rich in natural landscapes, with 3992 named mountains, 297 lakes and countless beautiful hikes throughout. As international students visiting the region for 6 months and excited to explore, the amount of information and variety of sources to learn about natural tourism was overwhelming. We did not know what points of interest could be accesible without car, and we were concerned doing very complex hikes that could be dangerous for begginers.

 To help ourselves and future visitors,  we will focus on developing a knowledge graph, which will function as a tool for connecting all neccesary natural tourism information  in Trentino.
In this project, we followed the iTelos methodology that aims for maximum flexibility in reusing both data and schemas. This goal is achieved by independently developing the data level and the schema level of an application.


## Project Purpose
The purpose of this project is to provide in a single place all the information that is available on nature tourism in the Trentino territory. To provide that service we will build a knowledge graph
(KG) that provides all the information about the natural tourism attractions such as lakes, natural parks, camp sites, waterfalls... and how to get there via bus/train/bike/taxi. This Knowledge Graph aims to provide in a single place all the information that is available on nature tourism in the 176 municipalities of the Trentino territory. 


## Project domain of interest (DoI)
The domain of interest for this project is natural tourism in the 176 municipalities of the Trentino province. There is no temporal boundary as the region receives tourism throughout the cold
(ski tourism) and hot seasons.



## Personas, Scenarios, and Competency questions
Building on the project’s main purpose outlined, this section aims to further formalize this initial purpose statement by providing scenarios and personas. These user-centered concepts represent how different users might interact with the knowledge graph. Through various scenarios and personas, we illustrate how individuals could use the knowledge graph to achieve specific goals, thus further formalizing the project’s purpose. Below, we briefly present the various personas and scenarios that were formulated.

### Personas

| Identifier | Origin               | Nature expertise | Age | Description                                                                                                                                                                                                                          |
|------------|----------------------|------------------|-----|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1          | Italy,Lombardy       | High             | 55  | Antonio is a local outdoor enthusiast, familiar with Trentino's trails, seeks challenging hikes and hidden gems. He enjoys skiing after picking it up from his business trips to the Alps. He has a car.                             |
| 2          | Italy,Toscana        | Medium           | 28  | Giulia is a young professional traveling with her boyfriend, Matio. Giulia enjoys art, history and good coffee .She is visiting Trentino for the first time, seeks diverse trails and wants detailed information. Matio loves biking |
| 3          | Italy,Toscana        | Low              | 27  | Mario is a young professional traveling with her wife, Julia, and children by car. A tourist with minimal nature experience, wants picturesque spots, child-friendly and needs guidance on transportation options.                   |
| 4          | Czech Republic, Brno | High             | 23  | Veronica is doing her Erasmus for 6 months in Trento and wants to thoroughly explore everything the region has to offer.  Time is not a limitation on her travels, but money is. She's into climbing and doing challeging hikes.     |
| 5          | Germany, Munich      | Low              | 32  | Dalim is a novice hiker on a weekend vacation, interested in scenic spots and gentle walks, prefers easily accessible locations.                                                                                                     |
| 6          | Poland, Krakow       | Medium           | 26  | Tymoteusz is a nature lover, keen on exploring Trentino's beauty at a relaxed pace, enjoys both hills and mountains.  He loves swimming and beautiful rocks                                                                          |

### Scenarios

| Identifier | Title                      | Description                                                                                                      |
|------------|----------------------------|------------------------------------------------------------------------------------------------------------------|
| 1          | Challenging Adventure      | A plan to enjoy adventurous hike in Trentino's mountains, looking for challenging trails and stunning views.     |
| 2          | Moderate Nature Experience | An exploration of Trentino's hills, combining nature with cultural experiences, seeking easy to moderate trails. |
| 3          | Relaxing Scenic Strolls    | Gentle walks around picturesque locations in Trentino, focusing on easy trails and accessible spots.             |


### Competency questions
Based on 6 Personas and 3 Scenarios, we defined 20 competency questions

| Identifier | Competency questions                                                                                             | Scenarios | Personas |
|------------|------------------------------------------------------------------------------------------------------------------|-----------|----------|
| 1          | What are the top three challenging trails in Trentino?                                                           | 1         | 1,4      |
| 2          | Can you suggest a moderate hill trail with historical points of interest?                                        | 0         | 0        |
| 2          | Can you suggest a moderate hill trail with altitude lower than 2000 m?                                           | 2         | 2        |
| 3          | Are there any beginner-friendly walks with scenic views near Trento?                                             | 0         | 0        |
| 3          | Are there any beginner-friendly walks near Trento?                                                               | 3         | 3,5      |
| 4          | How can I reach the Dolomites?                                                                                   | 1,2       | 1,2,4,6  |
| 5          | Can you provide a list of must-visit lakes in the Trentino region?                                               | 3         | 3,6      |
| 6          | Who can I ask for general touristic info in each comune?                                                         | 1,2,3     | 2,3,5,6  |
| 7          | Can you recommend a nature guide/tours or group?                                                                 | 3         | 2,3,4    |
| 7          | Who can I ask for information when I go to Lago di Santa Giustina?                                               | 1         | 3,5,6    |
| 8          | What public transportation options are available from Trento to the starting point of a beginner-friendly trail? | 3         | 2,4,5,6  |
| 9          | Any recommendations for family-friendly nature activities in Trentino?                                           | 3         | 3        |
| 9          | Is there any easy hike close to Pozza di Fassa?                                                                  | 3         | 3        |
| 10         | Where can I buy sleeping bags and a basic tent?                                                                  | 1,2,3     | 2,4,5    |
| 10         | Where can I buy sleeping bags and a basic tent close to my acommodation?                                         | 2,3       | 2,4,6    |
| 11         | What points of Trentino's natural landscape can be visited in a day without strenuous physical activity?         | 3         | 6        |
| 11         | How many caves, mountains and lake can be visited in Rovereto in a day trip?                                     | 2         | 2,6      |
| 12         | What public transportation is available from Trento to popular hiking destinations?                              | 1,2,3     | 2,4,5,6  |
| 13         | Where I can rent a bike?                                                                                         | 3         | 2        |
| 13         | How can I get to the longest ski resort?                                                                         | 1         | 1        |
| 14         | How can I acess the different skis stations in Trento?                                                           | 1         | 1        |
| 15         | Can you suggest a budget-friendly transportation option?                                                         | 1,2,3     | 4        |
| 15         | Is there a bus I can take to reach the Dolomites?                                                                | 1,2,3     | 4        |
| 16         | What are the top three panoramic viewpoints accessible by car?                                                   | 1,2,3     | 1,3      |
| 16         | What are the top three mountains accessible by car?                                                              | 1,2,3     | 1,3      |
| 17         | Which caves or grottoes are worth exploring for those interested in geological formations?                       | 2         | 6        |
| 17         | Which are the mountains that are close to the lakes?                                                             | 2         | 6        |
| 18         | Can you provide a list of mountain shelter of camping sites along their chosen mountain trails?                  | 1         | 1,4      |
| 19         | What is the closest gas station to every ski station?                                                            | 1         | 1,3      |
| 20         | Which natural attraction is close to this train station (e.g Levico Terme) ?                                     | 1,2,3     | 2,4,5,6  |


## ER Model
From the competency questions, relating to Personas and Scenarios, we extract entities with properties and connect them in a EER model. In our first version, we had mapped several object properties, expecting to obtain the data values that connect them while making queries within the Knowledge Graph. However, this is a mistake, as it is impossible to map properties before having the data first. Therefore, we have created two phases within our Knowledge Graph: the first one shows the current object properties. The second one illustrates in purple the future properties that will be obtained in a later phase.

![Simple EER model](/webassets/minimalEER.png)

![Complex EER model](/webassets/EERphaseii.png)


## Information Gathering
### Data Resources

##### Formal Data Sources:

- [OSM Places Trentino dataset]( https://datascientiafoundation.github.io/LiveDataTrentino/datasets/OSM%20Places/) provided by the DataScientia Foundation
- [Tourist Facilities datasets](https://github.com/rorosonoio/KGE---Trentino-tourist-facilities/tree/main) created by Roberta Peracchio and Hamid Omidi


##### Informal Data Sources:
- [Hike datasets](https://www.komoot.com/discover) sourced from Komoot
- [Lake dataset](https://www.trentino.com/en/highlights/nature-and-landscape/lakes/) sourced from the Trentino page
- [Regions and tourist profesional datasets](https://www.provincia.tn.it/Documenti-e-dati/Risorse/Elenco-dei-referenti-ISTAT-per-il-settore-turismo) sourced from ISTAT


### Knowledge Resources
##### Formal Knowledge Source:

- [OSM Lightweight Ontology](https://datascientiafoundation.github.io/LiveKnowledge/datasets/osm-lightweight-ontology/) provided by The DataScientia Foundation 
- [Various Ontologies](https://schema.org) sourced from schema.org


## Teleontology
In the teleontology phase, we directly import and join both the ontology(showcasing hierarchies) and teleology(showcasing properties) to producea single file, as a consumer.This step was done using Protege, and the illustration using yED. 
![Teleontology](/webassets/realteleontology.png)


## Final Knowledge Graph
After following all the steps outlined in more detail in the project report, we managed to build a knowledge graph in GraphDB based on Trento's natural tourism Teleontology and the associated data. A screenshot of a part of the knowledge graph can be seen in the figure below.

![KG](/webassets/graph.png)

We evaluated our competency questions through the use of SPARQL queries. Here is an example:

Query 1 (CQ 1): What are the top three challenging trails in Trentino?
By most challenging trails we mean the trails that need a high level of expertise.

![Query 1 question](/webassets/query1question.png)
![Query 1 solution](/webassets/query1.png)



## Conclusion

In summary, this research has successfully achieved its objective of constructing a knowledge graph that encapsulates the diverse information related to natural tourism in Trentino. The knowledge graph serves as a valuable tool for gaining insights into various aspects of visitors' options. The practical outcomes of this project signify a promising starting point, with ample opportunities for further enhancement and refinement within the context of Trentino's natural attractions. Looking forward, numerous potential directions for future work have been identified. These include the integration of additional hikes, modeling points of interest within the hikes, enriching the ontology with more references, and the incorporation of more time-specific data into the knowledge graph, possibly from diverse sources (specifying the best and worst times a year to make a certain visit). 
beyond mere points of interest, could provide deeper insights into their preferences and behaviors.Although the project has yielded practical outcomes, it represents just the initial phase of a broader exploration into understanding and enhancing the natural tourism experience using knowledge graphs. The extensive potential for future work promises exciting developments in advancing research within the realm of natural tourism in Trentino.

