### Project Overview

 Webster dictionary defines data as factual information (such as measurements or statistics) used as a basis for reasoning, discussion, or calculation'. Factual information can take many forms. We will discuss these forms of data and what they mean.

Data can be broadly classified into two categories viz categorical and quantitative data. As the name suggests qualitative data in non-numeric in nature whereas quantitative data is numeric. Categorical data can be further classified as ordinal and nominal, whereas quantitative data can be subcategorized as discrete and continuous.

Categorical Data

A categorical variable measures something and identifies a group to which the thing belongs. They describe a quality or characteristic of a data unit like what type or which category. They tend to be represented by a non-numeric value and fall into mutually exclusive and exhaustive categories. Sometimes a categorical variable is stored as a string. Ex: Blood group of a person

Categorical data are classified as:

Nominal data there is no natural order between the categories (eg eye color, Gender i.e Male or Female),

Ordinal data an ordering exists (eg. exam results, socio-economic status, Educational Level - Kindergarten, Primary, Secondary, Higher Secondary, Graduation, etc.).

Quantitative Data

Quantitative or numerical data arise when the observations are counts or measurements. The data are said to be discrete if the measurements are integers (ex. number of people in a household, number of cigarettes smoked per day) and continuous if the measurements can take on any value, usually within some range (ex. weight).

Interval data is numeric unlike nominal and ordinal data and the difference between the successive numbers is constant. Such variables do not have a zero point. This means that a value zero does not mean the absence of this variable. eg. (IQ score of individuals, temperature).

Ratio is quite the same as interval variables with the addition that they have a meaningful zero point. This means a ratio value zero indicates the absence of the given variable. eg. (height, age, the weight of individuals, dimensions of a room).

We should be aware of these different types of data, as we need to apply different processes to the same. We will look at these processes during the data pre-processing step.

Let us now take a look at a real dataset and try to identify the type of variables the dataset contains.

We will be using a rich dataset on housing prices from Ames, Iowa. Each row in the dataset describes the properties of a single house as well as the amount it was sold for. The original data set contains 82 features and 2930 data points. You can read more about this dataset here and download the dataset from here.

However, for the purpose of learning descriptive statistics, we will specifically, work on the following features of the house

Lot Area
Number of Bedrooms
Garage Area
Condition of the house
Sale Price
Brief explanation of the dataset & features

Lot Area (Continuous): Lot size in square feet.
Bedroom (Discrete): Bedrooms above grade (does NOT include basement bedrooms).
Garage Area (Continuous): Size of garage in square feet.
Overall Cond (Ordinal): Rates the overall condition of the house. 10 Very Excellent 9 Excellent 8 Very Good 7 Good 6 Above Average
5 Average 4 Below Average
3 Fair 2 Poor 1 Very Poor
SalePrice: Sale price of the house



### Learnings from the project

 After completing this project, you will have a better grip on the applications of descriptive statistics. In this project, you will be applying the following concepts:

Bar plotting
Boxplot plotting
Pie-chart plotting
Subplot operations
Feature Correlation
IQR operations


### Additional pointers

 Feature:	Description
        ID	:Unique character ID
    Name	Name of the character
    Gender	:Male/Female
        Intelligence	:Intelligence points of the character
    Strength	:Strength points of the character
    Speed	:Speed points of the character
    Durability:	Durability points of the character
    Power	: Power points of the character
    Combat:	Combat points of the character
    Total	:Total sum of all the above points of the character
    Height:	Height of the character(-99 value equates to 'immeasurable')
    Weight	:Weight of the character(-99 value equates to 'immeasurable')
    SkinColor:	Skin color of the the character
    EyeColor	:Eye color of the character
    HairColor:	Hair color of the character
    Race	:Which race the character belongs to


