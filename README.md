# Employee Attrition
## Tujuan
- Mengidentifikasi faktor - faktor yang berpengaruh terhadap berhentinya karyawan di IBM
- Membuat model untuk memprediksi karyawan yang akan resign

## Data Understanding
- Data Source: Kaggle 
https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset?datasetId=1067&sortBy=voteCount
- Packages: Pandas, Numpy, Matplotlib, Seaborn, Sklearn
- Dataset punya 35 kolom dan 1.470 baris

## Data Cleansing
- Tidak ada missing dan duplicate value
-	'EmployeeCount', 'Over18', 'StandardHours' hanya ada 1 unique value dan 'EmployeeNumber' punya 1470 unique values. Kolom ini tidak akan digunakan untuk analisa jadi bisa di drop.
- Imbalanced dataset karena 1233 (84%) karyawan masih bekerja di perusahaan sedangkan 237 (16%) karwayawan resign dari perusahaan

## Exploratory Data Analysis
- Laki – laki yang berhenti bekerja lebih banyak dibanding perempuan
- Laboratory Technician, Research Scientist, dan Sales Executive merupakan job role yang karyawannya paling banyak berhenti 
- Karyawan yang paling banyak berhenti dari Departemen Research dan Development 
- Karyawan berusia muda cenderung berhenti dari perusahaan dibanding karyawan yang berusia tua

Model yang dipilih adalah recall tinggi (69%) untuk menghilang false negative karena lebih baik orang yang diperkirakan resign namun ternyata tidak resign (false positive) daripada diperkirakan tidak resign namun ternyata resign (false negative)
