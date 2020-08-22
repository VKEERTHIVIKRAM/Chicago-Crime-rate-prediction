# Data Set
[Chicago crime rate prediction dataset](https://drive.google.com/drive/folders/1oh4fK7G4L8UkOBMHq-UXYwKR-HpLOqvH?usp=sharing)

# About
The Chicago Crime dataset contains a summary of the reported crimes occurred in the City of Chicago from 2001 to 2017. 

Dataset has been obtained from the Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system.

Dataset contains the following columns: 
1. ID: Unique identifier for the record.
2. Case Number: The Chicago Police Department RD Number (Records Division Number), which is unique to the incident.
3. Date: Date when the incident occurred.
4. Block: address where the incident occurred
5. IUCR: The Illinois Uniform Crime Reporting code.
6. Primary Type: The primary description of the IUCR code.
7. Description: The secondary description of the IUCR code, a subcategory of the primary description
8. Location Description: Description of the location where the incident occurred.
9. Arrest: Indicates whether an arrest was made.
10. Domestic: Indicates whether the incident was domestic-related as defined by the Illinois Domestic Violence Act.
11. Beat: Indicates the beat where the incident occurred. A beat is the smallest police geographic area – each beat has a dedicated police beat car. 
12. District: Indicates police district where the incident occurred. 
13. Ward: The ward (City Council district) where incident occurred. 
14. Community Area: Indicates the community area where the incident occurred. Chicago has 77 community areas. 
15. FBI Code: Indicates the crime classification as outlined in the FBI's National Incident-Based Reporting System (NIBRS). 
16. X Coordinate: The x coordinate of the location where the incident occurred in State of Illinois.
17. Y Coordinate: The y coordinate of the location where the incident occurred in State of Illinois.
18. Year: Year the incident occurred.
19. Updated On: Date and time the record was last updated.
20. Latitude: The latitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block.
21. Longitude: The longitude of the location where the incident occurred. This location is shifted from the actual location for partial redaction but falls on the same block.
22. Location: The location where the incident occurred.

## What is Facebook Prophet?

Prophet is open source software released by Facebook’s Core Data Science team. Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. Prophet works best with time series that have strong seasonal effects and several seasons of historical data. For more information, please check this out:

* [Prophet forecasting at scale](https://research.fb.com/prophet-forecasting-at-scale/)
* [Quick start to Prophet](https://facebook.github.io/prophet/docs/quick_start.html)

Prophet implements an additive regression model with four elements:

* A piecewise linear, Prophet automatically picks up change points in the data and identifies any change in trends. 
* A yearly seasonal component modeled using Fourier series.
* A weekly seasonal component.
* A holiday list that can be manually provided.

Additive Regression model takes the form: 
$$
Y=\beta_0+\Sigma^p_{_j=1} f_j(X_j )+\epsilon
$$




**NOTE:**

* You must install fbprophet package as follows: 

```python
pip install fbprophet
```

* If you encounter an error, try: 

```python
conda install -c conda-forge fbprophet
```

