# Kali Linux Araçlar ve Bilgi Toplama
## Nmap ve Zenmap
Nmap ve Zenmap, Kali Linux'ta etik hacking taraması için yararlı araçlardır.

Nmap ve Zenmap pratik olarak aynı araçlardır fakat, Nmap komut satırlarıyla çalışarak terminali kullanılır. Zenmap ise, grafiksel arayüze sahiptir.

Nmap ağ keşfi ve güvenlik denetimi için ücretsiz yardımcı bir araçtır.

Birçok sistem ve ağ yöneticisi, ağ envanteri, hizmet yükseltme zamanlarını yönetme ve ana bilgisayar himzet çalışma süresini izleme gibi görevler içinde yararlı bir araçtır.

## OS DEDECTION (İşletim Sistemi Tespiti)
nmap üzerinden tarama yaparken ```-O``` parametresi ile işletim sistemi tespiti yapmanız mümkündür.
```nmap -O 192.168.10.101```

## Açık Port Kontrolü
Nmap üzerinde açık TCP ve UDP portları bulunabilir.

Aşağıdaki komut ile tüm TCP bağlantı noktalarını tarayabilirsiniz.
```nmap -p 1-65535-T4 192.168.10.101```
Kodumuzdaki "-p" parametresi taranması gereken tüm TCP bağlantı noktalarını gösterirken, T4 parametresi tarama hızıdır.

## Nmap Shealt Scan (Nmap Gizli Tarama)
Gizli tarama veya SYN, TCP'nin üç yönlü anlaşmasını tamamlamadığı için **Yarı Açık Tarama** olarak da bilinir.

Saldırgan, hedefe bir SYN paketi gönderir ve bir cevap alınırsa hedefin bağlantıyı tamamlayacağı ve portun dinlendiği anlaşılır.

Hedeften bir cevap alınamazsa portun kapalı olduğu anlaşılır.

```nmap -sS -T4 192.168.10.101```

## DNS Araçları
### dnsenum.pl-
Bir domaine bağlı MX,A ve diğer kayıtları almaya yardımcı olan PERL Betiğidir.
```dnsenum <alanAdi>```

### dnsmap
dnsmap, aradığınız alan adına bağlı telefon numaralarını, kişileri ve diğer alt alanları bulamanıza yardımcı olur.
```dnsmap <alanAdi>```