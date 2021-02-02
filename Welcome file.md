# KS Geosinformatica - Kurs JS

## 1.  Wprowadzenie

### Omówienie języka

O Javascipcie można powiedzieć wiele rzeczy - interpretowany, luźno typowany, webowy. Każde z tych twierdzeń jest prawdziwe i nie jednocześnie. Programiści JS są tego typu ludźmi, jeśli można o nich tak powiedzieć , którzy lubią utrudniać sobie życie poprzez tworzenie nowych frameworkow, bibliotek i paczek każdego dnia jeśli nie co [godzine](https://dayssincelastjavascriptframework.com/).  Świetnym przykładem jest tego połączenie TypeScriptu oraz Electrona, które zaprzecza wszystkim trzem założeniom wspomnianym wcześniej.

A wiec czym jest JS? Jest językiem możliwości. Jeśli chcesz zrobić coś z zakresu programowania wysoko poziomowego, raczej uda ci się to zrobić. Od strony internetowej przez aplikacje desktopowe i mobilne po sterowanie urządzeniami fabrycznymi (zielonego pojęcia nie mam jak). Co w tym najlepsze? Często cześć kodu odpowiedzialna za _działanie_ aplikacji można przenieść bez większych problemów na nowa platformę, co pozostawia tylko cześć _wyglądową_ do napisania od nowa.

Zalety nie kończą się na uniwersalności. W standard wchodzą także takie koncepty jak closures, mixins, OOP, run-time evaluation, anonymous functions, promises, array comprehension i wiele wiele więcej. Większość zapewne wam nie mówi za dużo lub nie brzmi jak przełom w waszym życiu, ale jeśli faktycznie wejdziecie w JS to ... zapewne wciąż nie będzie to przełom. Są to wygodne udogodnienia które pomagają w codziennym programowaniu i mogę śmiało powiedzieć ze podczas pisania kodu w innych językach brakuje mi niektórych z wymienionych własności.

I tutaj dochodzimy do drugiej strony monety. Użyłem sformułowania "w standard" a nie "w listę cech języka". Javascript to tylko jedna z implementacji standardu ECMAscript, w dodatku nie zawsze zgodna. Nie każda linijka która napiszecie na silniku Node.js (który będzie głównym tematem kursu) zadziała w IE11 i vice versa. Istnieje dużo praktycznych implementacji języka javascript i czasami może się zdążyć ze ktoś użyje starszej przeglądarki lub silnika niż zamierzyliście i efekt waszej pracy pójdzie na marne, bo zamiast pochwały otrzymacie telefon o przełożonego, bo  przecież są błędy.

### NPM i inne takie
Ale koniec smęcenia i nudnej teorii - przejdźmy do kodu... no tak, npm. Co to takiego? Największy przyjaciel młodego programisty i największa zmora osoby która faktycznie stawia napisana aplikacje.

NPM, aka Node Package Manager, to program? system? do zarządzania bibliotekami, nazywanymi często w językach skryptowych jako paczki. Istnieją alternatywy, jak np `yarn` lub nakładki jak np `pnpm`, jednak podczas tego kursu będziemy używać czystego npm'a. Omawiając tylko npm'a można zapełnić tygodniowa konferencje, jeśli nie więcej, ale dla nas liczy się tylko kilka rzeczy:
 - Paczki instalowane są per projekt (aczkolwiek jest możliwość instalacji globalnej),
 - W oficjalnych repozytoriach znajdziemy bibliotekę prawie do każdej rzeczy która chcemy zrobić,
 - Instalacja biblioteki/paczki to proste `npm install <NAZWA> [<NAZWA2> ...]`.

Warto tez zauważyć, ze nie ma potrzeby zapełniania naszych repozytoriów na gicie setkami, tysiącami a czasami dziesiątakami tysięcy paczek - npm "zapamiętuje" jakie paczki powinny być zainstalowane w pliku `package.json`. Prosta komenda `npm install` (bez nazw paczek) sprawi, ze npm zainstaluje wszystkie paczki potrzebne lokalnie. 

### NODE

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ0NzUwMTY5OCwtODQ4NjU3NTAyLDE0NT
IwOTA4M119
-->