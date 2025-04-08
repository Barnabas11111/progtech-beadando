# Rendszerterv
## 1. A rendszer célja
Autókereskedésnek az üzemeltetése.Kocsik vásárlása, eladása.
## 2. Projektterv

### 2.1 Projektszerepkörök, felelőségek:
  * Üzleti szereplő:
	  -   Megrendelő:
		  -  Herbák Marcell
     
### 2.2 Projektmunkások és felelőségek:
   * Frontend és backend:
     - Dinyési Barnabás Ákos
     - Kovács Bálint Benedek
   * Tesztelés:
     - Dinyési Barnabás Ákos
     - Kovács Bálint Benedek
     
### 2.3 Ütemterv:

|Funkció                  | Feladat                                | Prioritás | Becslés (nap) | Aktuális becslés (nap) | Eltelt idő (nap) | Becsült idő (nap) |
|-------------------------|----------------------------------------|-----------|---------------|------------------------|------------------|---------------------|
|Rendszerterv             |Megírás                                 |         1 |             1 |                      1 |                1 |                   1 |
|Program                  |Prototípus elkészítése                  |         2 |            10 |                     10 |                0 |                   0 |
|Program                  |Tesztelés                               |         3 |             1 |                      1 |                0 |                   0 |

### 2.4 Mérföldkövek:
   *   04.9. Projekt elkezdése
   *   04.14. Alap prototípus elkészítése
   *   04.23. Végleges prototípus elkészítése
   *   04.25. Tesztelés
   *   05.13. Bemutatás és átadás

## 3. Üzleti folyamatok modellje

### 3.1 Üzleti szereplők
Az alkalmazás regisztráció vagy bejelentkezés után válik elérhetővé, bárki tud regiszrálni. Minden felhasználó ugyanolyan jogkörrel rendelkezik.

### 3.2 Üzleti folyamatok
Az alkalmazás indulását követően a felhasználónak be kell jelentkeznie a funkciók eléréséhez.
- Általános folyamatok:
     - Regisztrálni az oldalra a megfelelő adatok magadásával.
     - Bejelentkezni az oldalra a regisztráció során megadott megfelelő adatokkal.
     - Bármikor kilépni az alkalmazásból.
     - Autó eladása.
     - Autó vétele.
- Autó vétele:
	- Árak megnézése.
	- Autó leírása.
	- Rendelés leadása.
  - Elérhetőség
- Autó eladása:
  - Fel kell rakni az autó képét és a leírást.
  - Ár beállítása.
  - Elérhetőség

## 4. Követelmények

### Funkcionális követelmények

| ID | Megnevezés                        | Leírás                                                                                             |
|----|-----------------------------------|----------------------------------------------------------------------------------------------------|
| K1 | Bejelentkezési ablak              | A felhasználónak egyes funkciók elérése előtt azonosítania kell magát, mielőtt elérhetné azokat.   |
| K2 | Regisztráció                      | A felhasználó itt tudja regisztrálni magát.                                                        |
| K3 | Autó vétel-eladás választás       | A fehasználó kiválaszthatja, mely játékmódot szeretné játszani.                                    |
| K4 | Autó vétele                       | Az autó megvásárlásánál a felhasználó megnézheti az autó árát,képeit, leírását, elérhetőséget.     |
| K5 | Autó eladása                      | Az autó eladásánal a felhasználó feltölti az autónak az adatait.                                   |
 
### Nemfunkcionális követelmények

| ID | Megnevezés                             | Leírás                                                                                                              |
|----|----------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| K6 | Átlátható, könnyen kezelhető felület   | A felületek könnyen használhatóak, átláthatóak legyenek, intuitívak, illetve ne legyenek zsúfoltak.                 |
| K7 | Tervezési minták használata            | Az alkalmazás forráskódja tartalmazzon legalább 3 tervezési mintát. Mi esetünkben ez a Stratégia és a Command lesz. |

### Támogatott eszközök

 * Bármely Java alkalmazás futtatásra képes eszköz. Például otthoni számítógép, laptop, tablet. Preferáltabb Windows alapú rendszer.

## 5. Funkcionális terv

### 5.1 Rendszerszereplők
 - Felhasználó
   - Autót adhat el és vehet meg.

### 5.2 Menühierarchiák
- Főoldal (Bejelentkezés és Regisztráció)
- Autó eladása
- Autó vétele

## 6. Fizikai környezet

### Vásárolt szoftverkomponensek, valamint esetleges külső rendszerek
Nincsenek vásárolt szoftverkomponensek.
### Hardver topológia
Olyan számítógép alkalmas, amely Windows 10 vagy 11 operációs rendszerrel rendelkezik.
### Fizikai alrendszerek
Kliens gépek: A követelményeknek megfelelő, Windows 10 vagy 11 operációs rendszerrel rendelkező PC-k.
Szerver (Host) gép: Az adatbázis rendszer és a háttérfolyamatokat ellátó szolgáltatáshoz szükséges összetevők itt találhatóak. A kliens gép ezzel kommunikál.
### Fejlesztő eszközök
 - IntelliJ IDEA
 - Visual Studio Code
 - XAMPP (MySQL)


## 8. Architekturális terv

### Webszerver

-XAMPP.

### Adatbázis rendszer

- MySQL alapú adatbázis rendszer.

### A program elérése, kezelése

- Szükséges Swing, XAMPP, ami az installáció esetén egy szervergép.


## 9. Adatbázis terv

![dbterv]([Dokumentumok/dbterv.png](https://github.com/Barnabas11111/progtech-beadando/blob/main/Dokumentumok/dbterv.png))

## 10. Implementációs terv
A projektet két részre oszlik: a frontendre és a backendre. A frontend Java Swing segítségével készül, míg a backend Java keretrendszerben.
A program kódjában használt nyelv elsősorban az angol.
A szerver és az adatbázist összekötő csomag  felelős az adatbázis kezeléséért.
Mind a frontend, mind a backend fejlesztéséhez szükség van a IntelliJ környezet telepítésére és konfigurálására a szükséges eszközökkel és kiegészítőkkel
együtt.
## 11. Tesztterv

A tesztelések célja a rendszer és komponensei funkcionalitásának teljes vizsgálata,
ellenőrzése a rendszer által megvalósított üzleti szolgáltatások verifikálása.
A teszteléseket a fejlesztői csapat minden tagja elvégzi.
Egy teszt eredményeit a tagok dokumentálják külön unit teszt függvényekbe és metódusokba tárolja.

A tesztelés során a szoftver megfelelő működését vizsgáljuk. Amennyiben az elvártnak megfelelő eredményt kapunk, a teszt eset sikeresnek tekinthető, ellenkező esetben a hibát megpróbáljuk elhárítani, ha a teszt nem direkt nem sikerül.

### Tesztesetek

#### Tesztelés módja: Unit Teszt

 | Teszteset          | Elvárt eredmény                                                                                            | 
 |--------------------|------------------------------------------------------------------------------------------------------------| 
 | Regisztráció       | A felhasználó az adatok megadásával sikeresen regisztrálni tud.                                            |
 | Bejelentkezés      | A felhasználó az adatok megadásával sikeresen be tud jelentkezni.                                          |
 | Autó megvásárlása  | Az autó adatai.                                                                                            |
 | Autó eladása       | Az eladás után valóban eltűnik-e a készletből az autó.                                                     |

## 12. Telepítési terv

**Fizikai telepítési terv**:
 - A felhasználónak szüksége van egy működő számítógépre, amely rendelkezik internet hozzáféréssel.
 - A szoftverünk működéséhez szükség van egy szerverre. A szervernek kapcsolódni kell egy hálózathoz, hogy elérhető legyen.

**Szoftver telepítési terv**:
 - A felhasználónak szüksége van egy Windows 10 vagy 11 operációs rendszerre, amely támogatja a Java alkalmazásokat.
 - A szoftverünk futtatható Windows szerveren.
 - Szükség van valamilyen adatbázis szerverre, például MySQL:
   - Szükséges telepíteni az XAMPP nevű szoftvert.
   - Az adatbázis konfigurálása az XAMPP segítségével történik.
 - A backend és frontend konfigurálásához szükség van az  IntelliJ fejlesztői környezetre.
   -  Szükséges csomagok a Java.
 - A fejlesztők számára az alkalmazás szabadon konfigurálható, fejleszthető.
 - Abban az esetben, ha a szükséges beállítások megtörténtek, a felhasználók számára az alkalmazás futtatható

## 13. Karbantartási terv
Fontos ellenőrizni:
*	Az alkalmazás megfelelően kezeli a kritikus információkat, azok nem elérhetők a megfelelő jogkör és felhasználói adatok nélkül. Ilyenek például a bejelentkezési adatok, és a felhasználók személyes adatai adatai.

Figyelembe kell venni a felhasználó által jött visszajelzést is a programmal kapcsolatban.
Ha hibát talált, mielőbb orvosolni kell, lehet az:
*	Működéssel kapcsolatos
*	Kinézet, dizájnnal kapcsolatos
