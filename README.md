# Diamonds Data Exploration

## Dataset

The data consists of 4898 instances of physico chemical propoerties of wines from Portuguese "Vinho Verde". 
There are 11 features of physico chemical properties such as alcohol content, wine volatile acidity, and residual 
sugar and our main interest variable here is the wine quality which is rated by the sensory test from 0-10. 
Here is the url to the dataset (http://www3.dsi.uminho.pt/pcortez/wine/winequality.zip).


## Summary of Findings

In the exploration, I found that there were strong relationship between wine 
quality and alcohol content, volatile acidity, wine density, and wine chlorides.
The majority of this dataset is mediocre wine, wine rated between 5-6 so we 
encountered some difficulty trying to find correlated features and to find the right 
feature to predict the wine quality, since physico chemical properties might have its 
limitation at the first place. However, there are clear separation between physico-
chemical properties values between white and red wine such as density, volatile
acidity, and chlorides. We used scatterplot of volatile acidity vs. alcohol
content to view whether there is trend of highly rated wine. From our analysis,
it seems that most highly rated wine falls under the alcohol content between 
13-14% and volatile acidity between 0.3-0.6 g/ml. We then further performed PCA
to reduce the dimensionality of the data to see whether there is a huge difference
between the trend between the 2 principal components and the previous 2 features
that were selected. The graph looks quite similar in the trend. We then performed
Decision Tree Regression to visualize how our algorithm is making decision when 
deciding for different rating of wine. Using feature importance, which is a metric
to input features based on how useful they are at predicting a target vairables,
the alcohol content showed 79% and volatile acidity shows 12%. 


## Key Insights for Presentation

For the presentation, I started the univariate section with the distribution 
of the target variables,quality score by plotting the histogram. I then look 
into to proportion of classes(wine type, quality score) of the data. Then, 
I explored the correlation matrix to obtain correlated features with the
target variables.I also engineered a new feature, free SO2 proportion, since
from preliminary research, it is an essentail metric for wine chemical/microbial
stability. Then, the boxplot was used to explore relationship between quality scores,
wine type, and numerical variables such as alcohol content and volatile acidity.
After finding important features as alcohol content and volatile acidity,
the scatterplot was used to plot the trend of different rated wine to these 2
features. Another scatterplot with principal components was used to confirm and
visualize how good our features were at prediciting our target variables. Last,
decision tree was plotted in order to understand how the algorithm predict wine
rating.Throughout this project, I want to acknowledge UCI ML repository for the
dataset. I also used a lot of codes we went through this lesson at udacity.
