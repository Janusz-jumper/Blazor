W komponencie Weather.razor wykonałem następujące modyfikacje:

Zwiększyłem długość prognozy do 10 dni.

Dodałem zmienną warmDays, która zlicza liczbę dni z temperaturą powyżej 15°C (obliczane w OnInitializedAsync()).

Wyświetliłem wynik w interfejsie jako:
Warm days count: @warmDays.

Dodałem pole tekstowe do filtrowania prognozy po nazwie (Summary) – implementacja za pomocą metody Input(ChangeEventArgs arg) i zdarzenia @oninput.

Zaimplementowałem przycisk Show only warm days, który filtruje dane (WarmDaysFilter()).

Dodałem przycisk Restore all, który przywraca pełną listę (RestoreForecasts()).

Użyłem dyrektywy @rendermode InteractiveServer, aby komponent był interaktywny po stronie serwera.

Aplikacja działa poprawnie z dynamicznym filtrowaniem danych oraz interaktywnym renderowaniem komponentu.
