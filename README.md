# Automation Testing

## Izrada projekta

Scenarij ovog testa bio je provjeriti funkcionalnost web stranice, uključujući prijavu korisnika i rad košarice. 
Koristila sam Katalon Recorder za snimanje testova na temelju 6 testnih slučajeva. Nakon toga, koristila sam Visual Studio za kreiranje NUnit Test Projekta u kojem sam pomoću Selenium Webdrivera, NUnit frameworka, Test Adaptera te Chrome drivera (NuGet paketi), testirala dodanu testnu skriptu u C# (WebDriver + NUnit format) koju sam prije toga prilagodila. Pokretanje testa izvršila sam u Test Exploreru.

![image](https://user-images.githubusercontent.com/102880715/173625714-c9d553ca-2acf-4764-be2f-7128b64a5b59.png)

## Testni slučajevi

Kako bih istestirala te funkcionalnosti, kreirala sam 6 testnih slučaja koji su navedeni u nastavku: 

- Test ID:	1.1
- Area of functionality:	Modul za prijavu korisnika te  rukovanje košaricom
- Objective:	Provjera funkcionalnosti prijave korisnika i funkcionalnosti rada košarice
- Test case results:	6 testnih točki: 6 Pass, 0 Fail
- Note:	Korisnik je prethodno registriran	
					
Test seq. ID	Action taken	Precondition	Expected results	Pass/Fail	Note (in the case of "Fail")
1.	Korisnik u web preglednik upisuje https://www.saucedemo.com/	/	Korisnik je uspješno pristupio stranici.	Pass	
2.	Korisnik upisuje korisničko ime i lozinku.	Korisnik zna ime i lozinku.	Forma je ispravno popunjena.	Pass	
3.	Korisnik potvrđuje login potvrdom na gumb 'Login'.	Podatci su ispravno uneseni.	Prikazuje se Account korisnika.	Pass	
4.	Korisnik odabire proizvod dodajući ga u košaricu.	/	Proizvod je dodan u košaricu.	Pass	
5.	Korisnik pritisne ikonu košarice.	/	Korisnik je uspješno pristupio košarici.	Pass	
6.	Korisnik uklanja proizvod iz košarice.	Proizvod je dodan u košaricu.	Korisnik je uspješno uklonio proizvod iz košarice.	Pass	
