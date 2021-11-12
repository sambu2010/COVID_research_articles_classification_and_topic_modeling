## COVID -19 Research Articles Analysis

### Abstract

It is important for scientists to get information coming from all scientific sources that may help them combat the pandemic. The challenge, however, is that the number of scientific papers created is large and the papers are published very rapidly, making it nearly impossible for medical professionals to digest and understand all important aspects of the data in this chaos. One of the solutions to this problem will be to create an unsupervised learning model that will be organizing research documents by information containing in them.

### Design

Create an unsupervised learning model that will read scientific papers and will be able to analyze what is it about based on the text and extract key terms allowing researchers to quickly and easily gather targeted information and locate relevant text in the paper to answer important questions of the analysis.

### Data

Dataset is used for this project is CORD-19 (COVID-19 Open Research Dataset). CORD-19 is a resource of over 500,000 scholarly articles, including over 200,000 with full text, about COVID-19, SARS-CoV-2, and related coronaviruses. Only subset of this data is used for this project (research articles for 2020-2021 years).

### Algorithms

Initial EDA includes handling missing values, type conversion, filtering and graphical representation fo data.

Data is then cleaned using spaCy: stop words and punctuation removed, data is lemmatized and tokenized using CountVectorizer.

LDA is performed for topic modeling using GridSearchCV to determine the optimal number of components. 15 components selected. As a result 15 topic have been identified. Topics linked back to the original dataset, so each research article has a topic and most common words associated with it. This will make a process of analyzing articles more streamlined and more efficient.

### Tools

- Pandas and Numpy are used for data cleaning and manipulation
- Sklearn us used for modeling
- Matplotlib and Seaborn are used for visualization

### Communication

The jupyter notebook containing data and full analysis and PP presentation are located in the GitHub repo folder for this project.
