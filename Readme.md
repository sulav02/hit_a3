> **📌 Note: Setting Up File Location in Google Colab with Google Drive**
>
> This code is intended to run in **Google Colab** and access datasets stored in **Google Drive**.
>
> **Steps to set up:**
>
> 1. **Mount Google Drive**:
>    ```python
>    from google.colab import drive
>    drive.mount('/content/drive')
>    ```
>
> 2. **Set the file path**:
>    ```python
>    path = '/content/drive/MyDrive/ratvsbat/'
>    ```
>
> 3. **Upload your dataset files** (`dataset1.csv` and `dataset2.csv`) into the `ratvsbat` folder located in your Google Drive:
>
>    ```
>    My Drive/
>    └── ratvsbat/
>        ├── dataset1.csv
>        └── dataset2.csv
>    ```
>
> 4. **Load datasets** using:
>    ```python
>    df1 = pd.read_csv(path + "dataset1.csv")
>    df2 = pd.read_csv(path + "dataset2.csv")
>    ```
>
> ⚠️ **Troubleshooting**:  
> If you encounter a `FileNotFoundError`, ensure:
> - The folder name and file names are correct  
> - The files are uploaded to the correct Google Drive location

