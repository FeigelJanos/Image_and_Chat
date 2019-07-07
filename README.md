# Image_and_Chat
Egyszerű képmegosztó chat funkcióval egyedi alkatrészgyártó cégek számára.

Funkciók:
- alkatrészkép tárolása
 - rajzi eszközök:ceruza és radír
 - projekten belöl több kép is feltölthető(galéria)
 
- alkatrészhez tartozó információk tárolása
 - az alkatrészhez tartozó adatok megadása személyre szabhatóak 
  - felülről megadhatók a kötelező adatok mezők
   - ezeket a projekten belül lehet módosítani is
   
- chat funkció
 - tartalma archiválásnál mentődik
 - chatszobák: céges szint, csoport szint, projekt szint


- felhasználóknak jogusultságokat lehet adni különböző projektekhez

- cégek nem szeretik ha az ügyfél látja a konkurenciát ezért egy meghívásos módszert kéne megoldani

- regisztrációnál megadjuk a céget, ha nem volt még ilyen cég akkor a regisztráló lesz a vezető
 
- projekt lezárása gomb megnyomása után lehetőség van rá hogy a projekt adatait archiváljuk


Adatbázis elemei:
  - Felhasználók
   - vezető <- minden projektet lát és módosíthat amik a cég neve alatt futnak, létrehozhat/törölhet projektet, hozzáadhat/eltávolíthat projektgazdát, hozzáadhat/eltávolíthat usereket, promotolhat/demotolhat akár vezető rangig
   - projektgazda <- minden projektet lát a cég neve alatt futnak, létrehozhat/törölhet saját projektet, hozzáadhat/eltávolíthat kapcsolattartót, hozzáadhat/eltávolíthat usereket, promotolhat/demotolhat projektgazdát rangig
   - user <- vezető/projektgazda állítja be a jogokat
   
  - Cég
    - Csoportok
  - Gépek
   - projektek
  - termékcsoport
   - termék
    -id
    -megnevezés
    -anyag

