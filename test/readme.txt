Pagrindinis failas yra  atsakymu_tikrinimas.py. Pagrindinė idėja yra tai, kad žaidėjai atsiunčia 
surašytus atsakymus .txt formate. Tiesiog atsakymo variantas nuo 1 iki 5 ir skaičius. Faile turėtų
būti tik skaičių stulpelis be jokių kitų ženklų. Tarkim:

1
3
4
2

Šis failas pavadinamas žaidėjo vardu, apatiniu brūkšneliu ir turo skaičiumi. Tarkim: Dominykas_1, Inga_3 
(Dominyko pirmo turo atsakymai, Ingos trečio turo atsakymai).
Tuomet, šis failas yra sulyginamas su atsakymų .txt failu. Jo formatas yra teisingas atsakymas ir skiriami taškai. 
Turai skiriami paprastu brūkšniu. Pavyzdys yra GitHub, o jo interpratacija yra ši:
Pirmo turo pirmo klausimo atsakymas yra 1, už jį skiriamas 1 taškas. Pirmo turo 5 klausimo atsakymas yra 1, už jį skiriami 3 taškai. 
Už 4 turo 4 klausimą skiriami 2 taškai. Turai atskiriami –

Eiga:
1.	Excel faile „rezultatai“ surašomi žaidėjai nuo A2 stulpeliu žemyn.
2.	Python faile main() fukcijoje, players kintamajame surašomi tie patys žaidėjai.
pvz: players = ["dominykas", "petras", "jonas", "Inga", "Dovydas"]
3.	Kintamajame link nurodome kur yra pagrindinė direktorija su visais failais.
4.	Įsitikiname, kad excel failas išjungtas. Kitaip nepasileis python programa.
5.	Kai gauname visus failus su žaidėjų atsakymais, pakeičiam kintamąjį stage į dabartinį turą. Tarkim stage = 1, yra pirmas turas. Jeigu yra visi failai su žaidėjų vardais tokiais pačiais, kaip players kintamąjame ir jie sunumeruoti teisingai, programa turėtų pasileisti. Svarbu, kad players kintamajame žaidėjai būtų surašyti ta pačia tvarka, kaip excel faile.
6.	Paleidžiame programą. Konsolėje turėtumėm matyti ar žaidėjas atsakė teisingai. Jei atsakyta teisingai, skiriami taškai nurodyti atsakymų .txt faile. Kai viskas baigiasi, atsidarome excel failą.
7.	Vyksta kitas turas, gauname kito turo atsakymus .txt faile, pakeičiame stage = 2 (antras turas) ir viską kartojame. 

