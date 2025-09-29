# kimiafarma-performance-analytics

Repositori ini berisi query BigQuery dan hasil analisis terkait proyek Performance Analytics Kimia Farma periode 2020–2023.
Analisis dilakukan berdasarkan data transaksi, inventori, produk, dan kantor cabang yang disediakan, kemudian divisualisasikan dalam Google Looker Studio Dashboard.

📊 Dataset yang Digunakan
kf_final_transaction.csv → data transaksi pelanggan
kf_inventory.csv → data stok/inventori cabang
kf_kantor_cabang.csv → data cabang, kota, provinsi, dan rating cabang
kf_product.csv → data produk dan kategori

🛠️ Langkah Analisis
Import Dataset ke BigQuery
- Buat dataset kimia_farma
- Import keempat file .csv → jadikan tabel sesuai nama file
Membuat Tabel Analisa
- Query agregasi untuk menghasilkan tabel analisis dengan kolom:
transaction_id, date, branch_id, branch_name, kota, provinsi, rating_cabang, customer_name, product_id, product_name, actual_price, discount_percentage, persentase_gross_laba, nett_sales, nett_profit, rating_transaksi
Analisis Kinerja Bisnis
- Total pendapatan tahunan
- Top 10 cabang berdasarkan transaksi & nett sales
- Rating cabang vs rating transaksi
- Geo Map provinsi vs profit
- Analisis kategori produk
Dashboard di Looker Studio
- Visualisasi data analisis 2020–2023
