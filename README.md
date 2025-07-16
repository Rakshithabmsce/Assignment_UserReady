# Assignment_UserReady
#assignment 1(load)
The goal of this project is to develop a machine learning model that predicts the Load Type (Light_Load, Medium_Load, Maximum_Load) of a power system using historical energy usage and environmental data. The task involves data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and model evaluation

Steps Performed in the Notebook
1.Data Preprocessing
Converted Date_Time to datetime format using dayfirst=True
Extracted month from the timestamp
Applied feature scaling with StandardScaler
Encoded the target class with LabelEncoder
2.EDA
Count plot of target class distribution
3.Modeling
Trained a RandomForestClassifier on 90% of the dataset (time-based split)
Evaluated on the remaining 10% (last month’s data)
4.Evaluation
Classification Report (Accuracy, Precision, Recall, F1-score)
Confusion Matrix visualization

How to Run
Open load_type_prediction.ipynb in Google Colab.
Upload load_data.csv when prompted.
Run each cell sequentially to preprocess, train, and evaluate the model.
View the classification metrics and confusion matrix in the output.



Assignment 2:(test)
The objective of this project is to build a machine learning-based system that can extract key metadata fields from .docx and .png files regardless of their format or layout. The system must not use rule-based methods (like regex or hardcoded patterns) and should instead apply Natural Language Processing (NLP) techniques to understand and extract required fields from document text.

The following six fields are extracted from the documents:

Agreement Value
Agreement Start Date
Agreement End Date
Renewal Notice (Days)
Party One
Party Two

Used python-docx to extract text from .docx files.
Used pytesseract for OCR-based text extraction from .png scanned images.
Applied the spaCy NLP library with its pre-traine English model to identify entities like dates, names, and monetary values.
Mapped the extracted entities into the six required fields using semantic and positional cues (no static patterns or regex).
Combined results into a structured output matching the format of test.csv

How to Run
Open test.ipynb in Google Colab.
Upload your .docx and .png files when prompted.
The notebook will extract and display the metadata fields.
A test_predictions.csv file will be generated and downloaded automatically.

