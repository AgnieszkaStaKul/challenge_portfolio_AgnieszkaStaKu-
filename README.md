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
