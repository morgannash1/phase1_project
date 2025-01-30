![skydiving](images/skydiving.png)

# Aviation Accident Analysis
**Author**: [Morgan Nash](mailto:morganmichellenash@gmail.com)

## Business Understanding
This project aims to determine which planes would be best to look into first for indoor skydiving companies that plan to expand to offer real, outdoor skydiving. Beginner skydiving companies can use this analysis to determine which planes would be of lowest risk to start with as the project will offer recommendations based on vizualizations that show safety comparisons.

## Data Understanding
The data source used in this project is a data set from the National Transportation Safety Board with specifics about US aviation accidents between 1962 through 2023. There are over 90,000 records of specific accidents with 31 columns of information telling location, date, aircraft make, aircraft model, number of engines, total fatal injuries, total uninjured, etc. 


### Data Preparation & Analysis
To clean the data set, many unnecessary columns were dropped. For example: Accident Number, Event ID, Airport Code, Airport Name, etc did not help with analysis. Some rows and columns with a high percent of missing data were also dropped.

A smaller portion of the dataset was used to determine a starting point by looking at commonly reported aircraft Make and Models specific to skydiving. 

Then these makes and models were re-examined in a cleaned version of the original dataset. 

### Visualizations & Findings: 
![accidents by year](images/visualizations/accidents.by.year.png)

**Note**: Many accidents between the years of 2001 and 2006 were dropped while cleaning the dataset

![top sky makes](images/visualizations/top.sky.makes.png)

We see the top reported aircraft Makes for skydiving specific accidents, with Cessna clearly as the top reported.

![top sky models](images/visualizations/top.sky.models.png)

![engine fatality](images/visualizations/enginefatality.png)

Here we see 2 key points. First, we see that Cessna has many more accidents reported where people were uninjured as compared to Beech. We also see that this is more specifically true for Cessna aircrafts with 1 engine.

![percent fatality](images/visualizations/percent.fatality.png)

![percent uninjured](images/visualizations/percent.uninjured.png)

## Conclusions

### Recommendations
- **Cessna is the top reported make for Skydiving Aircrafts. Cessna models compared to Beech (the second top reported Skydiving Make) are safer.**

- **Cessna Aircrafts with 1 engine appear to be the safest choice as compared to Cessna Aircrafts with 2 engines as well as compared to Beech Aircrafts with any number of engines.**

- **By comparing Percent of Fatality and Percent of Uninjured, Cessna Models 180 and 170 are safer than other models as their Fatality Rate is lowest and Uninjured Rate is highest**

### Limitations
The largest limitation of this data set is that we only have the data for accidents. We don't have the data for when flights occurred where everything went smoothly. This means we cannot say anything like: "99% of flights of a certain kind of plane occured safely." This also makes it difficult to see the whole picture. We assume that certain Aircrafts appear more often because they are more common, not because they are inherently more dangerous. 


### Next Steps
When it comes to aircrafts that will be used for Skydiving, there are many other important features not included in the Aviation Accident Dataset. A few of these that should be considered next include: how fast the aircraft can climb to reach desired elevation for jumping, safety features related to the exit doors, cost of the aircrafts, aircraft speed, and passenger capacity.

## For More Information

See the full analysis in the [Jupyter Notebook](./aviationaccidentanalysis.ipynb) 

Interact with the visualizations in [Tableau](https://public.tableau.com/app/profile/morgan.nash/viz/AviationAccidentsSkydiving/AviationAccidentsSkydiving#1)

## Repository Structure

```
├── images
├── README.md
├── Presentation.pdf
└── aviationaccidentanalysis.ipynb
```
