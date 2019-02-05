## Project: Recommending Restaurants using Collaborative Filtering.

### Install

This project requires **Python 3.6** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 3.6 installer and not the Python 2.x installer. 

### Run

In a terminal or command window, navigate to the top-level project directory `Restaurant-Data/` (that contains this README) and run one of the following commands:

```bash
ipython notebook Collaborative_Filtering.ipynb
```  
or
```bash
jupyter notebook Collaborative_Filtering.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.


## Data

The Restaurant Data is a collection of data points obtained from restaurants and users.<br />
The task is to generate a top-n list of restaurants according to the consumer preferences using collaborative filtering.<br />
The collaborative filtering technique uses geoplaces2.csv, rating_final.csv and userprofile.csv files.<br />
More information can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data).

**Files, instances and attributes**<br />
Number of Files: 9<br />

Restaurants<br />
1. chefmozaccepts.csv
2. chefmozcuisine.csv
3. chefmozhours4.csv
4. chefmozparking.csv
5. geoplaces2.csv

Consumers<br />
1. usercuisine.csv
2. userpayment.csv
3. userprofile.csv

User-Item-Rating<br />
1. rating_final.csv

**Description format of datasets required for collaborative filtering**<br />
File name<br />
Number of instances<br />
Number of attributes<br />
attribute: Type, Number of missing values (if any), Number of values [list of values]

`geoplaces2.csv`<br />
Instances: 130<br />
Attributes: 21<br />
placeID: Nominal<br />
latitude: Numeric<br />
longitude: Numeric<br />
the_geom_meter: Nominal (Geospatial)<br />
name: Nominal<br />
address: Nominal,Missing: 27<br />
city: Nominal, Missing: 18<br />
state: Nominal, Missing: 18<br />
country: Nominal, Missing: 28<br />
fax: Numeric, Missing: 130<br />
zip: Nominal,Missing: 74<br />
alcohol: Nominal, Values: 3 [No_Alcohol_Served,Wine_Beer,Full_Bar]<br />
smoking_area: Nominal, 5 [none,only_at_bar,permitted,section,not_permitted]<br />
dress_code:	Nominal, 3 [informal,casual,formal]<br />
accessibility: Nominal, 3 [no_accessibility,completely,partially]<br />
price: Nominal, 3 [medium,low,high]<br />
url: Nominal, Missing: 116<br />
Rambience: Nominal, 2 [familiar,quiet]<br />
franchise: Nominal, 2 [t,f]<br />
area: Nominal, 2 [open,closed]<br />
other_services:	Nominal, 3 [none,internet,variety]<br />

`rating_final.csv`<br />
Instances: 1161<br />
Attributes: 5<br />
userID: Nominal<br />
placeID: Nominal<br />
rating: Numeric, 3 [0,1,2]<br />
food_rating: Numeric, 3 [0,1,2]<br />
service_rating:	Numeric, 3 [0,1,2]<br />

`userprofile.csv`<br />
Instances: 138<br />
Attributes: 19<br />
userID: Nominal<br />
latitude: Numeric<br />
longitude: Numeric<br />
the_geom_meter: Nominal (Geospatial)<br />
smoker: Nominal, Missing: 3, 2 [false,true]<br />
drink_level: Nominal, 3 [abstemious,social drinker,casual drinker]<br />
dress_preference:Nominal, Missing: 5, 4 [informal,formal,no preference,elegant]<br />
ambience: Nominal, Missing: 6, 3 [family,friends,solitary]<br />
transport: Nominal, Missing: 7, 3 [on foot,public,car owner]<br />
marital_status:	Nominal, Missing: 4, 3 [single,married,widow]<br />
hijos: Nominal, Missing: 11, 3 [independent,kids,dependent]<br />
birth_year:	Nominal<br />
interest: Nominal, 5 [variety,technology,none,retro,eco-friendly]<br />
personality: Nominal, 4 [thrifty-protector,hunter-ostentatious,hard-worker,conformist]<br />
religion: Nominal, 5 [none,Catholic,Christian,Mormon,Jewish]<br />
activity: Nominal, Missing: 7, 4 [student,professional,unemployed,working-class]<br />
color: Nominal, 8 [black,red,blue,green,purple,orange,yellow,white]<br />
weight: Numeric<br />
budget: Nominal, Missing: 7, 3 [medium,low,high]<br />
height: Numeric<br />
