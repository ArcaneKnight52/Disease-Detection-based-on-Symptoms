# Disease Detection based on Symptoms

# Introduction
This project uses novel techniques of Machine learning and IR techniques to detect diseases based on symptoms and provide more details about the top fetched diseases including treatment recommendation.

The model which performed best was _DT (Decision Tree) & KNN (K-Nearest Neighbor) with an accuracy of 91.29% and LR (Logistic Regression) model with cross validation accuracy of 89.1%._

The system can be used by a person with restricted medical knowledge as well with ease and can come handy in early disease detection and diagnosis. It can also benefit users that are reluctant to visit hospitals on the onset of minor symptoms. This will provide them with a basic idea of the severity of the disease.


# Dataset used
The previously available dataset is restricted to a particular part of human body disease and is also smaller in volume. Hence, the dataset of disease and their symptoms has been scraped from the web by running the Python script. The dataset consists of diseases and their symptoms, which are fetched from the following sources:

**Diseases**: The list of diseases has been retrieved from the National Health Portal of India ( https://www.nhp.gov.in/disease-a-z ), developed and maintained by Centre for Health Informatics (CHI). The script fetches the HTML code of the page and extracts the disease list by filtering values in HTML tags.

**Symptoms**: The script uses the Google Search package to perform searching and fetch the disease’s Wikipedia page among the various search results obtained. The HTML code of the page is processed to fetch the symptoms of the disease using the ’infobox’ available on the Wikipedia page.

The scraping script fetches over 261 different diseases that form the label and 500+ symptoms.

# Running the system

Either run **SymptomSuggestion.ipynb** or **TF-IDF-NN.ipynb** to use the system. **Google Colab is recommended** for running the system as it uses googlesearch library to suggest treatments, it was observed to be throwing error in Pycharm and Spyder IDE.

# Results

Evaluation of the dataset is done by applying various machine learning algorithms and comparing the accuracy obtained from them. The **highest accuracy is reported by K-Nearest Neighbor (91.29%) and Decision Tree (91.29%) while the lowest is of Multinomial Naive Bayes
(83.94%).**

The system’s performance is evaluated by comparing the predicted diseases that were obtained by the proposed system with the one obtained from WebMD’s Symptom Checker Module ( https://symptoms.webmd.com/default.htm ) and it showed similar results.

# Referrences 
[Anand Sharma](mailto:anand19059@iiitd.ac.in), 
[Nikunj Agarwal](mailto:nikunj19093@iiitd.ac.in) 
[Rahul Maheshwari](mailto:rahul19027@iiitd.ac.in)
