# Capstone-Project-3-Telco-Customer-Churn

## BUSINESS UNDERSTANDING

### Business Context
Dalam industri telekomunikasi, churn terjadi ketika pelanggan berhenti menggunakan layanan seperti internet atau telepon, yang menyebabkan penurunan pendapatan dan peningkatan biaya untuk mendapatkan pelanggan baru. Dengan persaingan yang ketat, memahami dan memprediksi churn sangat penting untuk mempertahankan pelanggan dan menjaga profitabilitas bisnis.

Target : 
0 : Tidak berhenti berlangganan 
1 : Berhenti berlangganan (churn)

### Problem Statement :

Memperoleh pelanggan baru jauh lebih mahal daripada mempertahankan pelanggan yang sudah ada. Biaya untuk mengakuisisi pelanggan baru bisa mencapai lima kali lipat lebih mahal daripada mempertahankan pelanggan yang sudah ada. Biaya Akuisisi Pelanggan (CAC) dalam industri telekomunikasi bervariasi, tetapi biasanya sekitar $315 per pelanggan. Angka ini menunjukkan biaya rata-rata yang dikeluarkan perusahaan telekomunikasi untuk mendapatkan pelanggan baru, termasuk biaya pemasaran dan penjualan. (Source: [Article 1](https://startuptalky.com/cac-by-industry/) & [Article 2](https://www.revechat.com/blog/customer-acquisition-cost/)).<br>

Mempertahankan pelanggan yang sudah ada umumnya lebih murah. Hal ini melibatkan pemeliharaan kepuasan dan loyalitas melalui layanan pelanggan, pemasaran yang dipersonalisasi, dan keterlibatan yang berkelanjutan. Strategi retensi yang kuat dapat menghasilkan laba atas investasi yang lebih tinggi. Sebagai contoh, peningkatan retensi pelanggan sebesar 5% dapat meningkatkan keuntungan sebesar 25% hingga 95%.(Source: [Article 3](https://www.paddle.com/resources/customer-acquisition-vs-retention) & [Article 4](https://www.wellnessliving.com/blog/customer-retention-vs-customer-acquisition-which-better/))​.

Kesimpulannya, kehilangan pelanggan memaksa perusahaan untuk mendapatkan pelanggan baru, yang lebih mahal daripada mempertahankan pelanggan yang sudah ada melalui strategi tertentu. Dengan demikian, perputaran pelanggan bisa sangat merugikan perusahaan.

### Goals :

1. Memprediksi pelanggan mana yang mungkin akan berpindah (churn). Dengan demikian, potensi kehilangan pendapatan dan Biaya Akuisisi Pelanggan (CAC) dapat diminimalisir.
2. Mengetahui faktor-faktor apa saja yang cenderung mempengaruhi pelanggan bertahan, sehingga mereka dapat membuat program-program yang lebih tepat sasaran dalam mengurangi jumlah pelanggan yang churn

### ML Objective

Membuat model prediktif untuk mengidentifikasi pelanggan yang berisiko melakukan churn. Dengan melatih data historis, model akan mengenali pola yang terkait dengan churn dan menggunakan wawasan ini untuk memprediksi kejadian churn di masa depan. Tujuannya adalah untuk mencapai F2 Score yang tinggi dalam prediksi dengan False Negative (FN) yang rendah, memastikan perusahaan dan pemangku kepentingan dapat bergantung pada model untuk pengambilan keputusan yang tepat.

### Analytic Approach :

1. Menganalisis data untuk menemukan pola yang membedakan pelanggan yang akan berhenti berlangganan (churn) atau tidak.
2. Membangun model klasifikasi yang akan membantu perusahaan untuk dapat memprediksi probabilitas seorang pelanggan akan berhenti berlangganan (churn) atau tidak.

### Metric Evaluation

Kami akan menggunakan F2 Score karena kami tertarik dengan False Negative dan False Positive, namun lebih menitikberatkan pada False Negative karena lebih mahal.

- Type I Error/ False Positive (FP): Jika pelanggan diprediksi akan churn, namun ternyata bertahan.
- Type II Error / False Negative (FN): Jika Pelanggan diprediksi akan bertahan, namun ternyata churn.
