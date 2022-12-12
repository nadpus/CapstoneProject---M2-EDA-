## **Latar Belakang**

Sebuah perusahaan memiliki kumpulan data dari transaksi customer selama dua tahun terakhir. Perusahaan ingin melakukan *Customer Personality Analysis* terhadap populasi customernya agar dapat membantu perusahaan dalam membuat perencanaan penjualan yang lebih tepat dan *marketing campaign* yang lebih efektif.

## **Rumusan Masalah**

1. Bagaimana karakteristik customer yang membeli produk berdasarkan usia, pendapatan, status perkawinan, dan jumlah anak?
2. Bagaimana efektifitas campaign terhadap populasi customer?

## **Data Understanding**

Untuk menjawab rumusan masalah diatas, maka saya akan menganalisis data yang sudah dikumpulkan oleh perusahaan. Dataset dapat diakses pada xx[[sumber berikut]](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis). Dataset ini memiliki 29 variable yang dikelompokkan menjadi 5 kelompok dengan detail sebagai berikut:

* People
    - ID: ID unik customer
    - Year_Birth: Tahun lahir customer
    - Education: Level pendidikan customer
    - Marital_Status: Status pernikahan customer
    - Income: Pendapatan rumah tangga tahunan customer
    - Kidhome: Jumlah anak kecil yang dimiliki customer
    - Teenhome: Jumlah remaja yang dimiliki customer
    - Dt_Customer: Tanggal pendaftaran customer ke perusahaan
    - Recency: Jumlah hari sejak customer melakukan pembelian terakhir
    - Complain: 1 jika customer complain dalam 2 tahun terakhir, 0 sebaliknya
<br><br>
* Products
    - MntWines: Jumlah yang dibelanjakan untuk Wine dalam 2 tahun terakhir
    - MntFruits: Jumlah yang dibelanjakan untuk Buah dalam 2 tahun terakhir
    - MntMeatProducts: Jumlah yang dibelanjakan untuk Daging dalam 2 tahun terakhir
    - MntFishProducts: Jumlah yang dibelanjakan untuk Ikan dalam 2 tahun terakhir
    - MntSweetProducts: Jumlah yang dibelanjakan untuk produk Makanan Manis dalam 2 tahun terakhir
    - MntGoldProds: Jumlah yang dibelanjakan untuk Emas dalam 2 tahun terakhir
<br><br>
* Promotion
    - NumDealsPurchases: Jumlah pembelian yang menggunakan diskon
    - AcceptedCmp1: 1 jika customer menerima penawaran dari campaign ke-1, 0 sebaliknya
    - AcceptedCmp2: 1 jika customer menerima penawaran dari campaign ke-2, 0 sebaliknya
    - AcceptedCmp3: 1 jika customer menerima penawaran dari campaign ke-3, 0 sebaliknya 
    - AcceptedCmp4: 1 jika customer menerima penawaran dari campaign ke-4, 0 sebaliknya
    - AcceptedCmp5: 1 jika customer menerima penawaran dari campaign ke-5, 0 sebaliknya
    - Response: 1 jika customer menerima penawaran dari campaign terakhir, 0 sebaliknya
<br><br>
* Place
    - NumWebPurchases: Jumlah pembelian yang dilakukan melalui website perusahaan
    - NumCatalogPurchases: Jumlah pembelian yang dilakukan menggunakan katalog
    - NumStorePurchases: Jumlah pembelian yang dilakukan langsung di toko
    - NumWebVisitsMonth: Jumlah kunjungan ke website perusahaan dalam sebulan terakhir
<br><br>
* Others
    - Z_CostContact: Kolom irrelevan dengan dataset "Customer Personality Analysis"
    - Z_Revenue: Kolom irrelevan dengan dataset "Customer Personality Analysis"

## Data Wrangling

1. Handling missing values
2. Drop irrelevant columns
3. Feature engineering

## **Data Analysis**

Setelah data cleaning dilakukan, tahap selanjutnya adalah data analisis untuk dapat menjawab rumusan masalah dibawah ini yaitu:
1. Bagaimana karakteristik customer yang membeli produk berdasarkan usia, pendapatan, status perkawinan, dan jumlah anak?
2. Bagaimana efektifitas campaign terhadap populasi customer?

Dari rumusan masalah diatas, akan saya mendetailkannya menjadi beberapa business question sebagai berikut:
- Kelompok usia mana yang melakukan pembelian produk paling banyak dalam 2 tahun terakhir?
- Bagaimana `Expenses` dari masing-masing kelompok usia berdasarkan produk yang dibeli?
- Bagaimana hubungan korelasi antara `Expense` vs `Income` customer?
- Customer dengan `Marital_Status` seperti apa yang melakukan pembelian produk paling banyak dalam 2 tahun terakhir?
- Bagaimana hubungan korelasi antara `Expense`, `Income`, dan `Num_Children`?
- Pada channel manakah customer lebih banyak membeli produknya (web, catalog, store)?
- Bagaimana respon customer terhadap marketing campaign yang telah dibuat? 
