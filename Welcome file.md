# KS Geosinformatica - Kurs JS

## 1.  Wprowadzenie

### Omówienie języka

O JavaScripcie można powiedzieć wiele rzeczy - interpretowany, luźno typowany, webowy. Każde z tych twierdzeń jest prawdziwe i nie jednocześnie. Programiści JS są tego typu ludźmi, jeśli można o nich tak powiedzieć, którzy lubią utrudniać sobie życie poprzez tworzenie nowych frameworkow, bibliotek i paczek każdego dnia jeśli nie co [godzinę](https://dayssincelastjavascriptframework.com/).  Świetnym przykładem jest tego połączenie TypeScriptu oraz Electrona, które zaprzecza wszystkim trzem założeniom wspomnianym wcześniej.

A więc czym jest JS? Jest językiem możliwości. Jeśli chcesz zrobić coś z zakresu programowania wysoko poziomowego, raczej uda ci się to zrobić. Od strony internetowej przez aplikacje desktopowe i mobilne po sterowanie urządzeniami fabrycznymi (zielonego pojęcia nie mam jak). Co w tym najlepsze? Często cześć kodu odpowiedzialna za _działanie_ aplikacji można przenieść bez większych problemów na nową platformę, co pozostawia tylko cześć _wyglądową_ do napisania od nowa.

Zalety nie kończą się na uniwersalności. W standard wchodzą także takie pojęcia jak closures, mixins, OOP, run-time evaluation, anonymous functions, promises, array comprehension i wiele więcej. Większość zapewne wam nie mówi za dużo lub nie brzmi jak przełom w waszym życiu, ale jeśli faktycznie wejdziecie w JS to ... zapewne wciąż nie będzie to przełom. Są to wygodne udogodnienia, które pomagają w codziennym programowaniu i mogę śmiało powiedzieć ze podczas pisania kodu w innych językach brakuje mi niektórych z wymienionych własności.

I tutaj dochodzimy do drugiej strony monety. Użyłem sformułowania "w standard" a nie "w listę cech języka". Javascript to tylko jedna z implementacji standardu ECMAscript, w dodatku nie zawsze zgodna. Nie każda linijka, która napiszecie na silniku Node.js (który będzie głównym tematem kursu) zadziała w IE11 i vice versa. Istnieje dużo praktycznych implementacji języka javascript i czasami może się zdążyć ze ktoś użyje starszej przeglądarki lub silnika niż zamierzyliście i efekt waszej pracy pójdzie na marne, bo zamiast pochwały otrzymacie telefon o przełożonego, bo  przecież są błędy.

### NPM i inne takie
Ale koniec smęcenia i nudnej teorii - przejdźmy do kodu... no tak, NPM. Co to takiego? Największy przyjaciel młodego programisty i największa zmora osoby, która faktycznie stawia napisana aplikacje.

NPM, aka Node Package Manager, to program? system? do zarządzania bibliotekami, nazywanymi często w językach skryptowych jako paczki. Istnieją alternatywy, jak np. `yarn` lub nakładki jak np. `pnpm` jednak podczas tego kursu będziemy używać czystego NPM'a. Omawiając tylko NPM'a można zapełnić tygodniowa konferencje, jeśli nie więcej, ale dla nas liczy się tylko kilka rzeczy:
 - Paczki instalowane są per projekt (aczkolwiek jest możliwość instalacji globalnej),
 - W oficjalnych repozytoriach znajdziemy bibliotekę prawie do każdej rzeczy, która chcemy zrobić,
 - Instalacja biblioteki/paczki to proste `npm install <NAZWA> [<NAZWA2> ...]`

Warto też zauważyć, ze nie ma potrzeby zapełniania naszych repozytoriów na gicie setkami, tysiącami a czasami dziesiątakami tysięcy paczek - npm "zapamiętuje" jakie paczki powinny być zainstalowane w pliku `package.json` Prosta komenda `npm install` (bez nazw paczek) sprawi, że NPM zainstaluje wszystkie paczki potrzebne lokalnie. 

### Node.js
No i kwintesencja naszego kursu - Node. Jest to de facto "sposób" aka interpreter, którego będziemy używać do odpalania naszego kodu. Nie będę się wypowiadał za dużo na jego temat, bo to wprowadzenie było wystarczająco długie, a kod się sam nie napisze. Dla nas liczy się to, że brakuje mu niektórych funkcjonalności, które posiada "przeglądarkowy" js, nadrabia gigantyczną ilością dużo bardziej przydatnych bibliotek i API (wspomniałem ze nie lubię pisać w JS przeglądarkowym?).

## 2.  Środowisko

###  Node i NPM

Teoria teorią, ale co my właściwie potrzebujemy zainstalować na komputerze, żeby pisać jakiś kod? Node i NPM! Zazwyczaj instalujemy je razem jednym instalatorem/ w jednej paczce. Instalator dla Windowsa oraz MacOS można znaleźć [tu](https://nodejs.org/en/download/). Na Linuxie instalujemy za pomocą ulubionego managera paczek.

### Edytor
Kwestia edytora jest podobna do kwestii ulubionego ciasta. Każdy jest dobry, ale każdy ma swój ulubiony. Osobiście mogę polecić WebStorm od firmy JetBrains. Posiada on natywne wsparcie dla wielu technologii jak i nawet przyzwoity zestaw pluginów, mimo że zdecydowanie ich nie potrzebuje.

Z innych dobrych edytorów mogę polecić Visual Studio Code, Atom lub Sublime (tylko z opinii), jednakze kazde z tych rozwiazan wymaga dodania znaczej ilosci dodatkow zeby dogonic WebStorm'a, ale daje nam to takze mozliwosc 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTUwNzQ5NzI4Nyw1NjY5MDQ0NDksMjAxOT
U5NjcwNSwtMjE0NjQ4OTc3MywtMTg1Njc5MjY2OCwtNjYyNzQ4
NTE5LC04NDg2NTc1MDIsMTQ1MjA5MDgzXX0=
-->