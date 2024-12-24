# ICP-HesapMakinesi

Bu proje, **Pelin İdil Güzel** tarafından Patika.dev Web3 Stajı kapsamında geliştirilmiştir. Motoko dilinde yazılmış bu uygulama, temel aritmetik işlemleri gerçekleştiren bir hesap makinesi işlevi görmektedir. Uygulama, **değişken yönetimi** ve **async fonksiyonlar** kullanılarak hesaplama işlemlerini etkin bir şekilde gerçekleştirmektedir.  

---

### Hakkımda  

Merhaba, ben Pelin İdil Güzel. Yazılım mühendisliği alanında kendimi geliştirmeye odaklanmış bir mühendis adayıyım. Şu anda **frontend geliştirme** ve **veri bilimi** gibi alanlarda çalışmakta ve yenilikçi projeler üretmekteyim. Patika.dev Web3 Stajı boyunca, Motoko dilinde uygulamalar geliştirerek teknik bilgi birikimimi artırmayı ve Web3 teknolojilerine yönelik derin bir anlayış kazanmayı hedefliyorum.  

---

### Proje Özellikleri  

Hesap makinesi, bir **aktör (actor)** yapısı kullanılarak Motoko dilinde geliştirilmiştir. Uygulama, bir `hucre` değişkenini kullanarak tüm işlemleri üzerinde gerçekleştirir ve aşağıdaki işlevleri sağlar:  

1. **Toplama**  
   - `toplama(s: Int): async Int`  
   - `hucre` değerine girilen sayıyı ekler ve sonucu döndürür.  

2. **Çıkarma**  
   - `cikarma(s: Int): async Int`  
   - `hucre` değerinden girilen sayıyı çıkarır ve sonucu döndürür.  

3. **Çarpma**  
   - `carpma(s: Int): async Int`  
   - `hucre` değerini girilen sayı ile çarpar ve sonucu döndürür.  

4. **Bölme**  
   - `bolme(s: Int): async ?Int`  
   - `hucre` değerini girilen sayıya böler ve sonucu döndürür.  
   - Sıfıra bölme kontrolü yapılır ve bu durumda `null` döndürülür.  

5. **Temizle**  
   - `temizle(): async ()`  
   - `hucre` değerini sıfırlar.  

---

### Kullanım Örnekleri  

1. **Toplama İşlemi**  
```motoko
let sonuc = await hesap_makinesi.toplama(5); // hucre: 5
```  

2. **Çıkarma İşlemi**  
```motoko
let sonuc = await hesap_makinesi.cikarma(2); // hucre: 3
```  

3. **Çarpma İşlemi**  
```motoko
let sonuc = await hesap_makinesi.carpma(4); // hucre: 12
```  

4. **Bölme İşlemi**  
```motoko
let sonuc = await hesap_makinesi.bolme(3); // hucre: 4
```  

5. **Sıfırlama**  
```motoko
await hesap_makinesi.temizle(); // hucre: 0
```  
