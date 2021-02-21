# Data Visulization 
Followed by Data Reshaping and Preprocessing, we obtained a series of tokenized words. Due to the large amount of data set, it is hard for us to uderstand the underlying trends and patterns. Therefore, the data visulization becomes neccesary. As a part of data visulization, the frequency table and wordclouds are genenarated to tell the story behind the data.   
## 1. Process

### 1.1 Generating Frequency Set 
Firstly, we use dictionary in Python to count the frequencies in the 'final_token' list obtained from data shaping. and increment the counter using loops. 

![Frequency Set](https://user-images.githubusercontent.com/78474798/108610401-3c2cf000-73cd-11eb-80b4-a43736206c4c.png)

Note:The Def in python is short for "define", which performs a specific task. Therefore, the statements under Def should run together. 

### 1.2 Word Clouds
Word clouds  are visual representations of words. Here our geoup use word clouds to popular words based on word frequency. In this way, the large amount of data could be present in a quick and simple visual insights. 

![Word cloud](https://user-images.githubusercontent.com/78474798/108610614-efe2af80-73ce-11eb-8ca0-90aaa5c8efe4.png)

Note: To use wordcloud, we need to install worldcloud package from 
      #git clone https://github.com/amueller/word_cloud.git
      #cd word_cloud
      #pip install
      #or easy downland with conda install -c conda-forge wordcloud

### 1.3 Frequency Table 

The frequency table shows the number of times a word occurring in Fosun tweets. We stored the frequency value key:value pairs and used a one-dimensional array (pd.series) to store the data. 

![Frequency Table](https://user-images.githubusercontent.com/78474798/108610622-0557d980-73cf-11eb-9b67-0274007e207e.png)

## 2. Results 
The world could picture and frequency table generating from the frequency of words in Fosun tweets are shown as below:

![Figure 2021-02-21 081058](https://user-images.githubusercontent.com/78474798/108612591-03b90080-7425-11eb-81db-328f9d995a54.png)

![fosun frequency](https://user-images.githubusercontent.com/78474798/108610649-4354fd80-73cf-11eb-92dd-cc84d46c4115.png)

## 3. Problems 

After finishing data visulization, we found two unrecoginized words appearing in our frequency table and world cloud of Fosun. Therefore, we re-examineed previous process step by step and ran the frequency of words in Bilibili tweets to do the rain check. The tables presenting the frequency of words in Bilibili tweets contains unregonized words as well. By checking the 'Variable Explorer' in Python, we discovered that these two unrecognized words are actually 'Chinese'. It shows the potential problems in the previous step, Data Reshaping and Preprocessing. It is always good to detect the problems in the early stage as it gives us the opportunity to correct the mistakes and stop loss in time. The process of analyzing natural language data would never be a smooth sailing and the most important thing is to keep going and moving forward. 
