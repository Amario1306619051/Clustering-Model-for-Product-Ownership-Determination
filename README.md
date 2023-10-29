# Clustering Model for Product Ownership Determination

## Problem Statement
The problem at hand is to create an effective strategy for offering the right type of products to potential customers based on their demographics. The objective is to develop a clustering model to understand product ownership patterns based on the demographics of customers who are already using the FundFusion service, with a Silhouette Score greater than 0.7.

## Dataset
The dataset contains the following variables:

- **GCIF:** Unique Customer Identifier
- **Area:** Customer Location (Jakarta, Bogor, Bandung, Surabaya, Jogja, Solo)
- **Jalur_Pembukaan:** Customer's Product Opening Channel (Branch, Telemarketing, Digital Application, Internet Banking)
- **Vintage:** Duration as a Customer (Since opening the account)
- **Usia:** Customer Age
- **Jenis_Kelamin:** Gender (1 for Male, 0 for Female)
- **Status_Perkawinan:** Marital Status (0 for Unmarried, 1 for Married, 2 for Divorced, 3 for Widow/Widower)
- **Jumlah_Anak:** Number of Children
- **Pendidikan:** Highest Education Level (0 for No Formal Education, 1 for Elementary, 2 for Junior High, 3 for High School, 4 for Bachelor's, 5 for Master's, 6 for Doctorate)
- **Produk_Tabungan:** Savings Product Ownership (1 for Yes, 0 for No)
- **Produk_Deposito:** Deposit Product Ownership (1 for Yes, 0 for No)
- **Produk_Kartu_Kredit:** Credit Card Product Ownership (1 for Yes, 0 for No)
- **Produk_Kredit_Rumah:** Home Loan Product Ownership (1 for Yes, 0 for No)
- **Produk_Kredit_Kendaraan:** Vehicle Loan Product Ownership (1 for Yes, 0 for No)
- **Produk_Kredit_Dana_Tunai:** Personal Loan Product Ownership (1 for Yes, 0 for No)
- **Total_Kepemilikan_Produk:** Total Number of Owned Products
- **Pendapatan_Tahunan:** Average Annual Income
- **Total_Relationship_Balance:** Total Customer Assets in the Observation Month

## Experiment
In this project, we aimed to group customers based on demographics to identify product ownership patterns. We conducted the analysis from two perspectives:
1. Grouped by demographics to find product ownership patterns.
2. Grouped by product ownership to find demographic patterns.

## Data Preparation
We cleaned the dataset by addressing missing data, removing duplicates, and handling outliers. We specifically focused on customers who used the Telemarketing channel for the analysis.

The dataset was divided into three experiments:
1. Experiment 0: All Variables Used
2. Experiment 1: Demographics Only
3. Experiment 2: Financial-Related Variables Only

We applied one-hot encoding to categorical data and standardized numerical data. We also checked and removed highly correlated features.

## Modeling & Evaluation
We built clustering models using two algorithms:
1. K-Means
2. K-Medoid

We assessed the models using silhouette scores for different numbers of clusters. The scatter plots and statistics for each cluster were also analyzed to gain insights.

## Results
The clusters revealed distinct patterns in terms of demographics and product ownership. The results provide valuable insights for targeted product recommendations to different customer segments.

## Getting Started
1. Clone this repository.
2. Install the required packages listed in the 'requirements.txt' file.
3. Run the Jupyter Notebook to perform the analysis.

## Contributors
- AMARIO FAUSTA

## License
This project is licensed under the [Your License] License - see the [LICENSE](LICENSE) file for details.
