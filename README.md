# Flight Data Exploration

In this project we are going to explore the [US Flights 2008 dataset](https://www.kaggle.com/vikalpdongre/us-flights-data-2008/download) of year 2008 & communicate some insights.

## Note
In this repository I don't include the `us-flights-data-2008.zip` which is zip file of `2008.csv` file, `2008.csv` the original data set & `modified_2008.csv` the final & clean dataset we get it after running notebook because they are too big to upload on github.<br/>
If you run the `part1_exploration_flights_2008.ipynb` notebook completely from the begning then these dataset files are downloaded automatically on the system.<br/>
* Downloading link of [us-flights-data-2008.zip](https://www.kaggle.com/vikalpdongre/us-flights-data-2008/download)


## Repository Structure
~~~~~~~
        Flight_Data_Exploration
          |-- part1_exploration_flights_2008.ipynb        # Jupyter notebook contains code foe exploration.
          |-- part1_exploration_flights_2008.html         # Html file of above notebook.	      
          |-- part2_slide_deck_flights_2008.ipynb         # Jupyter notebook contains investigation overview.   
          |-- part2_slide_deck_flights_2008.html          #  Html file of above jupyter notebook.
          |-- part2_slide_deck_flights_2008.slides.html   #  A presentation of above notebook.
          |-- output_toggle.tpl        # file for creating the presentation.
          |-- carriers.csv
          |-- carrier_sorted_2008.csv  # clean Dataset for bi & multi variate visualization.
          |-- README
~~~~~~~

## Installation
To run this project the following libraries need to be installed by using the package manager [pip](https://pip.pypa.io/en/stable/) if you do not have Anaconda installed:

```python
pip install numpy
pip install pandas
pip install matplotlib
pip install seaborn
```

## Dataset
* There are 7009728 rows of flights details in the data set for the year 2008, with 29 features, including cancellations and delay data for 20 unique carriers.<br/>
* Data set can be found in the web site:
[US Flights 2008 dataset link](https://www.kaggle.com/vikalpdongre/us-flights-data-2008/download)<br/>
[carrier dataset link](http://stat-computing.org/dataexpo/2009/carriers.csv)
<br>For the univariate investigation, I used the data set as it is as a data frame. However, for the bivariate and for the multivariate investigation, I used an engineed data frame from the main data frame.<br/>
* The engineered data frame consisted of details of individual carriers such as, total number schedulled flights, total cancellations and total number of delays by the carriers, total delay in minutes and delay per flight operated.

## Summary of Findings
* The distribution of UniqueCarrier column is dominated by the carrier, Southwest airline with a 17.1% contribution. This seems normal as bigger airline carriers contributions are larger and small carrier contributions are smaller as expected.<br/>
* Over 7 million flights schedulled in 2008, 98% have been operated and 2% have been cancelled.There are four types of cancellations (Weather, Carrier, NAS and Security).
* Both weather and carrier cancellations are almost equal and summed up to about 80% of overall cancellations.
* Calulated number of cancellations per 100 flights schedulled by the carrier are compared here.
* American Eagle airline has the highest percentage of about 3.7% and the lowest is owned by Frontier Airline. Calulated number of delayes per 100 flights operated by the carrier are compared here.
* Atlantic Southwest airline has the highest percentage of about 13% and the lowest of about 3% is recorded by Aloha Airline. Calulated delay time in minutes per flight operated by the carriers are compared here.
* Mesa airline has the highest close to 8 min while Aloha airline has the lowest closer to 1 min.

## Key Insights for Presentation
* The worst airline carrier in 2008 is Mesa airline. They have the highest delay time per flight and second highest in both percent cancellations and delayes.
* The best airline is Aloha air line and they recorded the lowest in both delay per flight and percent delayes while being the second lowest in percent cancellations.
