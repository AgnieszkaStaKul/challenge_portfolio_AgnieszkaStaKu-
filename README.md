# challenge_portfolio_AgnieszkaStaKu

# TASK1

## Subtask 1
$$\textcolor{green}{\text{9 punktów}}$$

## Subtask 2

Jak widać udało się! 😉

## Subtask 3
Hej! Mam na imię Agnieszka. Z wykształcenia jestem socjologiem i plastykiem, z pasji kucharzem. Chyba czas na kolejną specjalizację! 😉 Zdecydowałam się na udział w Dare IT Challenge, ponieważ docelowo chciałabym rozpocząć pracę jako tester. Wierzę (i już to widzę!), że zadania pozwolą mi usystematyzować wiedzę zdobytą do tej pory, umożliwą przećwiczenie jej i za te kilka tygodni będę wiedziała... Czego jeszcze muszę się nauczyć. :smiley: 

Chciałabym, żeby testowanie było dla mnie nie tylko możliwością zawodową, ale i przyjemnością - a żeby tak było, chcę być w tym naprawdę dobra. Liczę, że Challenge będzie właściwym krokiem w tym kierunku. 

*Agnieszka*

## Subtask 4

### Do czego służy aplikacja?

Aplikacja służy do analizowania piłkarzy. Pozwala wprowadzać graczy (ze wszystkimi niezbędnymi danymi), analizować mecze w czasie rzeczywistym, generować raporty. 

### Fukncjonalności aplikacji oraz ich intuicyjność. 

Aplikacja zawiera bazę danych piłkarzy z informacją o klubie w którym grają, na jakiej pozycji, rozegranych meczach, ich recenzji (opisanej numerycznie) oraz raportach dotyczących gracza. Tabelę z danymi dotyczącymi graczy można przeglądać, filtrować, edytować z jej poziomu graczy, pobierać oraz drukować. Zakładka "gracze" jest intuicyjna. Warto by było wprowadzić możliwość dodania nowego gracza z jej poziomu. Problemem jest fakt, że edycja gracza uruchamia się po kliknięciu w dowolny obszar w wierszu danego gracza - lepiej, by po prawej znajdował się przycisk edycji, lub by kursor zmieniał swój wygląd na taki, który sugeruje możliwość przejścia do okienka edycji przy nakierowanie go na imię lub nazwisko gracza. 

Aplikacja pozwala tworzyć raporty podczas trwania meczu poprzez dodawanie określonych akcji, z których następnie można wygenerować końcowy raport, który zawiera uszeregowane i podsumowane liczbowo wprowadzone wcześniej akcje oraz element opisowy, który scout wprowadza samodzielnie. Należy w zakładce z raportem stworzyć możliwość pobrania go oraz wydrukowania z poziomu aplikacji.

Strona główna jest mało intuicyjna. Panel po lewej stronie umożliwia jedynie przejście do strony głównej, podgląd bazy z graczami, zmianę języka i wylogowanie się. Warto, by zawarto w nim również pozostałe funkcjonalności - dodawanie meczy, podgląd i edycję raportów - aktualnie jest to możliwe jedynie z poziomu edycji gracza. Pomocną byłaby możliwość przejścia od razu do takiej zakładki (mecz/raport) a potem dopasowanie go do określonego gracza. 

Na stronie głównej w zakładkach zawierających informację liczbową o liczbie graczy, ilości meczów, ilości raportów i ilości akcji ciężko zorientować się o co chodzi właśnie w "ilości akcji". 

W tabeli  "ostatnia aktywność" na stronie głównej powinien też znajdować się "ostatnio utworzony raport".

W edycji gracza nie wiadomo czego dotyczą pozycje “Łączy na Piłka” oraz “90 minut” -  warto dodać informację (jak w przypadku Facebooka) “profil” - wtedy nawet osoba nie będąca w temacie będzie wiedziała czego dotyczy pozycja.

### Ocena interfejsu aplikacji.

Aplikacja jest wizualnie bardzo prosta. Ułatwia to korzystanie z niej, jednak wygląda nieco przestarzale. Poszczególne funkcje są rozstrzelone po stronie głównej, co wprowadza chaos. 

### Ocena intuicyjności aplikacji. 

Dodawanie niego gracza jest intuicyjne ze względu na zawarcie tej funkcjonalności w linkach pomocniczych na głównej stronie. Warto by dodać jednak tą możliwość także w bocznym panelu (jak również tworzenie meczów i raportów). 

Ciężko dotrzeć do menu dodawania meczów i raportów ze względu na konieczność przeklinania wpierw przez listę graczy, wejście w edycję gracza (co również jest nieintuicyjne) i dopiero wtedy w bocznym panelu pojawia nam się możliwość ich dodania. 

W tabeli “gracze” przydałaby się ikonka do edycji gracza - obecnie do edycji przechodzi się poprzez kliknięcie w dowolnym miejscu wiersza dotyczącego danego zawodnika.

### Błędy

#### Logowanie
Warto dać możliwość podglądu hasła.

#### Strona główna

W panelu “Aktywność” na stronie głównej literówka - “zaaktualizowany” powinno być “zaktualizowany”

Przy niezapisanym meczu brak możliwości powrotu do raportu przez link “wróć do raportu”

![niezapisany mecz](https://user-images.githubusercontent.com/120724034/212757103-afabf1f7-1f59-4106-adc2-9d018986a368.png)

#### Lista graczy

Powielający się gracze - konieczność kontroli, czy dany gracz nie został już wprowadzony.

Nie pokazuje się nad tabelą jakiego filtra dotyczy tekst - w pozycji “imię”, “nazwisko”, “pozycja”, “klub”. Działa dla “age” i “rate”. 

#### Edycja gracza

*Pola “imię” i “nazwisko”* - nie powinno być możliwości wprowadzania liczb i znaków specjalnych (oprócz myślnika), jedynie litery. Powinna być także ograniczona liczba znaków możliwych do wprowadzenia. 

*Pole "wiek"* - możliwość wyboru zbyt szerokiego zakresu dat, przez co pojawiają się kilkusetletni gracze, lub zbyt młodzi, lub jeszcze nie narodzeni. Powinien być ograniczony zakres do wyboru.

*Pole “e-mail”* - po wpisaniu tekstu bez znaku “@” nie ma możliwości zapisania/zaktualizowania gracza, jednak program nie podaje informacji dlaczego. Powinna być informacja w którym okienku jest wprowadzony element uniemożliwiający zapisanie gracza. 

*Pole “telefon”* - nie powinno być możliwości wprowadzania liter i znaków specjalnych, jedynie liczby. Powinna być także ograniczona liczba znaków możliwych do wprowadzenia. 

*Pole “waga”* - Nie powinno być możliwości wprowadzania wartości ujemnych oraz po przecinku. Powinna być także ograniczona liczba znaków możliwych do wprowadzenia. 

*Pole “wzrost”* - po wpisaniu błędnej wartości i klinięciu na inny obszar wartość ta jest akceptowana przez program. Po wpisaniu błędnej wartości i kliknięciu klawisza ‘enter” wyświetla się komunikat o błędzie. Należy wyświetlać komunikat o niepoprawnej wartości w obu przypadkach. Komunikat uwzględnia wartości ujemne jako prawidłowe. 

*Pola “klub”, “główna pozycja”* - powinna być ograniczona liczba znaków możliwych do wprowadzenia. 

*Pola “języki”, “Łączy nas piłka”, “90 minut”* - nie powinno być możliwości wprowadzania liczb i znaków specjalnych, jedynie litery. Powinna być także ograniczona liczba znaków możliwych do wprowadzenia. 

*Pola “profil facebook” i “link do YouTube”* - powinien być zapisany jako odnośnik url, a nie wartość tekstowa, żeby po kliknięciu móc od razu przejść na stronę.

#### Mecze

“Mecze” → “Rozpocznij mecz” - możliwość dodania więcej niż dwóch połów meczu.

#### Dodaj mecz

*Pole "data"* - możliwość podania nierealnych dat (04-04-0004). Umożliwienie wpisywania dat z określonego zakresu lub jedynie ich wyboru z kalendarza.

*Pola “zdobyte gole” i “stracone gole”* - ograniczenie liczby znaków możliwych do wprowadzenia. 

*Pole “kolor koszulki”* - nie powinno być możliwości wprowadzania liczb i znaków specjalnych, jedynie litery. Powinna być także ograniczona liczba znaków możliwych do wprowadzenia. 

*Pole “liga”* - najlepiej zrobić rozwijaną listę z możliwymi opcjami, żeby wszystko było ujednolicone. 

*Pole “numer”, “czas gry”* - wprowadzenie braku możliwości podania liczb ujemnych oraz po przecinku, ograniczenie zakresu liczb. 

#### Raporty

Po kliknięciu w przycisk “dodaj raport” przekierowuje nas na stronę z listą meczów. 

#### Dev tools

Strona główna na urządzeniach mobilnych na niski wskaźnik Performance, związany z długim czasem ładowania.

![lighhouse mobi strona główna](https://user-images.githubusercontent.com/120724034/212757861-9788dbaf-acdd-449c-9743-34737a45658f.png)

Podobnie w menu edycji gracza (na urządzenia mobilne) - niski Performance, dodatkowo stosunkowo niskie SEO. 

![lighthouse mobi edycja graczy](https://user-images.githubusercontent.com/120724034/212758154-1807581b-b0b1-41b2-9817-52fe9917ba9f.png)

Na urządzeniach mobilnych edycja gracza/meczu wygląda nieestetycznie. Pola do wprowadzania danych są za szerokie - lepiej, by dostosowywały się do rozdzielczości ekranu. 

https://user-images.githubusercontent.com/120724034/212758025-9e6fc8fa-962c-4da1-8a62-2d42cb498e44.mp4

Bardzo długi czas ładowania pliku png (1,3 min) - tu sytuacja miała miejsce o 20:20, dzień przed oddaniem zadania 😉 Możliwe, że sytuacja taka występuje przy obciążeniu serwera, ponieważ przy wcześniejszym ładowaniu tej strony (innego dnia, w godzinach porannych), ładowało się błyskawicznie.

![lighhouse deskop mecz ](https://user-images.githubusercontent.com/120724034/212757979-111a95ef-a013-4d9f-aa61-e8a50245b3ef.png)

Powtórzone parokrotnie - najpierw ładowało się wolno za każdym razem, potem po kilku minutach już szybko. Niezależnie od prędkości Internetu (testowane na Fast 3G i Slow 3G)

## Subtask 5

Projekt w Jirze założony - Pati zaproszona do projektu. 😉 

# TASK 2

## Subtask 1

[Pisanie przypadków testowych na podstawie User Story.](https://docs.google.com/spreadsheets/d/1tlJEn8MnRkRne9H9ARLT-GNZAJ_AwUfgYL44pbW1FPQ/edit#gid=0)

## Subtask 2

[Pisanie przypadków testowych na podstawie “własnych doświadczeń".](https://docs.google.com/spreadsheets/d/1ttNOXPRfkWQ0IL2bhyw6ofATzUdYoe8cBnOmVYlW0h0/edit#gid=0)

## Subtask 3

Test case'y pisane są po to, by dokładnie przetestować każdą możliwość - bez powielania, ale i bez pomijania elementów. Dodatkowo pozwalają na wielokrotne uruchamianie dokładnie tych samych testów - nawet jesli robią je rózne osoby, dzięki przypadkom testowym testy będą przebiegały identycznie. Dzięki nim także możliwe są retesty i testy regresji.

# TASK3

## Subtask 1 + 2

[Formatka ze zgłoszonymi błędami](https://docs.google.com/document/d/187JR2mQ-X5gIx5h9KsecllMvZQmI9IPkcVA9c2eY-AQ/edit#heading=h.kqm4mnf15nwb)

[Test Case z informacją o przebiegu testów](https://docs.google.com/spreadsheets/d/1-TkCSq9Zq19VPsIOzRatB1IXGq5xu_zyQVxTFeLAueY/edit#gid=0)

## Subtask 3

[Raport](https://docs.google.com/document/d/1yk8ftU-06ln9GRaOMP9iY5D2uOQQqAINR4bqrb2Awsk/edit#)

# TASK4

## Subtask 2

[Testowanie eksploracyjne](https://docs.google.com/document/d/1T9fFP6ys6V-78mODzQ-UNHgmL_IMan36ViGs6B7m0u4/edit?usp=sharing)

## Subtask 3

### Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?

Aplikacja służy mobilnej obsłusze strony Olx.pl z ogłoszeniami. Dzięki niej możemy utworzyć, edytować i usunąć profil użytkownika, wyszukiwać ogłoszenia sprzedaży, o pracę, wystawiać rzeczy na sprzedaż. Obsługuje dokłądnie te same elementy, co strona Internetowa. 

### Kto ma być użytkownikiem końcowym aplikacji?

Użytkownik portolu Olx.pl - posiadający profil na portalu, ale także taki, który dopiero profil chce założyć. Osoba/firma chcąca zamieścić na portalu (/w aplikacji) ogłoszenie kupna, sprzedaży, o pracę. 

### Czy według Ciebie aplikacja jest user friendly? 

Zdecydowanie tak. Aplikacja jest przejrzysta, poruszanie się po niej jest intuicyjne. Łatwo dostać się do poszczególnych elementów aplikacji - edycji profilu, ogłoszeń. Wypełnianie formatek jest przygotowane na błędy uzytkownika - pojawiają się komunikaty walidacyjne. Dodatkowo aplikacja jest estetyczna, a co jest dodatkowym atutem - jest kopią strony internetowej (w domyśle znanej użytkownikowi), dzięki czemu osobie znajacej Olx jest łatwo się po niej poruszać.

### Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? 

Brak uwag.

### Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?

- w testach aplikacji internetowej możemy pozyskać dodatkowe dane za pomocą dev tools;
- aplikacje natywne korzystają z dostępu do funkcjonalności telefonu (rozpoznawanie twarzy, dostęp do plików, powiadomienia push, mikrofon etc.), co również możemy testować;
- testy aplikacji internetowej wydają się być wygodniejsze - duży ekran, myszka komputerowa, kilka otwartych okien, kontra małe urządzenie odługiwane w łaściwie jednym palcem;
- testy aplikacji natywnych zmuszają do korzystania z wielu sprzętów lub emulatorów; aplikacje internetowe obsługują mniejszą różnorodność na przykład rozdzielczości.


# Task 5

## Subtask 1

- SELECT * FROM
- ORDER BY ... DESC
- ORDER BY ... ASC
- SELECT ... FROM ... WHERE ...
- GETDATE
- SELECT UPPER
- DATEDIFF
- SELECT ... AS ... 
- SELECT COUNT (*) AS ... FROM ...
- SELECT SUM(...) AS ... FROM ...
- SELECT MIN(...) AS ... FROM ...
- GROUP BY
- JOIN

## Subtask 2 

Serwer postawiony! 


------Do uzupełnienia------

# Task 6

# Subtask 1

11. Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd 🙈

UPDATE customers SET surname = 'Miler'
WHERE name = 'Ania' AND surname = 'Muler';

![Ad11](https://user-images.githubusercontent.com/120724034/219976474-401891dc-a98a-4c6e-a8e6-a31c8e18d2f4.png)

12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.

SELECT name, email FROM customers AS c 
JOIN sale AS s ON c.customer_id = s.customer_id
WHERE s.movie_id = 4;

![Ad12](https://user-images.githubusercontent.com/120724034/219976506-f414d771-4a5b-41a1-a240-1979a7c2b126.png)

13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com

UPDATE customers SET email = 'pati@mail.com'
WHERE name = 'Patrycja';

![Ad13](https://user-images.githubusercontent.com/120724034/219976542-0021f23f-31c5-4187-843f-97fa83c8ea4d.png)

14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).

SELECT DISTINCT name, surname FROM customers AS c
INNER JOIN sale AS s ON c.customer_id = s.customer_id;

![Ad14](https://user-images.githubusercontent.com/120724034/219976561-a3b7d69e-ccb2-4fee-9cc8-54d88268d447.png)

15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag

ALTER TABLE customers
ADD pseudonym varchar(20) COLLATE utf8_polish_ci DEFAULT NULL;

![Ad15](https://user-images.githubusercontent.com/120724034/219976574-5170203a-d05f-4aef-9ea2-c98d64133d48.png)

16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.

SELECT DISTINCT title FROM movies AS m
JOIN sale AS s ON m.movie_id = s.movie_id;

![Ad16](https://user-images.githubusercontent.com/120724034/219976582-cd6972af-dd24-4966-a85f-739c9517acbd.png)

17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)

SELECT name, surname FROM actors
UNION
SELECT name, surname FROM customers;

![Ad17](https://user-images.githubusercontent.com/120724034/219976604-9deb7a73-8f1d-4b7d-bfbf-79c72ccef199.png)

18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).

UPDATE movies SET price = price + 2.5
WHERE year_of_production > 2000;

![Ad18](https://user-images.githubusercontent.com/120724034/219976634-162204e7-6d6e-47e2-a491-b472e9a711a2.png)

19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał

SELECT DISTINCT a.name, a.surname, m.title FROM actors AS a
JOIN cast AS c ON a.actor_id = c.actor_id
JOIN movies AS m ON m.movie_id = c.movie_id 
WHERE a.actor_id = 4;

![Ad19](https://user-images.githubusercontent.com/120724034/219976647-bf4d51be-60da-4f8f-bc13-8e8efc8dd90b.png)

20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa

INSERT INTO customers (customer_id, name, surname, email, pseudonym)
VALUES (7, 'Honia', 'Stuczka-Kucharska', 'honia@mail.com', 'Hoa');

![Ad20](https://user-images.githubusercontent.com/120724034/219976665-f9bbaa21-de39-472e-9d04-8c2dd240f9a3.png)


# Subtask 2

$$\textcolor{green}{\text{11 punktów}}$$

# Subtask 3

[Portfolio](https://github.com/AgnieszkaStaKul/Portfolio/blob/main/README.md)

