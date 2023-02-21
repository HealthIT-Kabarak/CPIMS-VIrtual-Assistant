# CPIMS 

Devs
1. [Dedan Okware](https://github.com/SoftCysec)
2. [Rebecca Cheptoek](https://github.com/Rebeccacheptoek)
3. [Emmanuel Kigen](https://github.com/kigenchesire)
4. [Stanley Njoroge](https://github.com/stanley643)

<details>
  <summary><h2>Business Understanding</h2></summary>
  <h3>I. Problem</h3>

- CPIMS service desk receives a high volume of repetitive requests from users, negatively impacting the efficiency and effectiveness of the support team and creating a negative user experience.
- The need to develop a virtual assistant to help reduce the amount of requests and improve user experience.
- Key services that the end user expects the virtual assistant to perform.
  
  <h3>II. Client Engagement Process</h3>

A user-centered virtual assistant is developed through a user engagement process consisting of the following steps:
- Defining target audience
- Understanding user needs
- Defining virtual assistant purpose
- Creating a user-friendly virtual assistant
- Providing excellent services
- ntinuously improving the virtual assistant
- asuring user engagement
  
  <h3>III. Objectives</h3>
  
- To develop a user support Virtual Assistant for the CPIMS system.
- To deploy the virtual assistant for the CPIMS system into a web interface to enhance user experience.
- To develop online virtual assistance using machine learning which can be able to answer inquiries and user queries quickly and efficiently.
</details>
<details>
  <summary><h2>Data Acqusition</h3></summary>
  <h3>Sources of Data</h3>
  
- WhatsApp chats from 5 different groups based on regions
- CPIMS website documentations and frequently asked questions
  <h3>Data Acquisition Process</h3>
  
- Extraction, Transformation, and Loading (ETL) tool used
- Extraction of data from text files
- Transformation of data into JSON format
- Loading of data into system for model training
  </details>
<details>
<summary><h2>Exploratory Data Analysis</h2></summary>

<h3>I. Introduction</h3>

- Explanation of EDA and its purpose in this project
- The main variable of interest in the data

<h3>II. EDA Techniques Used</h3>

- Description of the exploratory visualizations used to analyze the frequently asked questions
- Explanation of data cleaning and preprocessing
- Identification of patterns and relationships

<h3>III. Results of EDA</h3>

- Distribution of user intentions
- Feature selection and most frequent phrases used to train the model
- Visualizations including histograms and box plots to examine the distribution of message types across different intents
- Word frequency analysis to identify the most common words and phrases used in different questions
- Conclusion on the most common topics and trends in the chat conversations
![](https://github.com/HealthIT-Kabarak/CPIMS-VIrtual-Assistant/blob/main/static/Images/image_1.jpg)
![](https://github.com/HealthIT-Kabarak/CPIMS-VIrtual-Assistant/blob/main/static/Images/image_2.jpg)

<h3>IV. Conclusion</h3>

- Outcome of EDA and its usefulness in understanding the data
- Importance of EDA in the development of the chatbot model

</details>

<details>
<summary><h2>Data Cleaning</h2></summary>

<h3>Introduction</h3>

Briefly introduce the topic of data cleaning and its importance in the data science process

<h3>Data Cleaning Process</h3>

- Explain the process of data cleaning which involved:
- Identifying the intents of each chat such as password reset
- Categorizing the data into different intents
- Creating a JSON file and tagging each intent with pattern and response
- Removing duplicated patterns and responses, and unnecessary characters
- Formatting the data
- Extracting key information related to CPIMS from the entire dataset
<h3>Data Cleaning Outcomes</h3>

Describe the outcomes of the data cleaning process, which included:
- Acquiring a dataset that only contained CPIMS related issues
- Creating a JSON file that was used to solve the problem
- Improving data quality by removing errors, inconsistencies, and irrelevant data

<h3>Conclusion</h3>
Summarize the importance of data cleaning in ensuring high quality data for analysis and modeling purposes.
</details>


<details>
  <summary><h2>Feature Engineering</h2></summary>
  <h3>I. Introduction</h3>

- Definition of feature engineering
- Importance of feature engineering in training a machine learning model
  
  <h3>II. Feature Engineering Process</h3>

- Data cleaning and transformation
- Converting data to lowercase
- Tokenizing of data
- Removing punctuation
- OneHotEncoding
- Removing emojis
- Lemmatization
- Limiting each question to a length of 50 words
  
  <h3>III. Features Used</h3>

- Intents
- Patterns
- Responses
  <h3>IV. Conclusion</h3>

- Summary of feature engineering process and features used
- Importance of feature engineering in training chatbots
</details>

<details>
  <summary><h2>Model Development</h2></summary>
  
  <h3>Model Development</h3>
This project uses a supervised learning approach for model development. The approach involves providing the computer with labeled data, which consists of input data and corresponding desired output. The computer then learns a model from this data, which can be used to map new input data to the desired output. The model can also classify data into different categories and make predictions on unseen data.

  <h3>Justification for Model Used</h3>
The chosen model is useful because it is capable of making predictions on unseen data and classifying data into different categories. It is an effective way of training a machine learning algorithm using labeled data. The supervised learning approach used in this project ensures accuracy and reliability since the computer is given both the input data and the corresponding desired output.

</details>

<details>
  <summary><h2>Model Evauation</h2></summary>
  
Machine learning models are evaluated using metrics, which are measures of performance that can be used to track and compare progress. Metrics provide an objective way to measure and compare progress, allowing for informed decision-making and identification of areas for improvement.

  <h3>Metrics Used</h3>
The following metrics were used to evaluate the model:

  <h4>Precision:</h4> measures accuracy and consistency in a model, assessing how accurately the model can predict the true value of the target variable. It measures how many of the predictions made by the model were correct. Higher precision indicates more accurate predictions by the model.

  <h4>F1-score:</h4> combines precision and recall into a single score to assess the overall performance of the model. It takes into account both precision and recall to give an overall measure of how well the model is performing. Higher F1-score indicates better overall performance of the model.

  <h3>Results from Different Metrics</h3>
The accuracy of the model was evaluated using precision and F1-score metrics. Results of the evaluation will be presented in this section.

  <h3>Justification for Metrics Used</h3>
The precision, recall, and F1-score metrics are useful for assessing the performance of a model. Precision measures accuracy, recall measures completeness, and F1-score combines these two metrics into a single score. Using these metrics allows for a more comprehensive assessment of the model's performance, helping to identify areas for improvement.


</details>
