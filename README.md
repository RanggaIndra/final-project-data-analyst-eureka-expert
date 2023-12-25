# final-project-data-analyst-kel-II
Final Project Data Analyst
About Dataset
Context
Dataset Penyebab Kematian di Indonesia dikompilasi dalam bentuk file CSV untuk memudahkan analisis.

Content
Data dikompilasi berdasarkan data eksplisit yang disebutkan di dalam laporan. Tidak mengikutsertakan data estimasi dan data implisit (yang hanya menyebutkan "banyak", "sedikit", dicantumkan relatif terhadap populasi, multi-intepretasi, dll). Dataset ini terdiri dari 2 file, yaitu sbb:

"Penyebab Kematian di Indonesia yang Dilaporkan - Raw.csv" : berisi data yang dikompilasi dari Profil Kesehatan Indonesia Tahun 2004 s.d Tahun 2021 dan data COVID-19. URL sumber data tercantum pada kolom "Source URL". Kolom "Type" (Jenis Penyebab Kematian) diisi oleh saya sendiri, tidak berasal dari sumber yang telah disebutkan, namun terinspirasi dari Profil Kesehatan Indonesia Tahun 2019 yang membagi Krisis Kesehatan menurut Jenis Bencana, yaitu Bencana Sosial, Bencana Alam, dan Bencana Non Alam. Dalam konteks dataset ini, saya menggunakan 3 jenis seperti itu tapi sedikit dimodifikasi, yaitu menjadi: "Bencana Sosial", "Bencana Alam", dan "Bencana Non Alam dan Penyakit"
"Penyebab Kematian di Indonesia yang Dilaporkan - Clean.csv" : berisi data yang telah dibersihkan dari file "Penyebab Kematian di Indonesia yang Dilaporkan - Raw.csv", melalui metode: a) Untuk row data yang memiliki data redudancy yang lebih dari 1, dipilih data dari laporan tahun terakhir, dengan asumsi bahwa laporan tahun terakhir merupakan update/perbaikan terbaru dari data tahun yang lalu; b) Untuk row data yang memiliki data redudancy yang lebih dari 1 di tahun yang sama, dipilih data yang memiliki jumlah total paling besar. Dalam konteks validitas data, saya menyarankan Anda untuk menggunakan file "Clean" ini daripada file "Raw". File Raw tetap saya publikasikan untuk transparansi dan koreksi apabila ada informasi lebih lanjut dari Anda atau visitor lain.

from : https://www.kaggle.com/datasets/hendratno/cause-of-death-in-indonesia/data