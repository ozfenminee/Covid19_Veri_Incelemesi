Bu proje, COVID-19 dönemine ait akademik makalelerin meta verilerini içeren metadata.csv adlı veri seti üzerinde temel veri analizi yapılmasını amaçlamaktadır. Veri seti, makalelerin başlıkları, yazarları, yayımlandığı dergi, yayın tarihi ve özet gibi bilgileri barındırır.

🎯 Hedefler
Veri setinin genel yapısını keşfetmek

Eksik değerlerin tespiti ve yönetimi

Yayınların yıllara göre dağılımını analiz etmek

En aktif yazarları, dergileri ve kaynakları tespit etmek

Görselleştirmelerle bilgiyi anlaşılır hale getirmek

📁 Kullanılan Veri Seti
Dosya Adı: metadata.csv
Kaynak: CORD-19 Dataset
Sütunlar:

cord_uid, sha, source_x, title, doi, pmcid, pubmed_id

license, abstract, publish_time, authors, journal

mag_id, who_covidence_id, arxiv_id, pdf_json_files, pmc_json_files

url, s2_id

🧰 Kullanılan Teknolojiler
Python (Jupyter Notebook)

Pandas

Matplotlib

Seaborn

NumPy

📊 Yapılan Analizler
📌 Veri setinin ilk 5 satırının görüntülenmesi

📌 Eksik değer analizi (isnull().sum())

📌 En çok kullanılan dergilerin ve kaynakların listelenmesi

📌 Yayınların yıllara göre dağılımı (publish_time)

📌 En çok katkıda bulunan yazarların bulunması

📌 DOI, başlık ve özet gibi metin sütunlarında benzersiz kayıt sayılarının incelenmesi

📈 Örnek Görselleştirmeler
Yayın sayısının yıllara göre dağılımı (bar chart)

En aktif yazarların katkı sayısı (value_counts)

📑 Nasıl Çalıştırılır?
Jupyter Notebook ortamında metadata.csv dosyasını aynı klasöre koyun.

Aşağıdaki kütüphanelerin yüklü olduğundan emin olun:

bash
Kopyala
Düzenle
pip install pandas numpy matplotlib seaborn
Notebook'u çalıştırın ve hücreleri sırasıyla yürütün.

📌 Notlar
low_memory=False parametresi ile veri türü karışıklıkları önlendi.

publish_time sütunu datetime tipine çevrilerek analiz edildi.

Özellikle eksik özet (abstract) verileri yaygın olduğundan bu durum analizde dikkate alındı.
