# RSB-Cer-evesi
BENİOKU.md
RSB Çerçevesi
Reverse Shell Backdoor, virüs bulaşmış makineleri bazı harika etkileşimlerle kontrol etmeye yönelik bir çerçevedir. Dosyaları gönderebilir, arka planda programları çalıştırabilir, ekran görüntüsü alabilir ve boktan şeyler yapabilir.

Kodun iki versiyonu vardır, C ve Python. Soketler ve ters bağlantı hakkında bilgi edinmek istiyorsanız, buna göz atmalısınız.

travis şubesi travis şubesi travis şubesi travis şubesi

Feragatname
Bu Çerçeve, başka bir kişinin bilgisayarına zarar vermek/tehdit etmek/zarar vermek için kullanılmamalıdır.

Amacı sadece Bilgisayar virüsü/İşletim Sistemleri/Programlama ile ilgili bilgi ve farkındalığı paylaşmak, güvenlik konusunda bilgi ve farkındalık oluşturmaktır.

Program tamamlanmadı veya tüm işlevler çalışmıyor.

Arka kapı nedir?
Arka kapı, truva atı olarak bilinen popüler bir bilgisayar virüsüdür. Kurban bilgisayara ters bir kabuk gibi çalışır. Böylece saldırgan, bazı sistem güvenlik açıklarından yararlanma ile köprüden sonra kurbanın bilgisayarına erişimini sürdürür.

Nasıl kullanılır ?
Önce kurban bilgisayarda derlenen arka kapıyı çalıştırmalıdır. Ardından, saldırgan servidor.py'yi çalıştırdığında, kurban bilgisayar bilgisayarıyla ters bağlantı elde edecektir.

Kurban:

python backdoor.py
Saldırgan:

python servidor.py
kullanımlar
Bir ters kabuk ile kurban bilgisayarı kontrol etmek için kullanılabilir.
Ayrıca evde olmadan kendi bilgisayarınızı kontrol etmek için de kullanılabilirsiniz!
Dosyaları gönderin ve indirin, programları çalıştırın.
Arka kapı özellikleri:
Uzak bağlantı.
Dosyaları kurban makineden indirin.
Dosyaları kurban makineye gönderin.
Sebat.
Kurban ekranının ekran görüntüsü.
Kurban bilgisayardaki diğer programları çalıştırın.
Arka kapı tamamlandı (Yalnızca tüm özellikler hazır olduğunda).
Kurulum
Python sürümünü çalıştırmak istiyorsanız, tüm bağımlılıkları yüklemeniz gerekir.

linux :

~$ sudo pip install -r requeriments.txt
pencereler :

pip install -r requeriments.txt
C kod sürümünü çalıştırmak istiyorsanız, herhangi bir bağımlılık yüklemeniz gerekmez.

derleme
Python kodunun bir betik olarak derlenmesi veya çalıştırılması gerekir ( önerilmez).

linux:

pyinstaller -F --clean -w backdoor.py -n backdoor
pencereler:

pyinstaller -F --clean -w backdoor.py -i icon.png
C kodunun derlenmesi gerekiyor .

~$ chmod +x comp.sh
~$ sh comp.sh
veya

~$ gcc backdoor.c lib/communication.c  lib/commands.c -o bin/client
~$ gcc server.c lib/communication.c lib/commands.c -o bin/server
