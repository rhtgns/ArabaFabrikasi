KapiSayisiGir: Etiketi:

Bu etiket, kapı sayısının kullanıcıdan alındığı kod bloğunun başına yerleştirilmiştir.
Program akışında bu etikete geri dönmek için kullanılır.
Kapı Sayısını Girdirme:

Console.Write("Kapı Sayısı: "); satırı, kullanıcıdan kapı sayısını girmesini ister.
Kullanıcının girdiği değer kapiSayisiInput adlı bir string değişkende saklanır.
Sayısal Olup Olmadığını Kontrol Etme:

int.TryParse(kapiSayisiInput, out kapiSayisi) metodu, kullanıcıdan alınan string değerin bir tam sayı (int) olup olmadığını kontrol eder.
Eğer girilen değer bir tam sayıya dönüştürülebiliyorsa, bu değer kapiSayisi değişkenine atanır ve işlem devam eder.
Eğer girilen değer bir tam sayıya dönüştürülemiyorsa, TryParse metodu false döndürür.
Hatalı Giriş Durumunda Uyarı:

Eğer kullanıcı geçersiz bir değer girerse (örneğin "abc" gibi sayısal olmayan bir değer), if bloğu çalışır.
Console.WriteLine("Geçersiz kapı sayısı. Lütfen sayısal bir değer giriniz."); satırıyla kullanıcıya hatalı giriş yaptığı belirtilir.
goto KapiSayisiGir; Komutu:

Kullanıcı hatalı bir giriş yaptığında, program akışı goto komutuyla KapiSayisiGir etiketinin olduğu yere geri döner.
Böylece kullanıcıdan tekrar kapı sayısı girmesi istenir.
