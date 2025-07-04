# Differentiated Thyroid Cancer Recurrence Exploratory Data Analysis

## Deskripsi Proyek

Proyek ini bertujuan untuk melakukan **eksplorasi data visual (EDA)** terhadap kumpulan data *Differentiated Thyroid Cancer Recurrence* dari [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/915/differentiated+thyroid+cancer+recurrence).

Dataset ini mencakup **16 fitur klinikopatologis** yang digunakan untuk memprediksi kemungkinan **kekambuhan kanker tiroid berdiferensiasi**. Data dikumpulkan selama **15 tahun**, dan setiap pasien dipantau selama minimal **10 tahun**.

## Tujuan Analisis

* Mengetahui distribusi variabel demografis dan klinis pasien.
* Mengidentifikasi korelasi antar fitur kuantitatif.
* Menganalisis hubungan antar fitur kategorikal dengan target `Recurred`.
* Menyediakan insight visual untuk pemodelan prediktif ke depan.

## Teknologi & Library

* Python 
* `pandas`, `numpy`, `matplotlib`, `seaborn`
* `sklearn.preprocessing.LabelEncoder`
* `math`, `itertools`, `re`
* Jupyter Notebook

## Eksplorasi Data (EDA)

### 1. **Univariate Analysis**

* **Numerik**: Distribusi umur (`Age`) melalui histogram, boxplot, dan violin plot.
* **Kategorikal**: Frekuensi distribusi untuk fitur-fitur seperti `Gender`, `Smoking`, `Stage`, `Risk`, dll.

### 2. **Multivariate Analysis**

* **Quantitative vs Quantitative**:

  * Korelasi antar variabel numerik dengan *heatmap* dan *scatterplot matrix*.
* **Quantitative vs Categorical**:

  * Boxplot dan LMPlot: `Age` terhadap variabel kategorikal dan `Recurred`.
* **Categorical vs Categorical**:

  * Countplot antar kombinasi fitur kategorikal terhadap target `Recurred`.

## Insight 

* Pasien dengan **tingkat risiko tinggi** menunjukkan proporsi kekambuhan yang lebih besar.
* Umur pasien berpengaruh terhadap kemungkinan kekambuhan, namun tidak secara linear.
* Fitur seperti `Stage`, `Risk`, `Response`, dan `Pathology` menunjukkan korelasi kuat dengan target `Recurred`.
