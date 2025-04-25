# DS-ML-Project
> [!NOTE]
Final project in the last month of Data Science/Machine Learning class

## Project Description
This project is intended to produce a machine learning model to capable of accurately predicting if a student has ever overdrawn their checking account based on their age, gender, and how many days per month they drink (see [Features](#features)).

### Project Goals
- [x] Explore and clean the dataset to prepare it for modelling
- [x] Test different machine learning models to predict if overdrawn
- [x] Compare the performance of the different models and choose the best one

## Results
The Decision Tree model turned out to be the best fit, with an 85% accuracy.

</br>

## Data
The [project_data.csv](src/data/Project_Data.csv) dataset of 450 records with features of students' ages, genders, how many days per month they drink, and if they have ever overdrawn their checking account.
### Features
#### Raw Data
450 records of
<table><thead>
  <tr>
    <td>Age</td>
    <td>Gender</td>
    <td>DaysDrink</td>
    <td>Overdrawn</td>
  </tr></thead>
</table>

#### Cleaned Data
435 records of
| Gender | Gender_Male | Gender_Female | Age | DaysDrink | Overdrawn |
|:-:|:-:|:-:|:-:|:-:|:-:|
| `string object` | `int64` | `int64` | `int64` | `category` | `int64` |
| `'Male' or 'Female'` | `0 or 1` | `0 or 1` | `> 0` | `'None', 'Low', 'Moderate' or 'High'` | `0 or 1` |
