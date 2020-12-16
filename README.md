**Uputstvo za decentralizovanu trgovinu BTC/RSD**

1. Preuzmite Electrum: https://electrum.org/#download (kliknite na "Standalone Executable" za najbrži način).

2. Pokrenite Electrum i klikćite "Next" sve dok se ne pojavi 12 reči u belom polju.

3. Kopirajte 12 reči u tekstualni fajl i sačuvajte ga. Kliknite "Next".

4. Upišite tih 12 reči, pa "Next" dva puta (lozinka nije potrebna).

5. Idite na "Tools" -> "Preferences" -> "Base unit" -> Izaberite "BTC".

6. Idite na "Tools" -> "Plugins" -> Čekirajte "Cosigner Pool".

7. Uđite u Telegram grupu: https://t.me/btc_bez_provizije

8. U polje za pretragu ukucajte "KBTC" da vidite ponude korisnika koji žele da kupe BTC, a "PBTC" da vidite ponude korisnika koji žele da prodaju BTC. Ako nema ponude koja Vam odgovara, napravite novu ponudu. Primer kako treba da izgleda ponuda ako želite da prodate BTC u vrednosti od 10000 dinara:
[PBTC][RSD10000]

9. Kada stupite u kontakt sa drugim korisnikom, dogovorite se čije bankomate ćete da koristite. Kupac mora da ima račun u nekoj od sledećih banaka: Raiffeisen, Komercijalna, OTP, Mobi, Unicredit ili AIK, osim u slučaju ako prodavac ima račun u Mobi banci - tad može da se koristi račun prodavca.

10. Idite na sajt (pomoćnik za lakšu trgovinu): https://btcrsd.github.io/

11. U polje na vrhu upišite dogovoreni iznos u dinarima. Kopirajte iznos u BTC i garanciju, pa pošaljite drugom korisniku radi potvrde. Ne gasite i ne osvežavajte sajt dok ne završite ceo proces.

12. U Electrum-u idite na "Receive" tab i kliknite dugme "New Address" (adresa je automatski kopirana).

13. Na tu adresu uplatite iznos prikazan u polju "Garancija" na sajtu.

14. U Electrum-u idite na Tools -> Sign/verify message i u polje "Address" paste-ujte adresu iz prethodnog koraka. A u polje "Message" upišite:
Ja, @moj_Telegram_username, prihvatam ponudu [KBTC][RSD20000] sa korisnikom @Telegram_username_korisnika_sa_kojim_trgujem

15. Pritisnite dugme "Sign". Kopirajte sadržaj sva tri polja i pošaljite drugom korisniku na proveru. Ne zatvarajte prozor.

16. U sva tri polja umesto Vaših ubacite podatke koje vam je poslao drugi korisnik i kliknite dugme "Verify". Neophodno je da se pojavi poruka "Signature verified".

17. Adresu drugog korisnika proverite u block exploreru po Vašem izboru (npr. blockchain.com), da utvrdite da se na njoj nalazi iznos garancije, isto kao na Vašoj adresi.

18. U Electrum-u zatvorite "Sign/verify message" prozor ako već niste, pa idite na File -> New/Restore i kliknite "Next".

19. Izaberite "Multi-signature wallet" i kliknite "Next".

20. Proverite da piše "From 2 cosigners" i "Require 2 signatures", ako ne piše, pomerajte slajdere da biste namestili tako. Kliknite "Next".

21. Izaberite "I already have a seed" i kliknite "Next". Paste-ujte 12 reči koje ste sačuvali u tekstualnom fajlu u koraku 3 i kliknite "Next".

22. Kopirajte "Master public key" i pošaljite ga drugom korisniku. Kliknite "Next".

23. Proverite da je izabrano "Enter cosigner key" i kliknite "Next".

24. Paste-ujte key koji ste dobili od drugog korisnika i kliknite "Next" dva puta (lozinka nije potrebna).

25. U novokreiranom multisig wallet-u idite na "Receive" tab i kliknite dugme "New Address" (adresa je automatski kopirana).

26. Vratite se u prethodni prozor Electrum-a gde ste prvobitno kreirali wallet.

27. Idite na "Send" tab. Paste-ujte adresu koju ste malopre kreirali u multisig wallet-u.

28. Kliknite dugme "Max", pa "Pay...", pa "Advanced", pa "Finalize".

29. **VAŽNO: Ovaj korak radi samo kupac!**  
Kliknite "Export" -> "Copy to clipboard", zatim "Close". Na Telegramu paste-ujte tekst prodavcu.

30. **VAŽNO: Ovaj korak radi samo prodavac!**  
Kopirajte tekst koji Vam je poslao kupac na Telegramu. Kliknite "Combine" -> "Join inputs/outputs", paste-ujte tekst i kliknite "Load transaction". Proverite ispravnost podataka i onda kliknite "Sign", pa "Export" -> "Copy to clipboard", pa "Close". Na Telegramu paste-ujte tekst kupcu.

31. **VAŽNO: Ovaj korak radi samo kupac!**  
Kopirajte tekst koji Vam je poslao prodavac na Telegramu. Kliknite "Tools" -> "Load transaction" -> "From text", paste-ujte tekst i kliknite "Load transaction". Proverite ispravnost podataka i onda kliknite "Sign", pa "Broadcast", pa "OK", pa "Close".

32. Sačekajte da transakcija ima jednu potvrdu na blockchain-u (kad odete na "History" tab, na levom kraju treba da bude ikonica sata). Nakon toga može da se pređe na sledeći korak.

33. **VAŽNO: Ovaj korak radi samo prodavac!**  
Idite do Vama najbližeg bankomata banke kupca. Kad dođete ispred bankomata, preko Telegrama tražite kod od kupca.

34. **VAŽNO: Ovaj korak radi samo kupac!**  
U svojoj bankovnoj aplikaciji upišite dogovoreni iznos u dinarima i generišite QR/bar kod, pa ga pošaljite prodavcu kao skrinšot/sliku. Eventualno možete da pošaljete i generisani broj u vidu teksta.

35. **VAŽNO: Ovaj korak radi samo prodavac!**  
Otvorite skrinšot ili poruku sa ciframa, na bankomatu odaberite funkciju podizanja keša bez kartice (konkretni nazivi te usluge se razlikuju od banke do banke) i zatim skenirajte ekran svog telefona ili otkucajte cifre na tastaturi bankomata. Preuzmite keš iz bankomata i vratite se kući.

36. Otvorite ponovo Electrum multisig wallet. Idite na "History" tab, zatim desni klik na transakciju, pa "Copy" -> "Balance". Vratite se u browser gde Vam je otvoren sajt iz koraka 10. Paste-ujte iznos u polje "Ukupno BTC u novčaniku".

37. Pripremite novu BTC adresu na koju ćete sebi isplatiti BTC iz zajedničkog (multisig) wallet-a.

38. **VAŽNO: Ovaj korak radi samo prodavac!**  
Pošaljite kupcu Vašu novu BTC adresu.

39. **VAŽNO: Ovaj korak radi samo kupac!**  
Otvorite Electrum multisig wallet, idite na "Send" tab i u polje "Pay to" unesite svoju BTC adresu. Vratite se u browser gde Vam je otvoren sajt pomoćnik. Kopirajte iznos iz polja "Za kupca". U Electrumu u polju "Pay to" nakon već unete Vaše BTC adrese stavite zarez, pa razmak, pa paste-ujte iznos "Za kupca". Zatim pritisnite "Enter" da biste dobili novi prazan red. Sada idite na Telegram i kopirajte BTC adresu prodavca, pa je paste-ujte u tom novom redu u polju "Pay to", pa stavite zarez, pa razmak, pa uzvičnik ("!"), što predstavlja ostatak novca. Pritisnite dugme "Pay...", pa prepišite "Mining fee" iznos na sajt pomoćnik u polje "Provizija". Sa sajta sada kopirajte novogenerisani iznos "Za kupca" i paste-ujte ga u Electrumu u "Pay to" polje na mesto prethodnog iznosa (biće veoma sličan). Sa sajta takođe kopirajte iznos iz polja "Provizija" i pošaljite ga prodavcu radi provere poklapanja svih iznosa. U Electrumu sada pritisnite dugme "Pay...", pa dugme "Advanced". Proverite adrese i iznose u "Outputs" polju - na Vašu BTC adresu treba da ide iznos "Za kupca". Pritisnite dugme "Finalize", pa dugme "Sign", pa dugme "Send to cosigner".

40. **VAŽNO: Ovaj korak radi samo prodavac!**  
Kopirajte iznos provizije koju Vam je poslao kupac na Telegramu i paste-ujte ga na sajtu u polje "Provizija". Kada kupac završi svoj deo procedure, iskočiće Vam prozor "An encrypted transaction was retrieved from cosigning pool...". Kliknite "Yes". U prozoru koji se pojavi dobro proverite sve podatke, da je tu Vaša BTC adresa i da se iznos za kupca podudara sa iznosom sa sajta pomoćnika. Pritisnite dugme "Sign", pa onda dugme "Broadcast", pa "OK", pa "Close".

41. Na Vašu novu adresu ste dobili BTC. Posle jedne potvrde na blockchainu, možete da obrišete dva iskorišćena Electrum wallet-a, uz prethodnu proveru u "History" tabu da je u wallet-u balans 0. Idite na "File" -> "Delete" -> "Yes" -> "OK". Ovim je decentralizovana BTC/RSD transakcija bez provizije uspešno završena!
