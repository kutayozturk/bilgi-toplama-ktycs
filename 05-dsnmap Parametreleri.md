-w  : wordlist belirterek alan adı taraması yapılır. Dosya yolu belirtilir.

```dnsmap google.com -w /temp/wordlist.txt```

-r  : Tarama sonuçlarını kaydetmek için kullanılır. Dosya yolu belirtilir.

```dnsmap google.com -r /temp/google.txt```

-d  : DNS sorgusu esnasından bantgenişliğini yormamak adına delay kontrolü yaparız. 500ms'de bir olmasını istersek

```dnsmap google.com -d 500```
