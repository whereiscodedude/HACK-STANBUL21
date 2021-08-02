# HACK-STANBUL21
Hackİstanbul'21 WriteUp

Hackİstanbul'21 Çözdügüm sorular ve çözemedigim birkaç soruyu içeren WriteUp'ım 

<h2>DETAİLED SEARCH-VT</h2>

Sorumuzda Detailed_Search.VT.txt uzantılı bir metin belgesi verilmekte metin belgesini açtıgımızda

![deta](https://user-images.githubusercontent.com/88288130/127787522-e9cf129b-a6b2-4bf1-9cac-1e68ec728ed1.JPG)

Şeklinde bir Sha-256 Şifrelemesi çıkıyor ilk başta şifrelemeyi kırmaya çalıştım kıramayacagımı anlayınca 
kırılmıyacak şifreyi vermezler herhalde diyerek bu işte bir iş var dedim 
googleda hash'i arattıgımda iexplorer.exe isimli dosyaya ait oldugunu fark ettim. farklı virüs tarama sitelerinde dosya mevcuttu
Sonrasında .txt uzantılı dosyamızın adında geçen VT sözcüğü dikkatimi çekti ve virüs totalden bahsettigini anladım.


![vt](https://user-images.githubusercontent.com/88288130/127787624-e1756a8e-aa75-4d33-a85e-f2a0b23ee40d.JPG)

Virüsü Totalde hash'i arattıgımda community kısmındaki yorum bizi bir pastebin linkine götürüyor.
linkten çıkan base64 tarzındaki şifreyi kırdıgımızda ise Flag'i ele geçiriyoruz.

<h2>Listen Well</h2>

Sorumuzda listen_Well.wav uzantılı ses dosyası verilmiş sesi dinledigimizde Mors alfabesi oldugunu anlıyoruz.
Online Mors Decoder ile decode ettigimizde Flag Karşımızda


![mors](https://user-images.githubusercontent.com/88288130/127787774-60746708-3631-45c2-84b4-6e9c6efc2555.JPG)

<h2>VAİL</h2>

Sorumuzda vail.txt uzantılı bir dosya içerisinde yine mors alfabesi ile yazılmış bir yazı görüyoruz.


![vail](https://user-images.githubusercontent.com/88288130/127787808-080db5ae-318d-407e-8f34-2b0b2a175be3.JPG)

Online Araçlar ile decode ettigimizde Flag karşımızda çıkıyor


![flag](https://user-images.githubusercontent.com/88288130/127787833-709ec5c5-b39f-4cc1-b8ba-297cccefc5da.JPG)

<h2>LİSTEN</h2>

Sorumuzda Şifreli zip arşivimiz ve Hist.wav uzantılı bir ses dosyamız var dinledigimizde anlamsız sesler oldugunu fark ediyoruz.
Aklımıza hemen Audio Stenegraph için sonicvisualizer'i açmak geliyor.Biraz karıştırdıgımızda ise sonuç


![LİSTEN](https://user-images.githubusercontent.com/88288130/127787924-de9e8d55-a84c-431f-a37f-3b5cc6d11d3a.JPG)


Ses dosyamızdaki metni Şifreli zip arşivimize giriyoruz hist.flag uzantılı dosyamızı metin belgesiyle açtıgımızda flag karşımızda

<h2>H3X</h2>
Sorumuzda bir .png uzantılı resim veriliyor string ettigimizde içinde gömülü bir dosya barındırdıgına dair ipuçları görüyoruz binwalk -e komutumuz ile extract ettigimizde
çıkan dosya içinde flag'imizi buluyoruz. (Affola Detayları unuttum)

<h2>ZİPPED FLAG</h2>
Sorumuzda zipped_flag.zip adında birbiri içine arşivlenmiş arşivler verilmiş string ettigimizde 2021 tane arşiv bulundugunu görüyoruz basit bir bash kodu ile

<code>#!/bin/bash

unzip zipped_flag.zip
for ((direct=1; direct>=1; direct++))
do
        read -r side < direction.txt
        unzip -o "$direct$side.zip"
done</code>

arşivleri açtıgımızda hex.zip isimli son bir zip ve içinden flag.exe isimli bir dosya çıkıyor
  
  
![hexa](https://user-images.githubusercontent.com/88288130/127789245-3fa5acdb-2a70-4c26-874c-932ea1678696.JPG)
  
string ettigimizde hexadecimal türünde verilen hash'imizi kırıyoruz ve flage ulaşıyoruz.
  

  <h2>Find Restoraunt</h2>
  
  Sorumuzda bir restorantın önüne ait resim verilmiş açıklamada ise belki yorumlar yardımcı olur yazılmıştı dogal olarak google görsel arama yaptıgımızda resimdeki restorant'ın
  internetten satış yaptıgı sayfasına ulaşıyoruz restorant yorumlarında ise flag'imiz bizi bekliyor ama biraz manipule edilmiş ve birde ipucu dilenilmiş şekilde :D
  ![hasd](https://user-images.githubusercontent.com/88288130/127789380-5fe974a5-f20f-4636-aab5-47ff802df0d9.JPG)

  <h2>B2B21</h2>
  
 Sorumuzda yine birbiri içine gömülmüş bu sefer .tar uzantılı arşivlere rastlıyoruz yine basit bir bash betiği ile dosyaları açmaya başlıyoruz dosyaları açtıgımızda bir adet .gpg dosyası ve A-B-C-D şeklinde her klasörde bu seferde iç içe zip dosyalarına rastlıyoruz.
  
  ![tar](https://user-images.githubusercontent.com/88288130/127789519-d4cee71e-ab1f-4ab7-9abd-3af3e50138c8.JPG)

  Klasörlerdeki arşivleri açtıgımızda F Klasörü içinde flag.exe uzantılı bir dosyanın arşive şifrelendigini görüyoruz ben buraya kadar gelebildim burdan ilerisinde ne bir ipucu  ne bir şifre bulamadım soruyu çözemedim.

  <h2>Where Am I</h2>
  
  Sorumuzda katar uçagına ait bir resim veriliyor açıklamaya resimdeki uçagın hangi havalimanına indigini ögrenmek isteyen bir muhabir oldugu söyleniyor google görsel aramalar ile uçagı buldugumuzda farklı haber sitelerinde Şanlıurfa havalimanına indigi söyleniyor şanlıurfa havalimanının ismini hiçbir şekilde flag olarak kabul etmedi haber sitelerini tek tek gezerek yorumlarda ipuçları bulmaya çalışsamda birşey bulamadım bu soruyuda çözemedim. 
  
  
 <h1>Yarışmaya tek katıldıgım için diger sorulara detaylı bakamadım .pcap soruları bana zor geldi ram imajı sorusunuda imajı açacak tool'u çeşitli hatalardan dolayı yükleyemedigim için hiç göremedimki içerigini en çok merak ettigim soruydu .png şeklinde verilen sorularda ise tool eksikligim dolayısıyla pek detay çıkartamadım hazırlıklı gelmiş arkadaşlar için gayet kolay bir ön eleme oldu. Yarı finalde yarışmacılara başarılar diliyorum</h1>

