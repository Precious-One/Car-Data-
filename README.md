# Car-Data 🚗
Repository is all about Linear Regression and Logistic Regression. Linear Regression helps you to train data and predict price accordingly. Logistic Regression helps to predict wheather car is 4WD, FWD, RWD

There are 2 types of Encoding you can use :
*Type 1 -
df['fueltypes'].replace({'diesel':1, 'gas':2})
df['aspiration'].replace({'std':1, 'turbo':2})
df['doornumbers'].replace({'four':1, 'two':2})
df['carbody'].replace({'convertible':1, 'hardtop':2, 'hatchback':3, 'sedan':4, 'wagon':5})
df['drivewheels'].replace({'4wd':1, 'fwd' :2,'rwd':3,})
df['enginelocation'].replace({'front':1, 'rear':2})
df['enginetype'].replace({'dohc':1, 'dohcv':2, 'l':3, 'ohc':4, 'ohcf':5, 'ohcv':6, 'rotor':7})
df['cylindernumber'].replace({'eight':1, 'five':2, 'four':3, 'six':4, 'three':5, 'twelve':6, 'two':7})
df['fuelsystem'].replace({'1bbl':1, '2bbl':2, '4bbl':3, 'idi':4, 'mfi':5, 'mpfi':6, 'spdi':7, 'spfi':8})

*Type 2 -
import pandas as pd
df1_lg = pd.get_dummies(df1,columns=cat,drop_first =True)

Both works fine.

Also I used StandardScaler because I'm comfortable with it, you can also try out MinMaxScaler.
