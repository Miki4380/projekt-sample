# Tytuł roboczy/nazwa kodowa projektu

**G4meD3v** – porównywarka cen gier z różnych stron gamingowych.

## Architektura

- Monolit – Pozwoli na utrzymanie całej struktury plików w jednym miejscu na lokalnym serwerze.
- SPA (Single Page Application) –  Z pomocą JS będzie odpowiedzialny za to, że podstrony bez odświeżania będą płynnie się przełączać. 
- Rest API – Będzie pobierał dane gier z plików JSON bez baz SQL.

## Stack technologiczny (języki, frameworki, biblioteki)

- js, php, html, css, json, markdown – Podstawowe języki do zaprogramowania mojej strony, a markdown jako plik .md posłuży do opisów gier.
- marked.js – Biblioteka która przerobi pliki .md na opisy gier przy pomocy HTML.
- node.js, vite – Wykorzystam je jako narzędzia szybkiego lokalnego serwera, jeśli będę mieć problemy z ich uruchomieniem to użyję zwykłego xamppa.
- tokeny/klucze API np.: do repo na GitHub – Strona nie użyje prawdziwych API sklepów, Będą one symulowane przez pliki JSON. Jedyny token API jest używany do połączenia VS Code z GitHubem żeby bezpiecznie przesyłać kod projektu.

## Logika biznesowa

- Wyszukiwarka i filtrowanie: Użytkownik wpisuje tytuł gry, a skrypt JS przeszukuje plik JSON i dynamicznie pokazuje wyniki cen i opisów bez odswieżania strony.
- Moduł opisów: Pokazuje informacje o grze i jej wymagania prosto z pliku .md.
- Moduł Porównywarki: Strona wyświetla tabele porównań z innych sklepów cenowo od najniższej do najwyższej.

## Grupa docelowa

- Kto jest odbiorcą projektu? Głównie gracze którzy chcą znaleźć najlepsze promocje na gry które ich interesują.
- Jakie są ich potrzeby i oczekiwania? Ich oczekiwania to m. in. natychmiastowy dostęp do listy sklepów z interesującymi ich ofertami, prosta nawigacja po stronie oraz ciemny motyw który jest komfortowy dla oczu.

## Wymagania techniczne

Strona będzie dostępna na komputer i telefon. Również nie może uruchamiać się z błędami w konsoli F12 popełnionymi przez JS.

### Wymagania prawne

- Prawa autorskie: Skrypty piszę sam z pomocą tutoriali na YT a także innych stron edukujących w językach programowania, napisane skrypty sprawdzam za pomocą sztucznej inteligencji pod kątem błędów i bugów żeby dowiedzieć się jakie błędy muszę poprawić.
- Licencje: Loga oraz podobne materiały będą wykorzystane tylko w celu edukacyjnym.
- RODO (cookies): Strona wyświetli informację o plikach cookies a one zapamiętają jedynie preferencje motywu wizualnego użytkownika.

### Standaryzacja

- WCAG 2.1: Dodam opisy `alt` do wszystkich obrazów, a kolory dobiorę tak, żeby tekst był dobrze widoczny i czytelny na ciemnym motywie.
- SEO: W sekcji `<head>` dodam odpowiednie tagi `title` i `meta description`, żeby strona była zrobiona zgodnie z przyjętymi standardami prawdziwych witryn.

---

# Standardowe wymagania końcowe projektu

- Dokumentacja techniczna kodu w JSDocs, PHPDoc, itp.: Do najważniejszych funkcji w JS i PHP dopiszę krótkie komentarze w kodzie, żeby było wiadomo, za co odpowiadają, jakie dane przyjmują i co zwracają.
- Dokumentacja markdown logiki biznesowej i abstrakcji projektu: Plik `README.md` posłuży właśnie jako główna dokumentacja, w której opiszę wszystkie założenia i zasady działania mojego projektu.
