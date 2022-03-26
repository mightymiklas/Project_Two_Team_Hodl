# BTC Buy & Sell Algo 2020-2021

UW FINTECH 2021-22 Project II

-This application utilizes EMA, SMA, and RSI market indicators to signify buy and sell signals among the Bitcoin currency thru Machine Learning models such as Support Vector Machine(SVM) and Logistic Regression (LR). 
 
---

## Technologies
--Requirements
python 3.7

- [plotly](https://pypi.org/project/plotly/) - for plotting data
- [pandas](https://pypi.org/project/pandas/) - for analyzing data 
- [numpy](https://pypi.org/project/numpy/) - for analyzing data 
- [seaborn](https://pypi.org/project/seaborn/) - for analyzing data
- [sklearn](https://pypi.org/project/sklearn/) - for analyzing data thru machine learning models
- [tensorflow](https://pypi.org/project/tensorflow/) - for machine learning modeling
- [keras](https://pypi.org/project/keras/) - for analyzing data thru deep learning models
- [matplotlib](https://pypi.org/project/matplotlib/) - for visualizing data
- [jupyter](https://pypi.org/project/jupyterlab/) - an IDE
 

---

## Data Sourced

This Bitcoin data is from the timeframe "yyyy-mm-dd" - "yyyy-mm-dd" and can be generated from [insert url here] <URL>.

---


## Preview

Classification Models...

Support Vector Machine

-Train
	
<img width="384" alt="Screen Shot 2022-03-25 at 19 57 45" src="https://user-images.githubusercontent.com/94579605/160222214-6bb64af7-3e54-4d60-bea8-37d1cf96d52e.png">


		
-Test
	
<img width="380" alt="Screen Shot 2022-03-25 at 19 56 10" src="https://user-images.githubusercontent.com/94579605/160222167-56455a08-aa6f-4fe4-b21c-3be72e3a7dbf.png">


	
Model Correspondence:
	
The SVM model maintains a large delta among both the test and train dataset which produces higher volatility and more sporadic price movement, ultimately decreasing the reliability of the model to produce accurate buy and sell signals. As noted above in the test data-set, our precision was at .58 which is only a minor improvement over a coin toss to make a correct decision to buy or sell. 

Given that SVM models in general work best with unstructured and semi-structured data, such as text or images, because SVM is based upon geometrical properties of the data whereas LR is derived from statistical methods, the risk of overfitting is less in SVM while LR is vulnerable to overfitting.
	
	
Logistic Regression
	
	
-Train
	
<img width="384" alt="Screen Shot 2022-03-25 at 19 59 08" src="https://user-images.githubusercontent.com/94579605/160222267-d474788d-fab1-4247-998b-a6b291f2e913.png">


	
-Test
	
<img width="384" alt="Screen Shot 2022-03-25 at 20 00 38" src="https://user-images.githubusercontent.com/94579605/160222304-c45e1ccb-b06c-4426-aaac-2c10df79a157.png">



Model Correspondence:

The LR model precision is higher and recall score is lower in comparison to the SVM model. This is because the SVM model operates based upon stringent margin principles between data-points which separates the classes and thus reduces the risk of error. In contrast, the LR model accounts for a multitude of decision boundaries, creating a varied margin of error boundary and can account for different weights between data points. 
	
The LR model works best with data that contains variables that maintain more contrast, and delineated identities. Thus fitting our data  with the already indentified "EMA," and "SMA" indicators, our LR model produces buy and sell signals with greater accuracy than the SVM model. 
 
				
## Installation Guide

Before running the application first install the following dependencies:

```python
  pip install pandas
  pip install plotly
  pip install numpy
  pip install sci-kit learn
  pip install tensorflow
  pip install seaborn
  pip install keras
  pip install matplotlib
  pip install jupyter

```
---
## Usage
To execute the application, first clone the repository using 'git clone' and then run 'BitcoinTradingStrategy.ipynb' from within your chosen jupyter environment that fulfills the application requirements, in order to run the program properly. 


## Contributors

[Dao, Nguyen](https://www.linkedin.com/in/nguyen-dao-a55669215/)

[Harrington, Sean](https://www.linkedin.com/in/sean-harrington16/)

[Miklas, Christopher](https://www.linkedin.com/in/christopher-miklas) 

[Rudd, Matthew](https://www.linkedin.com/in/matthewp-rudd/)


---

## License

MIT
