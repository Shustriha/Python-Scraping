# Scraping Python Code

## This code is designed to gather information about physics publications from arxiv.org




### What it does:   
1) Opens page scource code of advanced search page at arxiv.org
2) Goes through all publications in a given time period
3) Based on predefined list of key words it picks specific publisations and collects following information  
    Title,  
    Link,  
    Authors,  
    Abstract(full version),  
    keywords found in and article(might be more than one),  
    MM/YYYY date of publication,  
    Based on keywords found publication is assigned a specific Topic  
4) Information is added into a table
5) Table is then saved as a csv file


## IMPORTANT: To get more details about code implementation see Pictures 1 - 3


### Note:
1) Key words are provided in words_for_search.docx file AND might also be added at Jupyter Nobebook as well
2) Topics assigned to the articles are:  
     Tensor_Networks,     
     Holography,           (aka AdS/CFT - subtopic of String Theory)
     Black_Holes_and_GR,   (GR stands for General Relativity)
     Quantum_Computers_and_Quantum_Information
3) Updated versions of csv files are added from time to time to Kaggle.com and may be found under name
   "Physics articles from arxiv.org"
4) If a given article contains several key words from different Topics it will eventually be assigned a topic
   based on the last of them. (This was neccesary to do in order to prevent latter issues with Tableau visualisations)



### Issues needed to be resolved:
1) Articles don't have information about day of publication   
2) If I have two tables(for example from '2024-01-01' till '2024-06-15' and the other one from '2024-06-01' till '2024-06-27') I would like to be able consistently join them. This will be important for future automatisation of the process.    

   
    

