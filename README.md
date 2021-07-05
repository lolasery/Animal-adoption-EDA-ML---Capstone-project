# Animal-adoption-EDA-ML---Capstone-project
## *Table of contents*
- [Problem Statement](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#problem-statement)
- [Goal](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#goal)
- [Data pre-processing](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#data-pre-processing)
   - Data engineering
      - [Feature Engineering]()
         - [Total time spent in shelter]
      - [Example of features with data set errors](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#example-of-features-with-data-set-errors)
         - [animalage](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#animalage)
            - [Before & after data-preprocessing](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#before-and-after-data-preprocessing)
- [ML models used](https://github.com/lolasery/Animal-adoption-EDA-ML---Capstone-project/blob/main/README.md#ml-models-used)

## Problem statement
- need to maximise adoption rates to ensure adoption shelters are not completely dependent on government funding as well as to improve the quality of life of animals and pet owners.
- This is based off our label: (Adopted, adopted & Returned & Not adopted)
- ![label](https://user-images.githubusercontent.com/78312050/124507050-8dc79b80-ddff-11eb-9634-309278125e00.PNG)

## Goal
- to assist shelters in identifying features to take note of when trying to improve adoption rates.
![adoption-fee-banner](https://user-images.githubusercontent.com/78312050/123228543-17c25b00-d508-11eb-85fd-d3ca3396b6a8.jpg)
## EDA (exploratory data analysis) interesting points:
- Black cats and dogs have the highest abandon and adoption rates
- 
# Data pre-processing
## Data engineering
- Data needs to be in numbers for the Machine to read, these numbers shoud also make sense in the real world. 
### Feature engineering
- **Total time spent in shelter**
   - getting **Total time spent in shelter** with intake and movement date
   - ![movein](https://user-images.githubusercontent.com/78312050/124500047-a466f600-ddf1-11eb-9013-6921c74c396d.PNG)
   - ![timespent](https://user-images.githubusercontent.com/78312050/124503961-260e5200-ddf9-11eb-95ef-93b11234ca49.PNG)
   -  **Negative** timing is due to the same day dates being reversed is terms of newer and older dates. easily solved with abs() function
   - ![time spent in shelter](https://user-images.githubusercontent.com/78312050/124504257-acc32f00-ddf9-11eb-8600-d3a9a83e31f4.PNG)



### Example of features with data set errors
#### animalage
![sam](https://user-images.githubusercontent.com/78312050/124398735-dd4b9000-dd49-11eb-9381-c6cf2dee0af2.PNG)
- Dataset column is riddled with:
   - **strings** where days, weeks & months need to be converted into years
      - *Regular expression* usage to achieve this
   - **outlier errors** which need to make sense. Data that is on extreme ends can affect certain ML models 
      - *better to keep the data's SD relatively low*
      - Here i chose to replace the outlier age (100 year old cats/ dogs) with the googled average maximum age of a cat/dog
![regular expression](https://user-images.githubusercontent.com/78312050/124397544-f7ce3b00-dd42-11eb-8568-a1306e6e95d2.PNG)

### Before and after data-preprocessing
![age product](https://user-images.githubusercontent.com/78312050/124398208-1afae980-dd47-11eb-8f74-2de304e5754d.PNG)
![Capture](https://user-images.githubusercontent.com/78312050/124480640-12072800-ddda-11eb-85e0-94b6e83902fd.PNG)
## ML models used
Utilizing various Machine learning algorithmns and libraries to get the best model 
![Decision-Trees-Root-Node](https://user-images.githubusercontent.com/78312050/123955411-27481500-d9dc-11eb-91a8-321f66414e67.png)
![images (1)](https://user-images.githubusercontent.com/78312050/123228726-44767280-d508-11eb-91d5-7b23c811a19c.png)
![1523957272561](https://user-images.githubusercontent.com/78312050/123955599-637b7580-d9dc-11eb-9368-b50355d5b7fb.jpg)


