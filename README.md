Machine learning Work Flow
1.import libraries and model
2.load dataset
3.set -> features/input(X) and output/target(y)
4.used the model
5.train the model
6.predict the data from trained model

Code Flow
# whole logic to train a ml model 

#import libraries
import seaborn as sns
from sklearn.linear_model import LinearRegression
#load datasets
sns.load_dataset("tips")
# feature/input
X=df[["total_bill"]]
# target/output
y=df[["tip"]]
#used the model
model = LinearRegression()
#train the model
model.fit(X,y)
#predict the outcomes/results
model.predict([[50]])
