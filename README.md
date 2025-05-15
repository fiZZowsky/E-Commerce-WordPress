# WordPress vs Symfony – Porównanie

[![WordPress Version](https://img.shields.io/badge/WordPress-5.x-blue.svg)](https://wordpress.org/) [![License: GPL v2](https://img.shields.io/badge/License-GPL%20v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)

---

## Spis treści

1. [Opis teoretyczny WordPress](#opis-teoretyczny-wordpress)  
2. [Podstawowe cechy WordPress](#podstawowe-cechy-wordpress)  
3. [Struktura WordPress](#struktura-wordpress)  
4. [Zastosowania WordPress](#zastosowania-wordpress)  
5. [Zalety i wady WordPress](#zalety-i-wady-wordpress)  
6. [Porównanie najpopularniejszych motywów](#porownanie-najpopularniejszych-motywow)  
7. [Porównanie obszarów: WordPress vs Symfony](#porownanie-obszarow-wordpress-vs-symfony)  
   - [Instalacja i konfiguracja](#instalacja-i-konfiguracja)  
   - [Schemat docker-compose.yml](#schemat-docker-composeyml)  
   - [Czas wdrożenia](#czas-wdrozenia)  

---

## Opis teoretyczny WordPress

WordPress narodził się w 2003 roku jako prosty silnik blogowy, jednak już wkrótce wykrystalizował się w potężny i elastyczny system zarządzania treścią (CMS). Jego filozofia opiera się na zasadzie „demokratyzacji publikacji” – każdy, niezależnie od poziomu zaawansowania technicznego, powinien móc stworzyć i prowadzić własną stronę internetową. Lekki instalator, intuicyjny interfejs oraz przejrzysta organizacja plików sprawiają, że proces uruchomienia witryny jest szybki i nieskomplikowany.

Rdzeń WordPressa opiera się na języku PHP i relacyjnej bazie danych MySQL lub MariaDB. Architektura ta umożliwia dynamiczne generowanie stron oraz łatwe skalowanie od niewielkich blogów po rozbudowane portale korporacyjne. Kluczowym mechanizmem wewnętrznym są tzw. hooki — punkty zaczepienia (actions i filters), które pozwalają wtyczkom i motywom zmieniać lub rozszerzać funkcjonalność systemu bez ingerencji w pliki core. Dzięki temu całość pozostaje elastyczna i odporna na modyfikacje podczas aktualizacji.

Model danych WordPressa oparty jest na pojęciu „postów”, które domyślnie reprezentują zarówno wpisy blogowe, jak i statyczne strony. Możliwość definiowania własnych typów treści (Custom Post Types) oraz taksonomii (Custom Taxonomies) pozwala tworzyć rozbudowane struktury informacji, dopasowane do specyfiki danego projektu. To podejście sprawia, że WordPress doskonale radzi sobie nie tylko z prostymi publikacjami, ale również z katalogami produktów, galeriami czy nawet systemami e-learningowymi.

Interfejs graficzny panelu administracyjnego został zaprojektowany z myślą o czytelności i ergonomii pracy. Dzięki systemowi motywów (Themes) można niemal dowolnie zmieniać wygląd strony, a zaawansowany edytor blokowy Gutenberg umożliwia budowanie rozbudowanych układów treści bez pisania ani jednej linijki kodu. Z kolei architektura wtyczek (Plugins) otwiera niemal nieograniczone możliwości – od prostych formularzy kontaktowych, przez zaawansowane narzędzia SEO, aż po kompletne rozwiązania e-commerce, jak WooCommerce.

W ostatnich latach WordPress rozwinął również własne REST API, co czyni go pełnoprawnym headless CMS-em. Zewnętrzne aplikacje i frameworki (React, Vue, mobilne) mogą korzystać z zasobów WordPressa jako backendu, zachowując pełną kontrolę nad warstwą prezentacji. Dzięki temu deweloperzy otrzymują nowoczesne narzędzie, które łączy niezawodność sprawdzonego silnika z elastycznością nowoczesnych technologii front-endowych.

Podsumowując, teoretyczny fundament WordPressa stanowi połączenie prostoty użytkowania, otwartej architektury oraz szerokiego ekosystemu społeczności. To sprawia, że system jest zarówno doskonałym wyborem dla osób rozpoczynających przygodę z tworzeniem stron, jak i dla zaawansowanych programistów potrzebujących solidnej bazy do realizacji niestandardowych projektów.

---

## Podstawowe cechy WordPress

1. **Open Source**  
   Darmowy, ciągle rozwijany przez społeczność.

2. **Łatwość użycia**  
   Intuicyjny panel administracyjny.

3. **Rozbudowa i personalizacja**  
   Tysiące wtyczek i motywów.

4. **Skalowalność**  
   Od blogów po duże sklepy e-commerce.

5. **SEO**  
   Wbudowane mechanizmy i wtyczki (Yoast, All in One SEO).

6. **Wsparcie społeczności**  
   Fora, grupy, dokumentacja.

7. **Bezpieczeństwo**  
   Regularne aktualizacje i wtyczki zabezpieczające.

---

## Struktura WordPress

- **Baza danych (MySQL/MariaDB)**  
  Przechowuje treści, użytkowników, ustawienia.
- **Pliki motywów**  
  HTML/PHP, CSS, JS definiujące wygląd.
- **Wtyczki**  
  Rozszerzają funkcjonalność.
- **Panel administratora**  
  UI do zarządzania treścią i konfiguracją.

---

## Zastosowania WordPress

- **Blogi**  
- **Strony firmowe**  
- **Sklepy internetowe (WooCommerce)**  
- **Portfolia**  
- **Platformy e-learningowe**  
- **Fora internetowe (bbPress)**  

---

## Zalety i wady WordPress

| Zalety                          | Wady                                    |
|---------------------------------|-----------------------------------------|
| Łatwość w obsłudze              | Ataki, jeśli brak aktualizacji          |
| Elastyczność i personalizacja   | Możliwe spowolnienie przy wielu wtyczkach |
| Ogromna społeczność i zasoby    | Czasem potrzeba wiedzy technicznej      |
| Regularne aktualizacje          |                                         |

---

## Porównanie najpopularniejszych motywów

| Motyw               | Typ licencji | Responsywność | Liczba instalacji | Główne funkcje                         |
|---------------------|--------------|---------------|-------------------|----------------------------------------|
| **Astra**           | Free/Paid    | ✔             | >1 000 000        | Lekki, wtyczki SEO, buildery           |
| **GeneratePress**   | Free/Paid    | ✔             | >500 000          | Szybki, modularny, kompatybilny z Gutenberg |
| **OceanWP (Free)**  | Free/Paid    | ✔             | >700 000          | Demo import, WooCommerce, popup builder|
| **Neve**            | Free/Paid    | ✔             | >200 000          | AMP-ready, header builder              |

---

## Porównanie obszarów: WordPress vs Symfony

| Obszar                              | WordPress                                                    | Symfony                                                      |
|-------------------------------------|--------------------------------------------------------------|--------------------------------------------------------------|
| **Instalacja i konfiguracja**       | Docker+docker-compose, PHP & MariaDB                         | Composer, wymaga PHP 7.4+, skonfigurowanie bundle’ów         |
| **Baza danych**                     | WP_Query, tabela `wp_*`                                      | Doctrine ORM, encje, repository                              |
| **Zarządzanie produktami**          | WooCommerce: proste UI, warianty, kategorie                  | Ręczna implementacja, CRUD, bardziej kodu                    |
| **Zarządzanie użytkownikami**       | Wbudowane role, pluginy rozszerzające                        | Security Bundle, Role Hierarchy, voters                      |
| **Koszyk i zamówienia**             | WooCommerce: automatyczne, API                               | Custom API, kontrolery, więcej kodu                          |
| **Panel administratora**            | Gotowy WP-Admin, liczne wtyczki                              | EasyAdminBundle lub SonataAdmin, konfiguracja YAML/PHP       |
| **Wydajność**                       | Caching pluginy (WP Super Cache, W3 Total Cache)             | HTTP Cache, OPcache, Varnish                                 |
| **Rozszerzalność**                  | Wtyczki, hooki, filtry                                       | Bundles, EventDispatcher, Dependency Injection               |
| **Szablony i wygląd**               | PHP Template, Gutenberg Blocks                               | Twig, komponenty, Assetic                                    |
| **Bezpieczeństwo**                  | Core + pluginy zabezpieczające                               | Security Bundle, własne policy, HTTPS                        |
| **Cena i czas developmentu**        | Szybkie MVP dzięki gotowym rozwiązaniom                      | Dłuższy czas (kilka tygodni), wyższe koszty                  |
| **Testowanie**                      | PHPUnit, pluginy                                             | PHPUnit, Behat, PHPSpec                                      |
| **Społeczność i dokumentacja**      | Ogromna, fora, Codex                                         | Oficjalna docs, SensioLabs, mniejsze community               |

---

### Instalacja i konfiguracja

#### 1) Symfony

#### 2) Wordpress
  a) wymagania wstępne:
  - serwer WWW (np. Apache, Nginx, Docker),
  - baza danych (np. MySQL, MariaDB),
  - (opcjonalnie domena (na początku może być localhost).

> [!NOTE]
> W celu wykonania analizy porównawczej obu frameworków baza danych została stworzona na serwerze online. Dzięki czemu oba projekty zasilane są tymi samymi danymi. Na nasze potrzeby wybrano bazę MariaDB. Wordpress postawiony został na Dockerze przy użyciu pliku docker-compose.yml oraz podstawowych komend dockera.

  b) przygotowanie pliku docker-compose.yml
  ```yaml
version: '3.7'

services:
  db:
    image: mariadb:10
    container_name: wordpress-db
    restart: always
    volumes:
      - db_data:/var/lib/mysql
      - db_backups:/backups
    environment:
      MYSQL_DATABASE: <DB_NAME>
      MYSQL_USER: <DB_USER>
      MYSQL_PASSWORD: <DB_PASSWORD>
      MYSQL_ALLOW_EMPTY_PASSWORD: 'no'
      MYSQL_ROOT_PASSWORD: <DB_ROOT_PASSWORD>

  wordpress:
    image: wordpress:latest
    container_name: wordpress
    restart: always
    depends_on:
      - db
    ports:
      - "8080:80"
    links:
      - db
    volumes:
      - wp_data:/var/www/html
      - wp_backups:/backups
    environment:
      WORDPRESS_DB_HOST: db
      WORDPRESS_DB_NAME: <DB_NAME>
      WORDPRESS_DB_USER: <DB_USER>
      WORDPRESS_DB_PASSWORD: <DB_PASSWORD>

  phpmyadmin:
    image: phpmyadmin/phpmyadmin:4.7
    container_name: wordpress-phpmyadmin
    restart: always
    depends_on:
      - db
    ports:
      - "12000:80"
    links:
      - db:db
    volumes:
      - pma_backups:/backups
    environment:
      PMA_HOST: db
      PMA_USER: <DB_USER>
      PMA_PASSWORD: <DB_PASSWORD>

volumes:
  db_data:
  db_backups:
  wp_data:
  wp_backups:
  pma_backups:
```

  c) utworzenie i uruchomienie kontenerów
  
```
docker-compose up -d
```

  d) konfiguracja
  Po uruchomieniu środowiska, instalacja WordPressa została przeprowadzona przez przeglądarkę:
-	Wejście pod adres: http://localhost:8080
-	Wypełnienie formularza instalacji:
  	- Tytuł witryny — np. "wp-ecommerce"
    - Nazwa użytkownika — administrator WordPressa
    - Hasło — silne hasło do panelu
    - Adres e-mail — do odzyskiwania konta
-	Po instalacji utworzono pierwszego użytkownika i zalogowano się do panelu administracyjnego `/wp-admin`.

  e) czas wdrożenia:
  Na wykonanie wszystkich wymaganych kroków potrzebnych do uruchomienia strony startowej w wordpress potrzebne było około **15 minut**.
