Steps Involued:

  1.Library Imports
      
      #Import essential libraries for data handling, model training, evaluation, and visualization.
      #libraries used: pandas, numpy, scikit-learn, imbalanced-learn, ipywidgets,tabulate and drive.  
2.Data Preprocessing Function

    #preprocess_clean(data): Handles missing values, scales the features, splits the data in the ratio of 80:20, and balances the classes using SMOTE (Synthetic Minority Over-sampling Technique).

3. Model Implementation:
      (i) Random Forest

           #RandomForest(data): Trains and evaluates a Random Forest model.
      (ii)Decision Tree

          #Decision_Tree(data): Trains and evaluates a Decision Tree model.
      (iii)Logistic Regression

          #Logistic_Regression(data): Trains and evaluates a Logistic Regression model.

4. Data Loading

       #Mount Google Drive and load the dataset
       drive.mount("/content/drive", force_remount=True)
       data = pd.read_csv("/content/drive/MyDrive/Colab Notebooks/creditcard.csv").sample(frac=1)

5. Display Functions

        #display_metrics(model_name, prediction): Formats and displays the model's evaluation metrics in an HTML table using ipywidgets
   
7. Button Initialization for each model to display the evaluation metrics
8. Button Event Handler
   
        #on_button_clicked(model_name): Handles button clicks to train and evaluate the selected model and display the metrics.
9. Execution

       #Click a specific button to train and evaluate the desired model. Metrics will be displayed in a formatted table.

NOTE: In the provided creditcard.ipynb the table are not visible due to localhost jupyter notebook and would be in cloud based platform like google colab. The Outputs are provide in the output(Folder) and can visualize the formatted table.

* IF MODULE ERROR OCCUR use !#pip install <package> in google colab
* Ensure both code, dataset exist in GOOGLE DRIVE and change the path for accessing the dataset accordingly.


