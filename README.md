# 1
(I would) like to learn


## Alapvetések
Az alapvetések célja, hogy egyértelmű alapokat biztosítson eldönteni, hogy hol állunk, merre megyünk, mit célzunk meg és mit nem a munkánkkal.

- olyan technológiát használunk, amit jelenleg programozóként a profik használnak és még jó darabig fejlődő képes marad (dotnet core)
- olyan eszközöket használunk amit jelenleg a profi programozók is használnak
- Olyan feladatot választunk amit nem kell terveznünk, már létezik és körbejárható
- A tervet úgy kéászítjük, hogy később továbbfejleszthető legyen

## Vázlat
Vázlatunk célja megnevezni az egymásra épülő alkalmazásainkat és megrajzolni az összefüggéseket.

- elsődleges célj: egy webalkalmazás készítése (MVC)
- továbbfejlesztés: az adatok szolgáltatása és az üzleti logika elérése webapin keresztül (MVC)
- továbbfejlesztés: desktop alkalmazás készítése a webapira alapozva (WPF)
-mobil alkalmazás készítése a webapira alapozva (Xamarin)
- továbbfejlesztés: SPA: Single Page Application készítése a webapira alapozva (Blazor)
 (Blazor webes keretrendszer C++-t futtat webes böngészőben)

## Webalkalmazás
Készítsünk egy (továbbfejleszthető) oktató alkalmazást, ahova
 - oktatók tudnak tanfolyamokta feltölteni, valamint
 - hallgatók tudnak ilyen tanfolyamokat elvégezni

 Ez egy jól áttekinthető, mégis kellően összetett feladat, ahol a full-stack C+ fejlesztés minden részébe bepillanthatunk, immár a profi fejlesztő szemével..




## DB
- legyen Entity Framework Core áltlal támogatott adatbázisok
( SQlite, MSMSQL )
( https://docs.microsoft.com/en-us/ef/core/providers/)
  - adatbázis tervezés és a telepítés
- [docker container] (https://hub.docker.com) támogatás
- kezdetben sqlite, majd kibővítjük MSSQL-re

- kockázatok
  - teljesítmény
  - relációs adatbázisok
  
  - https://netacademia.blog.hu/2016/06/21/a_muszaki_adossag_fogalma


## webgui
 - http kérés fogadása és válasz küldése MVC keretrendszer
 - felhasználó azonosítás (authentikation) 
 ASP.NET Core Identity 
 - Jogosultságkezelés (authorization)
 ASP.NET Core Identity 

 Adatok forgalmának biztosítása a bejövő adatok validálása
 MVC Viewmodel -al tudjuk validálni a beérkező adatokat

- Kockázatok
  - több alkalmazáson át elosztott bejelentkezés és jogosultságkezelés
    - Identity Server

## Repository
- CRUD műveletek elvégzése (**C**reate, **R**ead, **U**pdate, **D**elete )
- Listázás (Szűrés, sorbarendezés és lapozás)
- offline adatokat szolgáltat
Sosem ad vissza Iqueryable példányt
- adatmodelleket szolgáltat
külön kimeneti modell osztályokat nem fog használni.
- LINQ-t csak itt használunk.

- Kockázatok 
Nem azonosítunk itt ilyet.

## Service
- transzformáció az adatmodel és a Viewmodel között (Data mapping)
- Adatok validálása Viewmodel képességeit meghaladó esetben.
- Minden más amit eddig nem említettünk.

- kockázatok
Nem vettünk ilyet a nyakunkba

## Továbbiak
- decker containeres fejlesztési környezet
- visual studio code


