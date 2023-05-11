![alt text](https://i.pinimg.com/originals/fc/3d/fa/fc3dfa2e7a902db1f7cc844c3a40f19d.jpg)
# Airline Customer Segmentation
### Airline customer segmentation with KMeans Clustering

**Introduction :**<br>
Suatu maskapai perusahaan ingin mengetahui bagaimana karakteristik umum dari customernya dengan cara membuat suatu customer segmentation. Segmentasi customer ini kemudian akan digunakan sebagai acuan dalam memutuskan keputusan bisnis selanjutnya, contohnya untuk menentukan promo yang sesuai dengan masing-masing segmentasi customer, atau campaign lain. 

Tentu jika digunakan dengan baik, segmentasi pelanggan ini dapat memberikan banyak keuntungan. Contohnya perusahaan dapat menekan marketing atau campaign cost karena dapat langsung memberikan treatment yang sesuai kepada tiap segmen customer, dan dengan treatment yang sesuai pasti campaign tersebut akan lebih mudah diterima oleh customer dan mendatangkan lebih banyak profit.

**Business Insight:**
* Angka customer yang ikut program FFP terus naik dari tahun ke tahun walaupun sempat turun pada tahun 2009 tetapi kembali naik pada tahun 2010, dan paling tinggi pada tahun 2012. 
* Terdapat penurunan customer yang sangat drastis pada tahun 2013, dimana sebelumnya angka customer selalu meningkat tiap tahunnya. <br>
![Alt text]('output1.png')

Perlu ditinjau kembali alasan penurunan customer pada 2013, jika melihat jumlah customer pada tahun 2012 yang sangat tinggi mengindikasikan terjadi hal penting yang menyebabkan penurunan drastis pada 2013.
* Penggunaan poin atau diskon customer masih terbilang rendah, hal ini mengindikasikan bahwa kampanye masih perlu ditingkatkan. Perlu ditinjau lagi apakah memang terdapat kendala seperti diskon yang diberikan kurang menarik di mata customer, atau campaign yang diberikan kurang sampai kepada customer, atau ada penyebab lain seperti proses penukaran poin yang rumit sehingga customer malas menggunakannya, dan sebagainya.

**Hasil Cluster yang terbentuk**
Terdapat 3 kelompok customer yang terbentuk, yaitu:
* CLUSTER 0 (Kelompok customer lama yang loyal) :
    * Customer merupakan customer lama
    * Customer masih menggunakan layanan maskapai, dilihat dari flight recency yang relatif baru
    * Customer memiliki frekuensi penerbangan tinggi
    * Customer cenderung sering melakukan perjalanan yang singkat
    * Customer menggunakan diskon yang tinggi
    * Dapat disimpulkan cluster ini merupakan kelompok customer loyal, jika dilihat dari angka rata-rata diskon yang diperoleh, pemberian diskon mungkin menjadi alasan customer bertahan menggunakan layanan maskapai ini, terlebih customer sering melakukan perjalanan dengan jarak dekat.
* CLUSTER 1 (Kelompok customer realtif baru) : 
    * Customer merupakan customer relatif baru jika dilihat dari durasi member dan flight recencynya
    * Customer masih menggunakan layanan maskapai, dilihat dari flight recency yang relatif baru
    * Customer memiliki frekuensi penerbangan rendah, hal ini mungkin karena memang customer baru bergabung member FFP dalam waktu dekat
    * Customer cenderung sering melakukan perjalanan dengan interval sedang
    * Customer menggunakan diskon yang rata-rata sedang
    * Dapat disimpulkan cluster ini merupakan kelompok yang relatif baru bergabung dengan maskapai.
* CLUSTER 2 (Kelompok customer lama yang relatif tidak aktif lagi) : 
    * Customer merupakan customer lama yang tidak lagi menggunakan layanan maskapai jika dilihat dari durasi member dan flight recencynya
    * Customer memiliki frekuensi penerbanganyang sangat rendah, hal ini mungkin karena memang customer hanya beberapa kali menggunakan layanan maskapai sebelum memutuskan untuk tidak menggunakannya lagi
    * Customer cenderung sering melakukan perjalanan dengan interval rendah atau jarak dekat
    * Customer menggunakan diskon yang rata-rata rendah
    * Dapat disimpulkan cluster ini merupakan kelompok yang kemungkinan hanya mencoba layanan maskapai beberapa kali dan berhenti menggunakan layanan. 

**Business Recommendation**

* Untuk customer pada cluster 0 (Customer loyal), perusahaan perlu untuk memberikan strategi yang bertujuan untuk menjaga loyalitas customer, seperti memberikan hadiah, diskon pelanggan, atau promo yang lebih menarik
* Untuk customer pada cluster 1 (Customer baru), perusahaan perlu untuk memberikan strategi yang bertujuan untuk menarik customer tersebut untuk terus menggunakan layanan maskapai pada masa depan, seperti promo buy 3 get 1 free ticket, atau kode referral untuk menarik customer agar terus menggunakan layanan dari perusahaan.
* Untuk customer pada cluster 2 (Customer lama yang berhenti berlangganan), perusahaan perlu berfokun untuk memberikan strategi agar customer  tertarik kembali untuk menggunakan layanan maskapai, seperti memberikan promo atau diskon khusus customer lama, atau memberikan diskon untuk penerbangan jarak dekat karena customer pada cluster ini cenderung melakukan penerbangan jarak dekat.