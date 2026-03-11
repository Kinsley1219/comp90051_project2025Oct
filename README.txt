COMP90051 Project 
Analysis of the robustness of machine learning under the cover of face recognition

Xinyao Li 1560643
Hanyue Li 1650115
Yichen Sun 1682096

How to Run :

1. Data Source: CelebA (200k images)
                https://www.kaggle.com/datasets/jessicali9530/celeba-dataset

   We sampled 12,000 images through a Kaggle notebook.
   Run the Kaggle notebook code "comp90051-sampled-image-data.ipynb"
   To download the final dataset we used:
     - /kaggle/working/celeba_subset
     - /kaggle/input/celeba-dataset/list_attr_celeba.csv

2. After downloading the two zip files from the Kaggle notebook,
   Upload them to your own Google Drive:
   Then, update the dataset paths to match your Drive:
     zip_image = "/content/drive/MyDrive/comp90051 project/share data/celeba_subset.zip"
     zip_attr  = "/content/drive/MyDrive/comp90051 project/share data/list_attr_celeba.csv.zip"

3. Open the Colab notebook:"comp90051_project_ipynb(Final).ipynb"

4. Switch Colab to a GPU runtime

5. Run all cells sequentially.
   The notebook will automatically:
     - Unzip and load data
     - Extract HOG features with occlusion
     - Train and evaluate three models (Linear SVM, MLP, LightGBM)
     - Perform 10-fold nested cross-validation
     - Generate and save results

6. Output files are saved to your Drive:
     - error_bar.png
     - learning_curves1.pdf

7. The complete run will take approximately one hour.

   You can view the results directly in HTML format
   Ensure Google Drive is mounted before running.
   Random seed is fixed (random_state=42) for reproducibility.


Google Drive for check: 
https://drive.google.com/drive/folders/16BsLStwhOewmc1N1Wl_H6-GRAKz-9k7J?usp=sharing 

GitHub Repository(Private):
https://github.com/Kinsley1219/comp90051_project_2025Oct.git


