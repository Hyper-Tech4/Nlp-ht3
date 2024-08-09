##A.VERİSETİ_HAZIRLIĞI

  Friends veri setinin kaynak linki: https://edersoncorbari.github.io/friends/

  Kaynaktan her sezon için ayrı bir text dosyası oluşturuldu. Bu dosyalar translate aracılığıyla türkçeye çevirildi. Text dosyalarını diyalog dışı cümlelerden ayılması, tek bir merged_friends.txt dosyası haline getirilmesi ve bu dosyanın friends.csv dosyası haline getirilebilmesi için veriseti_hazırlık.ipynb kodu kullanıldı.

##B.MODEL

  "Friends" dizisindeki karakterlerin diyaloglarını tahmin etmek için gömülü embedding kullanarak modeli [karakter tahminini](kod/KarakterTahmini.ipynb ) gerçekledik. Aşağıda modelin accuracy değerleri çıktısı verilmiştir.
  <img width="1004" alt="Screen Shot 2024-08-09 at 12 48 48" src="https://github.com/user-attachments/assets/e9402112-7a2c-48d5-bdab-e3aeba9456bb">

Pretrained embedding modeli olan [Word2Vec](kod/word2vec.ipynb) ile
eğittiğimiz model. Aşağıda modelin accuracy değerleri çıktısı verilmiştir.
  <img width="1008" alt="Screen Shot 2024-08-09 at 12 52 06" src="https://github.com/user-attachments/assets/aa460ad8-7166-4700-b77a-262db47d1059">


  Modelin belirli [karaktere göre cümle üretimi ve tahmini](kod/karaktere-gore-cumle-uretimi-ve-cumle-tahmini.ipynb) yapıldı.  Aşağıda modelin accuracy değerleri çıktısı verilmiştir

  <img width="801" alt="Screen Shot 2024-08-09 at 13 03 28" src="https://github.com/user-attachments/assets/9da20495-0fd3-4cb2-bca0-bbb9313a20df">

<img width="706" alt="Screen Shot 2024-08-09 at 13 05 23" src="https://github.com/user-attachments/assets/2e843773-740b-4ae8-af63-7f6cc7b0056d">

  
<img width="926" alt="Screen Shot 2024-08-09 at 13 03 39" src="https://github.com/user-attachments/assets/b83e41e1-bd80-47cf-81ff-8df56d35deba">


Modelimizi seçtiğimiz karakterlerin en sık ([frekans](url)) kullandığı kelimeleri verisetinden çıkararak cümle üretme [accuracy değerinin arttırıldığı model](kod/cumle_uretme_gelistirilmis.ipynb).


###YARDIMCI KODLAR

Seçtiğimiz "Rachel" ve "Chandler" karakterlerinin [en sık](kod/karakter_diyalog_kelime_frekans.ipynb) kullandığı kelimeler:


<img width="690" alt="Screen Shot 2024-08-09 at 13 13 54" src="https://github.com/user-attachments/assets/5cc4e87e-d25d-4daf-a5d5-a9a8d3fa7a99">


<img width="704" alt="Screen Shot 2024-08-09 at 13 14 03" src="https://github.com/user-attachments/assets/05d6c3a2-ba98-404d-9df4-c42a1712e739">

Modelin genelleştirme yeteneğini artırmak için kullanılan teknikler [bu dosyadadır](kod/overfitting_ornegi.ipynb).
  

<img width="962" alt="Screen Shot 2024-08-09 at 13 16 18" src="https://github.com/user-attachments/assets/f0c31043-5068-477c-a1c0-8db93cf07d19">


  
