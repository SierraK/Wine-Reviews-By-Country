# Wine Reviews by Country
Big Data  
Group 1  
### Developer Names:  
- Sierra King  
- Sirisha Vinukonda  
- Anusha Chowdary kollu  
- Liz Conard   
### Developer Pairs:   
###### Pair 1:   
- Sierra King
- Sirisha Vinukonda  
###### Pair 2:  
- Anusha Chowdary kollu
- Liz Conard  

## Links  
Repository: https://github.com/s523286/Group1MapReduce  
Issue Tracker: https://github.com/s523286/Wine-Reviews-By-Country/issues

## Introductory  
We are doing a project in python to perform MapReduce functions on Wine Reviews. The functions we will be performing are to find the sum, count, minimum, and maximum.

## Data Source
We have taken a dataset of Wine Reviews which has 51MB. The variety of the dataset is structured. The file extension is .csv which means it is an excel file.  The dataset provides information on the country the wine is from, the number of points that the wine was rated, and the price of the wine. 

## Data Source Link
https://www.kaggle.com/zynicide/wine-reviews

## The Challenge
The volume of the data is 51MB.
The variety of the data is structured.
The value of the dataset would be important to those interested in the rating of specific wine, where certain wines are from, and the price of the wine.
The veracity of the data is clear and truthworthy.

## Big Data Questions



- ##### Liz Conard  
for each country, find the total sum of points
- ##### Anusha Chowdary Kollu  
for each country, find the average price for each bottle 
- ##### Sirisha Vinukonda    
for each country, find the total highest points  
- ##### Sierra King    
for each country, find the total lowest points
 


## Big Data Solutions
- for each country, find the total lowest points?
#### Mapper input
| country | description                                                                                                                                                                                                                                                                                                                                                                     | designation       | points | price | province   | region_1    | region_2 | variety            | winery |
|---------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------|-------|------------|-------------|----------|--------------------|--------|
| Spain      | This tremendous 100% varietal wine hails from   Oakville and was aged over three years in oak. Juicy red-cherry fruit and a   compelling hint of caramel greet the palate, framed by elegant, fine tannins   and a subtle minty tone in the background. Balanced and rewarding from start   to finish, it has years ahead of it to develop further nuance. Enjoy   2022â€“2030. | Martha's Vineyard | 87    | 65   | California | Napa Valley | Napa     | Cabernet Sauvignon | Heitz  |
#### Mapper Output or Reducer Input
Key: US, Value: 87 (example: Spain, 87)
#### Reducer Ouput
Key: US, Value: 78(lowest: 78)
#### Language
Python
#### Kind of Chart
Bar Graph

- for each country, find the total highest points?
#### Mapper input
| country | description                                                                                                                                                                                                                                                                                                                                                                     | designation       | points | price | province   | region_1    | region_2 | variety            | winery |
|---------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------|-------|------------|-------------|----------|--------------------|--------|
| Spain      | This tremendous 100% varietal wine hails from   Oakville and was aged over three years in oak. Juicy red-cherry fruit and a   compelling hint of caramel greet the palate, framed by elegant, fine tannins   and a subtle minty tone in the background. Balanced and rewarding from start   to finish, it has years ahead of it to develop further nuance. Enjoy   2022â€“2030. | Martha's Vineyard | 96     | 235   | California | Napa Valley | Napa     | Cabernet Sauvignon | Heitz  |

#### Mapper Output or Reducer Input
Key: Spain, Value: 96 (example: US, 96)
#### Reducer Ouput
Key: Spain, Value: 96(highest points= 5679)
#### Language
Python
#### Kind of Chart
Bar Graph  

- for each country, find the average price for each bottle ?
#### Mapper input
| country | description                                                                                                                                                                                                                                                                                                                                                                     | designation       | points | price | province   | region_1    | region_2 | variety            | winery |
|---------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------|-------|------------|-------------|----------|--------------------|--------|
| US      | This tremendous 100% varietal wine hails from   Oakville and was aged over three years in oak. Juicy red-cherry fruit and a   compelling hint of caramel greet the palate, framed by elegant, fine tannins   and a subtle minty tone in the background. Balanced and rewarding from start   to finish, it has years ahead of it to develop further nuance. Enjoy   2022â€“2030. | Martha's Vineyard | 96     | 235   | California | Napa Valley | Napa     | Cabernet Sauvignon | Heitz  |

#### Mapper Output or Reducer Input
Key: US, Value: 235 (example: US, 235)
#### Reducer Ouput
Key: US, Value: 235(Average: sum=158/count=20)
#### Language
Python
#### Kind of Chart
Bar Graph

- for each country, find the total sum of points?
#### Mapper input
| country | description                                                                                                                                                                                                                                                                                                                                                                     | designation       | points | price | province   | region_1    | region_2 | variety            | winery |
|---------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|--------|-------|------------|-------------|----------|--------------------|--------|
| US      | This tremendous 100% varietal wine hails from   Oakville and was aged over three years in oak. Juicy red-cherry fruit and a   compelling hint of caramel greet the palate, framed by elegant, fine tannins   and a subtle minty tone in the background. Balanced and rewarding from start   to finish, it has years ahead of it to develop further nuance. Enjoy   2022â€“2030. | Martha's Vineyard | 96     | 235   | California | Napa Valley | Napa     | Cabernet Sauvignon | Heitz  |

#### Mapper Output or Reducer Input
Key: US, Value: 96 (example: US, 96)
#### Reducer Ouput
Key: US, Value: 96(sum= 560400)
#### Language
Python
#### Kind of Chart
Bar Graph


