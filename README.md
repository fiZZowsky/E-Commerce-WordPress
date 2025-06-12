# WordPress vs Symfony – Porównanie

[![WordPress Version](https://img.shields.io/badge/WordPress-5.x-red.svg)](https://wordpress.org/) [![License: GPL v2](https://img.shields.io/badge/License-GPL%20v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
[![Symfony Version](https://img.shields.io/badge/Symfony-6.4-orange.svg)](https://symfony.com/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


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

| Motyw             | Cena roczna (PLN) | FSE   | Customizer | Demo import     | Typografia               | WooCommerce-ready | Header/Footer Builder | Mega Menu | Global Styles | RTL Support | Performance       |
|-------------------|-------------------|-------|------------|-----------------|--------------------------|-------------------|-----------------------|-----------|---------------|-------------|-------------------|
| **Astra**         | ~250 PLN          | ❌    | ✅         | >100 szablonów  | Rozbudowane ustawienia   | ✅                | ✅                    | ✅        | ✅            | ✅          | Bardzo lekki      |
| **GeneratePress** | ~250 PLN          | ❌    | ✅         | ~60 szablonów   | Elastyczne, podstawowe   | ✅                | ❌ (hooki)            | ❌        | ❌            | ✅          | Ekstremalnie lekki|
| **OceanWP**       | ~165 PLN          | ❌    | ✅         | >50 szablonów   | Dobre                    | ✅                | ✅                    | ✅        | Ograniczone   | ✅          | Średnio lekki     |
| **Blocksy**       | ~210 PLN          | ✅    | ✅         | >40 szablonów   | Pełna kontrola           | ✅ (Pro)          | ✅                    | ✅        | ✅            | ✅          | Lekki             |

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
| **Dane porównawcze i metryka**      | Caching pluginy (WP Super Cache, W3 Total Cache)             | Developer mode                                               |
| **Szablony i wygląd**               | PHP Template, Gutenberg Blocks                               | Twig, komponenty, Assetic                                    |
| **Społeczność i dokumentacja**      | Ogromna, fora, Codex                                         | Oficjalna docs, SensioLabs, mniejsze community               |

---

### Instalacja i konfiguracja

#### 1) Symfony
a) **Wymagania wstępne**  
- PHP ≥ 7.4 (zalecane 8.0+).  
- Composer (menedżer zależności dla PHP).  
- Serwer WWW (najczęściej Nginx lub Apache, choć w trakcie developmentu można korzystać z wbudowanego serwera Symfony).  
- Opcjonalnie: Docker (w celu odizolowania środowiska) lub Symfony CLI (ułatwia uruchamianie serwera deweloperskiego i inne komendy).  
- Baza danych (np. MySQL/MariaDB, PostgreSQL itp.).
b) **Tworzenie nowego projektu**
1. **Bez Dockera (lokalnie)**  
   ```bash
   # Jeżeli użytkownik posiada Symfony CLI:
   symfony new nazwa_projektu --full
   cd nazwa_projektu

   # Lub przy pomocy Composera:
   composer create-project symfony/skeleton nazwa_projektu
   cd nazwa_projektu
   composer require webapp         # instaluje podstawowy pakiet „full stack” (Twig, Form, Doctrine itp.)
   ```
c) **Konfiguracja środowiska** 
- Symfony korzysta z pliku .env (lub .env.local na lokalne nadpisania), w którym definiujemy zmienne, np. połączenie z bazą
   ```bash
   # APP_ENV=dev
   APP_SECRET=0123456789abcdef0123456789abcdef
   DATABASE_URL="mysql://symfony_user:symfony_pass@db:3306/symfony_db?serverVersion=10.5"
   ```
d) **Uruchomienie środowiska deweloperskiego** 
- Jeżeli użytkownik posiada Symfony CLI
   ```bash
   symfony server:start
   ```
-Domyślnie aplikacja będzie dostępna pod adresem https://127.0.0.1:8000 (lub http://127.0.0.1:8000)

e) **Czas wdrożenia**
- Przy założeniu, że mamy zainstalowane PHP, Composer i ewentualnie Docker:

   - Klon repozytorium + instalacja zależności (composer install): 5–10 minut.

   - Konfiguracja zmiennych w .env.local: 2–3 minuty.

   - Pierwsze uruchomienie serwera deweloperskiego i weryfikacja działania: 2–3 minuty.

- W sumie od zera do działającej aplikacji Symfony (bez zaawansowanego własnego kodu) potrzeba około 10–15 minut.


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
  wordpress:
    image: wordpress:latest
    container_name: wp
    restart: always
    ports:
      - "8080:80"
    volumes:
      - wp_data:/var/www/html
    environment:
      WORDPRESS_DB_HOST: <DB_HOST>
      WORDPRESS_DB_NAME: <DB_NAME>
      WORDPRESS_DB_USER: <DB_USER>
      WORDPRESS_DB_PASSWORD: <DB_PASSWORD>

  phpmyadmin:
    image: phpmyadmin/phpmyadmin:4.7
    container_name: wp-phpmyadmin
    restart: always
    ports:
      - "12000:80"
    environment:
      PMA_HOST: <DB_PMA_HOST>
      PMA_USER: <DB_PMA_USER>
      PMA_PASSWORD: <DB_PMA_PASSWORD>

volumes:
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

---
## Podłączenie i komunikacja z bazą danych
#### 1) Symfony
Symfony korzysta z Doctrine ORM (Object-Relational Mapper) do mapowania encji PHP na tabele w bazie danych. Poniżej kluczowe kroki:
a) **Konfiguracja w ```.env``` lub ```.env.local```**
   W zmiennej DATABASE_URL definiujemy parametry połączenia, np.:
   
   ```bash
   DATABASE_URL="mysql://symfony_user:symfony_pass@127.0.0.1:3306/symfony_db?serverVersion=10.5"
   ```

   - symfony_user i symfony_pass to użytkownik i hasło w bazie.

   - 127.0.0.1:3306 to adres i port bazy (w Dockerze adres usługi db dla kontenerów).

   - symfony_db to nazwa bazy.

   - serverVersion=10.5 (dla MariaDB 10.5, pomaga Doctrine generować optymalny SQL).

2) **Tworzenie bazy danych**
   Po skonfigurowaniu ```DATABASE_URL``` można utworzyć bazę za pomocą komendy w terminalu:
   
   ```bash
   php bin/console doctrine:database:create
   ```
- Jeżeli baza już istnieje, zostanie zwrócony komunikat, że nie można jej stworzyć, a w logach – że już istnieje.

c) **Tworzenie encji (Model)**
- Korzystając z narzędzia MakerBundle, można wygenerować encję tak jak poniżej:

```bash
php bin/console make:entity

# Przykład kroków w konsoli:
# Class name of the entity to create or update (e.g. BraveChef):
> Product

# Now enter the fields you want to add to the Product entity (press <return> to stop adding fields):
# New property name (press <return> to stop adding fields):
> name
# Field type (enter ? to see all types) [string]:
>
# Field length [255]:
>
# Can this field be null in the database (nullable) (yes/no) [no]:
>

# Kolejne pole:
> price
# Field type (enter ? to see all types) [string]:
> float
# Czy pole może być null (nullable) (yes/no) [no]:
> no
# Now finished:
> 
```

c) **Migracje bazodanowe**
Po utworzeniu modeli można wykonać migrację za pomocą poniższych komend:

```bash
php bin/console make:migration
php bin/console doctrine:migrations:migrate
```
- Wtedy tabela product (oraz inne wymagane) zostaną utworzone w bazie.

e) **Dostęp do danych w kodzie**
- W Symfony każda encja (Product, User itd.) ma odpowiadający jej ```Repository``` (np. ProductRepository), który dziedziczy po ```ServiceEntityRepository```.
- Typowy kod do pobrania rekordów:
  ```php
  // src/Controller/ProductController.php
   namespace App\Controller;

   use App\Repository\ProductRepository;
   use Symfony\Bundle\FrameworkBundle\Controller\AbstractController;
   use Symfony\Component\HttpFoundation\Response;
   use Symfony\Component\Routing\Annotation\Route;

   class ProductController extends AbstractController
   {
       #[Route('/products', name: 'product_list')]
       public function list(ProductRepository $productRepo): Response
       {
           $products = $productRepo->findAll();
           return $this->render('product/list.html.twig', [
               'products' => $products,
           ]);
       }
   }
  ```
- Można też pisać zapytania DQL lub korzystać z QueryBuilder:
  ```bash
  $qb = $productRepo->createQueryBuilder('p')
                  ->where('p.price > :minPrice')
                  ->setParameter('minPrice', 100)
                  ->orderBy('p.name', 'ASC')
  ;
   $query = $qb->getQuery();
   $results = $query->getResult();
  ```

#### 2) Wordpress
Podłączenie do bazy danych w projekcie Wordpress można zrealizować na kilka sposobów.

- Pierwszy sposób polega na utworzeniu projektu wordpressa i modyfikacji wygenerowanego pliku `wp-config.php`. 

> [!NOTE]
> Plik wp-config.php to pierwszy załadowany przez WordPressa plik konfiguracyjny, który definiuje wszystkie kluczowe ustawienia witryny. Zawiera dane dostępu do bazy danych (nazwa, użytkownik, hasło, host) oraz prefiks tabel, dzięki czemu WordPress wie, gdzie i jak przechowywać swoje tabele. W tym samym miejscu umieszczone są tzw. klucze tajne (authentication keys i salts), które zabezpieczają pliki cookie i sesje użytkowników, a także opcje debugowania (WP_DEBUG i WP_DEBUG_LOG), pozwalające na rejestrowanie błędów w czasie tworzenia i testowania witryny. Dzięki centralizacji tych ustawień w jednym pliku możliwe jest szybkie uruchomienie, modyfikacja i zabezpieczenie środowiska WordPressa.
   
   W pliku tym dane podłączenia do bazy można ustawić na dwa sposoby:
   - poprzez zdefiniowanie w kodzie stałych takich jak `DB_NAME`, `DB_USER`, `DB_PASSWORD`, `DB_HOST`
   - pobieranie zmiennych środowiskowych z `$_ENV` lub `getenv()`
   
   ```php
   define('DB_NAME',     'nazwa_bazy');
   define('DB_USER',     'użytkownik');
   define('DB_PASSWORD', 'hasło');
   define('DB_HOST',     'localhost:3306');
   ```

- Drugi sposób polaga na utworzeniu połączenia z bazą danych poprzez odpowiednią konfigurację w pliku `docker-compose.yml` (zakładając że projekt wordpressa tworzony jest na Dockerze). Działa to na bardzo podobnej zasadzie co ustawianie zmiennych środowiskowych. Do kodu tworzenia kontenera należy dopisać poniższy fragment kodu:

   ```yml
   ...
   wordpress:
   ...
   environment:
     WORDPRESS_DB_HOST: db.example.com:3306
     WORDPRESS_DB_NAME: mydb
     WORDPRESS_DB_USER: user
     WORDPRESS_DB_PASSWORD: pass
   ...
   phpmyadmin:
   ...
   environment:
      PMA_HOST: <DB_PMA_HOST>
      PMA_USER: <DB_PMA_USER>
      PMA_PASSWORD: <DB_PMA_PASSWORD>
   ```

> [!NOTE]
> Zdefiniowanie w pliku `docker-compose.yml` zmiennych `PMA_HOST`, `PMA_USER` i `PMA_PASSWORD`pozwala by kontener phpMyAdmin automatycznie nawiązywał połączenie z bazą danych MariaDB, bez konieczności ręcznego logowania się w interfejsie po starcie. Tak przygotowana usługa dostarcza w przeglądarce całe środowisko do zarządzania bazą danych – od przeglądania i edycji rekordów, przez wykonywanie zapytań SQL, aż po import i eksport danych, optymalizację tabel czy zarządzanie uprawnieniami użytkowników.

- Trzecim sposobem na podłączenie do bazy danych jest użycie wtyczki do zewnętrznych źródeł danych. Istnieją wtyczki-most, które pozwalają łączyć się z innymi systemami (np. LDAP, zewnętrzne API, inne CMS'y), mapując tabele lub uwierzytelnianianie na wordpress.

> [!TIP]
> W przypadku podłączenia do bazy poprzez konfigurację z pliku `docket-compose.yml` poprawność połączenia można zweryfikwać poprzez zastosowanie kilku prostych komend w kosnoli.
```
docker exec -it wp bash
php -r "echo 'Host: '.getenv('WORDPRESS_DB_HOST').PHP_EOL;"
php -r "echo 'User: '.getenv('WORDPRESS_DB_USER').PHP_EOL;"
php -r "echo 'Pass: '.getenv('WORDPRESS_DB_PASSWORD').PHP_EOL;"
exit
```
Wyświetlenie poprawnych danych będzie oznaczać prawidłowe podłączenie do bazy.

---
## Zarządzanie produktami
#### 1) Symfony
- W Symfony „zarządzanie produktami” to w praktyce ręczna implementacja CRUD (Create, Read, Update, Delete) w oparciu o encję Product, formularze, kontrolery oraz widoki. Poniżej skrócony przegląd procesu:
  
a) **Generowanie kontrolera i CRUD-a**
- Przy użyciu MakerBundle można szybko wygenerować CRUD:

  ```bash
  php bin/console make:crud Product
  ```

- To utworzy ProductController, szablony Twig (templates/product/*) oraz formularz ProductType.
   - Kod wygenerowanego kontrolera zazwyczaj zawiera akcje:
     - ```index()``` (lista produktów),
     - ```new()``` (dodawanie produktu),
     - ```show()``` (podgląd produktu),
     - ```edit()``` (edycja produktu),
     - ```delete()``` (usunięcie produktu)
  
   - Plik ```src/Form/ProductType.php``` definiuje formularz oparty na polach encji. Przykład:


   ```php
   namespace App\Form;

   use App\Entity\Product;
   use Symfony\Component\Form\AbstractType;
   use Symfony\Component\Form\Extension\Core\Type\MoneyType;
   use Symfony\Component\Form\Extension\Core\Type\TextType;
   use Symfony\Component\Form\FormBuilderInterface;
   use Symfony\Component\OptionsResolver\OptionsResolver;

   class ProductType extends AbstractType
   {
       public function buildForm(FormBuilderInterface $builder, array $options): void
       {
           $builder
               ->add('name', TextType::class, [
                   'label' => 'Nazwa produktu',
               ])
               ->add('price', MoneyType::class, [
                   'label' => 'Cena',
                   'currency' => 'PLN',
               ])
               ->add('description', TextType::class, [
                   'label' => 'Opis',
                   'required' => false,
               ])
           ;
       }

       public function configureOptions(OptionsResolver $resolver): void
       {
           $resolver->setDefaults([
               'data_class' => Product::class,
           ]);
       }
   }
   ```
   - Widoki (Twig)
     - Wygenerowane szablony templates/product/index.html.twig, new.html.twig, edit.html.twig, show.html.twig umożliwiają wyświetlenie formularzy i listy produktów.
       - Przykład fragmentu z index.html.twig:
        ```twig
        {% extends 'base.html.twig' %}
        
        {% block title %}Lista produktów{% endblock %}
        
        {% block body %}
            <h1>Produkty</h1>
            <a href="{{ path('product_new') }}">Dodaj nowy produkt</a>
        
            <table>
                <thead>
                    <tr>
                        <th>Nazwa</th>
                        <th>Cena</th>
                        <th>Akcje</th>
                    </tr>
                </thead>
                <tbody>
                {% for product in products %}
                    <tr>
                        <td>{{ product.name }}</td>
                        <td>{{ product.price | number_format(2, ',', ' ') }} zł</td>
                        <td>
                            <a href="{{ path('product_show', {'id': product.id}) }}">Pokaż</a>
                            <a href="{{ path('product_edit', {'id': product.id}) }}">Edytuj</a>
                            <form method="post" action="{{ path('product_delete', {'id': product.id}) }}" onsubmit="return confirm('Na pewno?');">
                                <input type="hidden" name="_token" value="{{ csrf_token('delete' ~ product.id) }}">
                                <button type="submit">Usuń</button>
                            </form>
                        </td>
                    </tr>
                {% else %}
                    <tr>
                        <td colspan="3">Brak produktów</td>
                    </tr>
                {% endfor %}
                </tbody>
            </table>
        {% endblock %}
        ```
b) **Uwagi**

- W przeciwieństwie do gotowego interfejsu WooCommerce w WordPressie, w Symfony wszystko implementuje się od podstaw lub korzysta z gotowych pakietów (np. Sylius, Symfony UX Commerce lub innych bibliotek e-commerce).

- Dzięki wygenerowanemu CRUD i formularzom, podstawowe zarządzanie produktami można postawić w ciągu kilkunastu minut, ale dalsze dostosowanie do potrzeb biznesowych (warianty produktów, promocje, relacje itp.) wymaga więcej pracy programistycznej.

#### 2) Wordpress
Zarządzanie produktami w sklepie zostało oparte na wtyczce `WooCommerce`, która automatyzuje cały proces — od dodawania i edycji asortymentu, przez kontrolę stanów magazynowych, aż po obsługę zamówień. 
Po pobraniu wtyczki i jej włączeniu na pasku bocznym pojawiła się zakładka `Produkty`.

![Zakładki panelu admina po dodaniu WooCommerce](doc-resources/Zakladki-Produkty.png)

Po wejściu w zakładkę wyświetlają się grid zawierający dodane produkty i przyciski pozwalające na wykonanie na nich działań.

![Zawartość zakładki produkty](doc-resources/Produkty.png)

Utworzenie produktu jest dokonywane na stronie wyświetlonej po kliknięciu przycisku `Dodaj produkt`. 
Po jej otwarciu wyświetla się pełno opcji umożliwiających tworzenie zarówno prostych jak i rozbudowanych produktów posiadających różne warianty.
Dla każdego produktu ustawiona zostaje nazwa, opis i zdjęcie produktu. Można dodaźć również całą galerię zdjęć dla pokazania jego szczegółów.

![Dodawanie produktu - dane podstawowe](doc-resources/Dodaj-Produkt-cz1.png)

Druga część to dane produktu. Tu wybiera się typ produktu:
- produkt prosty
- produkt grupowy
- produkt zewnętrzny/afiliacyjny
- produkt z wariantami.

Na jego podstawie wyświetlane są odpowiednie opcje konfiguracyjne. Najczęstszym wyborem jest tu produkt z wariantami. 

![Dodawanie produktu - dane produktu - z wariantami](doc-resources/Dodaj-Produkt-cz2.png)

Posiada on opcje do tworzenia różnych wersji tego samego produktu poprzez dodawanie atrybutów. Atrybuty te są używane potem w kolejnej zakładce `Warianty`. Służą one do wygenerowania wszystkich możliwych kombinacji produktu bądź takich jakie zażyczy sobie użytkownik. Konfiguruje się tu również takie opcje jak wysyłka czy powiązane produkty.

![Dodawanie produktu - dane produktu - tworzenie wariantów](doc-resources/Dodaj-Produkt-cz4.png)

Prosty produkt ma zakładkę `Ogólne` pozwalającą na ustawienie ceny oraz opcjonalnie ceny promocyjnej. 

![Dodawanie produktu - dane produktu - prosty](doc-resources/Dodaj-Produkt-cz3.png)

> [!NOTE]
> W przypadku produktów z wariantami ceny również się ustawia, ale po wygenerowaniu wariantów. Można ustawić dla wszystkich tą samą ceną, bądź różne dla wszystkich.

Opisane możliwości to jedynie część z nich jakie umożliwia wtyczka `WooCommerce`.
Po wypełnieniu wszystkich opcji jakie ma spełniać produkt i opublikowaniu go zostaje on dodany do grida w zakładce `Produkty`. 
Opublikowane produkty są już wyświetlane na stronie sklepu. Dzieje się to automatycznie dzięki wtyczce `WooCommerce`, która dostarcza oprócz samego zarządzania produktami inne funkcjonalności związane z zarządzaniem oraz tworzeniem sklepu.

---
## Zarządzanie użytkownikami
#### 1) Symfony
W Symfony najczęściej korzysta się z **Security Bundle** wraz z narzędziem **MakerBundle** do wygenerowania encji użytkownika oraz mechanizmów uwierzytelniania. Kluczowe elementy:
a) **Generowanie encji User**
    ```bash
        php bin/console make:user
    
        # Przykładowy dialog w konsoli:
        # Class name of the User to create (e.g. BraveChef):
        > User
        # Do you want to store user data in the database (via Doctrine)? (yes/no) [yes]
        > 
        # Enter a property name that will be the unique "display" name for the user (e.g. email, username, uuid):
        > email
        # Will this app need to hash/check user passwords? (yes/no) [yes]
        > 
        # Your User class can implement "PasswordAuthenticatedUserInterface"!
        # Add "use Symfony\Component\Security\Core\User\PasswordAuthenticatedUserInterface;" to the class automatically (yes/no) [yes]
        > 
        # created: src/Entity/User.php
        # created: src/Repository/UserRepository.php
b) **Konfiguracja uwierzytelniania**
- Po wygenerowaniu encji Symfony doda automatycznie wpis security.yaml z minimalnym ustawieniem firewalli i providerów. Przykład podstawowej konfiguracji:
    ```yaml
    # config/packages/security.yaml
    security:
        encoders:
            App\Entity\User:
                algorithm: auto
    
        providers:
            app_user_provider:
                entity:
                    class: App\Entity\User
                    property: email
    
        firewalls:
            dev:
                pattern: ^/(_(profiler|wdt)|css|images|js)/
                security: false
    
            main:
                anonymous: true
                provider: app_user_provider
                form_login:
                    login_path: app_login
                    check_path: app_login
                logout:
                    path: app_logout
                    target: app_home
    
        access_control:
            - { path: ^/admin, roles: ROLE_ADMIN }
            - { path: ^/profile, roles: ROLE_USER }
    ```
- Trasy app_login, app_logout można wygenerować poprzez:

```bash
php bin/console make:auth

# Wybieramy: 1) "Empty authenticator" lub 2) "Login form authenticator".
```
- Formularz logowania (LoginFormAuthenticator.php) będzie obsługiwał sprawdzanie hasła, pobieranie użytkownika z bazy itp.
  
c) **Rejestracja użytkownika**
- Można wygenerować kontroler i formularz rejestracji:
```bash
php bin/console make:registration-form

# Ten kreator stworzy:
# - RegistrationController.php
# - templates/registration/register.html.twig
# - configure Security w security.yaml (firewall, provider, encoder itp.)
```
- Formularz rejestracji będzie zawierał co najmniej pola: e-mail, hasło (haszowane), atrybuty daty utworzenia konta, ról itp.
  
d) **Role i uprawnienia**
- Domyślnie użytkownik tworzony przez kreator otrzymuje rolę ```ROLE_USER```. Można manualnie zarządzać tablicą roles w encji ```User```.
- W ```security.yaml``` definiujemy hierarchię ról, np.:
  
```yaml
role_hierarchy:
    ROLE_ADMIN: [ROLE_USER]
    ROLE_SUPER_ADMIN: [ROLE_ADMIN, ROLE_ALLOWED_TO_SWITCH]
```
- Aby zabezpieczyć konkretne akcje w kontrolerze, używamy adnotacji lub kontroli w kodzie:

```php
// Przy użyciu adnotacji (jeśli zainstalowany sensio/framework-extra-bundle):
use Sensio\Bundle\FrameworkExtraBundle\Configuration\IsGranted;

#[IsGranted('ROLE_ADMIN')]
public function adminDashboard(): Response
{
    // ...
}
```
- Dodatkowo można tworzyć Voter („głosowisko”) – klasę, która decyduje, czy dany użytkownik może wykonać operację na określonym obiekcie (np. edytować tylko swoje zamówienie).
  
e) **Panel zarządzania użytkownikami**
- W standardowej instalacji nie ma gotowego panelu users; należy albo stworzyć własny CRUD dla encji User, albo skorzystać z pakietu:
   - EasyAdminBundle: pozwala w prosty sposób zarządzać encjami (Users, Role, itp.).
   - SonataAdminBundle: bardziej rozbudowany, ale wymaga solidniejszej konfiguracji.
  
f) **Uwierzytelnianie zewnętrzne**
- Uwierzytelnianie zewnętrzne
   - Można też wykorzystać FOSUserBundle (Starszy, ale czasem używany) lub inne implementacje (OAuth, LDAP, JWT itp.).
   - Do integracji z zewnętrznym serwisem autoryzacji (np. Google, Facebook) używa się HWIOAuthBundle lub Symfonycasts KnpOAuthBundle.
#### 2) Wordpress

Zarządzanie użytkownikami w WordPressie opiera się na prostym, ale elastycznym modelu ról i uprawnień. Wszystkie podstawowe operacje na użytkownikach można wykonać w kokpicie. Nie są potrzebne do tego żadne wtyczki.
Opcje do zarządzania użytkownikami znajdują się w zakładce `Użytkownicy` po lewej stronie na pasku nawigacyjnym.

![Otwarta zakładka zarządzania użytkownikami](doc-resources/Uzytkownicy.png)

Z tego miejsca można:
- przeglądać listę kont – z podziałem na role i liczbę opublikowanych treści;
- filtrować i wyszukiwać nazwiska, e‑maile lub role, co ułatwia szybkie odszukanie właściwej osoby;
- wykonywać akcje zbiorcze (np. przypisanie nowej roli lub usunięcie konta kilku osobom naraz);
- resetować hasła i wysyłać linki „Ustaw nowe hasło” w przypadku zagubienia danych logowania;
- włączać/wyłączać dwustopniowe logowanie, jeśli korzystasz z wtyczek do 2FA lub passkeys.

Podsekcja `Utwórz użytkownika` pozwala ręcznie zarejestrować świeże konto (wraz z automatycznym e‑mailem powitalnym) albo wysłać zaproszenie, dzięki któremu użytkownik sam ustawi hasło. Z kolei każdy zalogowany widzi w menu pozycję Profil – tu zmieni swoje dane wyświetlane publicznie, podpis awatar z Gravatara, język kokpitu czy klucze aplikacji do REST API.

![Strona tworzenia użytkownika](doc-resources/Utworz-uzytkownika.png)

Jak WordPress zarządza uprawnieniami?
Sercem systemu jest model ról i uprawnień (Roles & Capabilities). Domyślne role – od Subskrybenta aż po Administratora – mają przypisane konkretne „zdolności” (capabilities), takie jak edit_posts czy install_plugins. Dzięki temu WordPress może precyzyjnie określić, kto widzi daną opcję w kokpicie i jakie operacje wolno mu wykonać. Jeśli prowadzisz instalację wielosieciową (Multisite), nad wszystkimi witrynami stoi jeszcze rola Super Admin.

Co, jeśli potrzebujesz czegoś więcej?
Choć wbudowane narzędzia wystarczą do prostych stron firmowych czy blogów, rozbudowane projekty szybko wymagają dodatkowych możliwości. Najpopularniejsze klasy rozszerzeń to:

| Typ wtyczki | Do czego służy? | Przykładowe funkcje |
|-------------|-----------------|---------------------|
| **Edytory ról** | Tworzenie nowych ról lub modyfikacja istniejących bez dotykania kodu. | Graficzne zaznaczanie/odznaczanie capabilities; klonowanie ról; masowe przypisywanie do kont. *User Role Editor, Members* |
| **Profile & rejestracja front‑end** | Zamiana domyślnego, „szarego” formularza WP na własny, dostosowany do motywu. | Kreatory pól profilu, avatary, pola „zgoda RODO”, reCAPTCHA; wieloetapowa rejestracja. *WP User Manager, Profile Press* |
| **Systemy członkostw (membership)** | Sprzedaż subskrypcji, kursów, treści „tylko dla zalogowanych”. | Płatne lub darmowe poziomy dostępu, automatyczne nadawanie/odbieranie ról, integracja z płatnościami. *MemberPress, Paid Memberships Pro* |
| **Sklepy e‑commerce** | WooCommerce dodaje role *Customer* i *Shop Manager*, a zarządzanie kontami klientów odbywa się w osobnym panelu zamówień. | Historia zakupów, reset haseł na maila, import/eksport klientów, segmentacja odbiorców. |
| **Bezpieczeństwo i 2FA** | Hartowanie logowania i monitorowanie aktywności. | Authenticator, passkeys/WebAuthn, blokady IP, dziennik „kto, co i kiedy” w kokpicie. *Wordfence Login Security, WP 2FA, Simple History* |
| **Social / SSO / LDAP** | Logowanie jednym kliknięciem przez Google, Facebooka lub serwer firmowy. | Mapowanie pól profilu, automatyczne zakładanie kont, wymuszanie domeny e‑mail. *Nextend Social Login, miniOrange LDAP* |

Dzięki hookom i REST API wtyczki mogą też uruchamiać akcje przy każdym utworzeniu lub zmianie konta – na przykład dodać nowego użytkownika do listy mailingowej lub wysłać powiadomienie na Slacka. Narzędzia deweloperskie (WP‑CLI, GraphQL) pozwalają natomiast masowo importować tysiące kont czy modyfikować role poleceniem w terminalu.

---
## Koszyk i zamówienia
#### 1) Symfony
- Ten widok pełni rolę interaktywnego koszyka zakupowego w aplikacji SymfonyShop. Użytkownik widzi tutaj listę produktów, które dodał do koszyka – każda pozycja składa się ze zdjęcia, nazwy (linkowanej do strony szczegółów produktu) oraz ceny. Dzięki przyciskowi „Delete” można od razu usunąć niechciane pozycje, a na dole wyświetlana jest automatycznie wyliczana suma całego zamówienia. Całość działa w oparciu o dane przechowywane w localStorage przeglądarki: skrypt JavaScript odczytuje je przy ładowaniu strony, generuje dynamicznie wiersze tabeli i pozwala na bieżąco aktualizować zarówno zawartość, jak i łączną kwotę koszyka.

![Koszyk Symfony](doc-resources/symfony-cart.png) 
  
#### 2) Wordpress

---
## Panel administratora
#### 1) Symfony
- W Symfony domyślnie nie ma gotowego panelu administracyjnego, dlatego najpopularniejsze podejście to:
a) **EasyAdminBundle**
 - Instalacja:
   ```bash
   composer require easycorp/easyadmin-bundle
   ```
 - Konfiguracja: w pliku ```config/routes/easy_admin.yaml```:
```yaml
easy_admin:
    resource: '@EasyAdminBundle/Controller/EasyAdminController.php'
    prefix: /admin
```
 - Konfiguracja panelu w ```config/packages/easy_admin.yaml```:
```yaml
easy_admin:
site_name: 'Panel Admina'
design:
    menu:
        - { label: 'Dashboard', route: 'easyadmin' }
        - { label: 'Produkty', entity: 'Product' }
        - { label: 'Użytkownicy', entity: 'User' }
        - { label: 'Zamówienia', entity: 'Order' }
entities:
    Product:
        class: App\Entity\Product
        list:
            title: 'Produkty'
            fields:
                - id
                - name
                - price
        form:
            fields:
                - name
                - description
                - price
    User:
        class: App\Entity\User
        list:
            fields: [ id, email, roles ]
        form:
            fields: [ email, roles ]
    Order:
        class: App\Entity\Order
        list:
            fields: [ id, user, status, total, createdAt ]
        show:
            fields: [ orderItems, total, status, createdAt, user ]
```

- Po wgraniu konfiguracji wchodzimy w przeglądarce na http://localhost:8000/admin.
- ![Panel Admina Symfony](doc-resources/symfony-admin.png) 

#### 2) Wordpress
### Kokpit
![Kokpit WordPress](doc-resources/wp-admin.png)  
Centralny pulpit nawigacyjny prezentuje kluczowe informacje i udostępnia szybki dostęp do najczęściej używanych funkcji:  
- **Stan witryny (Site Health)**  
  - Automatyczny monitoring wydajności, bezpieczeństwa oraz zgodności z zaleceniami WordPressa.  
  - Wykrywanie przestarzałych wtyczek, brakujących rozszerzeń PHP czy nieprawidłowych uprawnień plików.  
- **Powiadomienia i aktualizacje**  
  - Informowanie o dostępnych wersjach WordPressa, motywów i wtyczek.  
  - Jednoklikowa instalacja aktualizacji lub planowanie ich na dogodny moment.  
- **Widżety szybkiego dostępu**  
  - Tworzenie szkiców wpisów, stron lub zadań przy użyciu konfigurowalnych kafli.  
  - Podsumowanie aktywności użytkowników i komentarzy w czasie rzeczywistym.  
  - Możliwość dostosowania układu i widoczności widżetów w zależności od potrzeb administratora.

---

### Wpisy  
![Sekcja Wpisy](doc-resources/wp-admin-strony.png)  
Kompleksowe zarządzanie treścią blogową i newsami:  
- **Blokowy edytor Gutenberg**  
  - Komponowanie układów stron z wykorzystaniem predefiniowanych bloków (tekst, obrazy, galerie, multimedia, shortcodes).  
  - Złożone konfiguracje kolumn, tła i stylów CSS bez konieczności pisania kodu.  
- **Kategoryzacja i tagowanie**  
  - Tworzenie hierarchii kategorii i oznaczanie wpisów tagami dla lepszej nawigacji i SEO.  
  - Bulk–akcje na wielu wpisach jednocześnie (zmiana statusu, przypisanie kategorii).  
- **Harmonogram publikacji**  
  - Planowanie automatycznej publikacji wpisów w określonym dniu i godzinie.  
  - Możliwość cofania terminu publikacji lub wcześniejszego udostępnienia treści.  
- **Rewizje i historia zmian**  
  - Śledzenie kolejnych wersji wpisu, porównywanie różnic i przywracanie wcześniejszych stanów.

---

### Media  
![Biblioteka multimediów](doc-resources/wp-admin-media.png)  
Zarządzanie wszystkimi zasobami graficznymi, wideo i dokumentami:  
- **Przesyłanie i organizacja**  
  - Import plików metodą drag-and-drop lub wybór z lokalnego dysku.  
  - Automatyczne generowanie miniaturek w kilku rozmiarach (thumbnail, medium, large).  
- **Edycja metadanych**  
  - Uzupełnianie tytułu, opisu, tekstu alternatywnego (alt) i podpisu, co wpływa na optymalizację SEO i dostępność.  
  - Modyfikacja parametrów obrazów (obrót, kadrowanie, skalowanie) wbudowanym edytorem.  
- **Filtrowanie i przeszukiwanie**  
  - Sortowanie zasobów według typu pliku, daty, nazwy lub rozmiaru.  
  - Grupowe zaznaczanie i usuwanie niepotrzebnych plików.

---

### Strony  
![Lista stron](doc-resources/wp-admin-strony.png)  
Obsługa statycznych podstron witryny:  
- **Hierarchia i atrybuty**  
  - Tworzenie stron nadrzędnych i podrzędnych, definiowanie szablonów (np. pełna szerokość, z sidebar’em).  
  - Ustalanie kolejności wyświetlania w menu poprzez ustawienie atrybutów „Kolejność”.  
- **Szablony i bloki globalne**  
  - Zastosowanie gotowych wzorców bloków lub zapis własnych bloków do ponownego wykorzystania.  
  - Integracja z page builderami, umożliwiająca tworzenie dedykowanych wzorców stron.  
- **Planowanie i dostęp**  
  - Harmonogram publikacji, ochrona strony hasłem lub ograniczenie widoczności dla zarejestrowanych użytkowników.

---

### Edycja strony (Page Builder)  
![Edycja strony – Page Builder](doc-resources/wp-admin-edycja-strony.png)  
Zaawansowane narzędzie do tworzenia niestandardowych układów:  
- **Drag & Drop**  
  - Przeciąganie sekcji, kolumn i widżetów bezpośrednio na podgląd strony.  
- **Elastyczne siatki (Flexbox / Grid)**  
  - Konfiguracja kierunku, rozmieszczenia i proporcji elementów dla uzyskania responsywnego designu.  
- **Stylizacja i animacje**  
  - Definiowanie stylów tła, obramowań, cieni, marginesów i paddingów w intuicyjnym panelu.  
  - Możliwość dodawania animacji wejścia elementów (fade, slide itp.) oraz efektów hover.

---

### Komentarze  
Sekcja moderacji dyskusji nad treściami:  
- **Automatyczne filtrowanie**  
  - Wykrywanie spamu za pomocą reguł Akismet lub innych wtyczek antyspamowych.  
- **Panel moderacji**  
  - Szybkie akcje: zatwierdzenie, oznaczenie jako spam, przeniesienie do kosza.  
  - Masowe operacje na wielu komentarzach jednocześnie.

---

### Wygląd  
![Motywy i personalizacja](doc-resources/wp-admin-wyglad.png)  
Dostosowanie wizualnej oprawy witryny:  
- **Instalacja motywów**  
  - Pobieranie i aktywacja motywów z oficjalnego repozytorium lub przesłanych archiwów.  
- **Customizer w czasie rzeczywistym**  
  - Podgląd zmian w układzie, kolorystyce, typografii, tle i nagłówkach przed zapisaniem.  
  - Konfiguracja menu nawigacyjnego, widgetów w sidebarze i stopce.  
- **Edytor plików motywu**  
  - Bezpośrednia edycja plików szablonu (PHP, CSS, JS) z uwzględnieniem funkcji override w motywach potomnych (child themes).

---

### Wtyczki  
![Zarządzanie wtyczkami](doc-resources/wp-admin-wtyczki.png)  
Rozszerzanie funkcjonalności witryny:  
- **Instalacja i aktywacja**  
  - Wyszukiwanie, instalacja i konfiguracja wtyczek z oficjalnego repozytorium WP lub z lokalnych paczek.  
- **Zarządzanie aktualizacjami**  
  - Harmonogram automatycznych aktualizacji, przegląd dostępnych wersji i zabezpieczenie przed konfliktami.  
- **Konfiguracja**  
  - Bezpośrednie linki do stron ustawień każdej wtyczki, wsparcie dla multisite i ról użytkowników.

---

### Użytkownicy  
Sekcja zarządzania kontami i uprawnieniami:  
- **Role i uprawnienia**  
  - Przypisywanie ról (Administrator, Redaktor, Autor, Współpracownik, Subskrybent) z różnymi poziomami dostępu.  
- **Profil użytkownika**  
  - Edycja danych osobowych, ustawień biogramu, avataru i haseł.  
- **Import/eksport**  
  - Masowe dodawanie użytkowników przez pliki CSV lub integracja z systemami LDAP/SSO.

---

### Narzędzia  
Zestaw pomocniczych operacji administracyjnych:  
- **Import/Eksport treści**  
  - Eksport całej zawartości witryny lub wybranych elementów (wpisy, strony, komentarze) w formacie XML (WXR).  
  - Import danych z zewnętrznych systemów (WordPress, Blogger, CSV).  
- **Diagnostyka i konserwacja**  
  - Site Health: szczegółowe raporty o konfiguracji serwera, wydajności i bezpieczeństwie.  
  - Narzędzia deweloperskie: możliwość wykonania operacji naprawczych (reset permalinek, optymalizacja bazy danych).

---

### Ustawienia  

#### Ogólne  
![Ustawienia ogólne](doc-resources/wp-admin-ustawienia.png)  
Konfiguracja podstawowa witryny:  
- **Tożsamość witryny**  
  - Nazwa, slogan (tagline) i favicon (ikonka przeglądarki).  
- **Adresy URL**  
  - Adres instalacji WordPress (WordPress Address URL) i adres strony widocznego front-endu (Site Address URL).  
- **Użytkownicy**  
  - Domyślna rola nowych rejestrujących się użytkowników, włączenie/wyłączenie rejestracji.  
- **Lokalizacja**  
  - Język interfejsu, strefa czasowa, format daty i czasu.

#### Permalinki  
![Permalinki](doc-resources/ustawienia-bezposrednie-odnosniki.png)  
Zarządzanie strukturą adresów URL:  
- **Gotowe schematy**  
  - Prosty (identyfikator wpisu), Data + Nazwa, Miesiąc + Nazwa, Liczbowy, Nazwa wpisu.  
- **Własny format**  
  - Dowolne połączenie znaczników: `%year%`, `%monthnum%`, `%day%`, `%post_id%`, `%postname%`, `%category%`, `%author%`.  
- **SEO i użyteczność**  
  - Konstrukcja przyjaznych dla użytkownika i wyszukiwarek URL, eliminacja nieczytelnych parametrów.

---

Opisane możliwości panelu administracyjnego WordPress pozwalają na kompleksowe zarządzanie każdą stroną — od treści i mediów, przez wygląd i funkcje, aż po zaawansowane opcje wydajności i bezpieczeństwa.

---
## Dane porównawcze i metryka
**1. Liczba plików**

**2. Ilość zależności**

**3. Rozmiar projektu na dysku**

**4. Zużycie pamięci RAM**

**5. Czasy ładowania widoków, rozmiar wygenerowanej strony (payload)**

a) **Dashboard**

b) **Kolekcja butów**

c) **Podgląd danego produktu**

d) **Koszyk**

**6. Czas zapytania do bazy i liczba zapytań SQL**

a) **Dashboard**

b) **Kolekcja butów**

c) **Podgląd danego produktu**

d) **Koszyk**

---
## Szablony i wygląd (UI/UX)
#### 1) Symfony
- W Symfony możesz korzystać z silnika szablonów Twig, ponieważ jest to domyślny, lekki i wydajny sposób na oddzielenie warstwy prezentacji od logiki aplikacji – Twig kompiluje szablony do czystego PHP, wspiera dziedziczenie bloków i łatwo integruje się z systemem routingu i helperów Symfony.

- Czym jest Twig?
   - Twig to domyślny silnik szablonów w Symfony. Pozwala oddzielić logikę PHP od prezentacji HTML-owej: w szablonach używamy lekkiej składni ({{ }} do wyrenderowania zmiennych, {% %} do instrukcji, pętli czy dziedziczenia). Ma szybki kompilator – przy pierwszym       wywołaniu Twój .twig jest przetwarzany do czystego PHP i cache’owany.
   - Struktura plików w projekcie dla szablonów Twig
     
    ![Symfony Twig Templates](doc-resources/symfony-templates.png)
  - Przykład bazowego szablonu ```base.html.twig```
    
    ```twig
    {# templates/base.html.twig #}
    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="UTF-8">
        <title>{% block title %}Symfony Shop{% endblock %}</title>
        {% block stylesheets %}
            <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css">
            <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@mdi/font@7.4.47/css/materialdesignicons.min.css">
            <style>
                html, body {
                    height: 100%;
                    margin: 0;
                    padding: 0;
                    display: flex;
                    flex-direction: column;
                }
                body > main {
                    flex: 1;
                }
                footer {
                    background-color: #0E3F35;
                    color: #fff;
                    padding: 20px 0;
                }
                .header-container {
                    background-color: #023430;
                    width: 100%;
                    height: 40%;
                }
            
                .bar-container {
                    margin-top: 15px;
                    background-color: #e3e3e3;
                    padding: 16px 20px 16px 20px;
                    border-radius: 25px;
                }
                .bar-container-text {
                    color: black;
                    font-weight: bold;
                    font-size: 16px;
                }
                /* ------------------------ NAVBAR ------------------------ */
                .custom-navbar {
                    background-color: #023430;
                    display: flex;
                    align-items: center;
                    justify-content: space-between;
                    padding: 1rem 2rem;
                }
                .custom-navbar .logo {
                    color: #fff;
                    font-size: 1.5rem;
                    font-weight: 700;
                    text-decoration: none;
                }
                .custom-navbar .logo:hover {
                    transform: scale(1.02);
                }
                .custom-navbar ul {
                    list-style: none;
                    display: flex;
                    gap: 2rem;
                }
                .custom-navbar li {
                    display: inline-block;
                }
                .custom-navbar a {
                    color: #000000;
                    text-decoration: none;
                    font-weight: 500;
                }
                .custom-navbar a:hover {
                    color: #878787;
                    text-decoration: underline;
                }
                .bar-container-text i {
                    font-size: 24px;
                }
                .bar-container-icons {
                    margin-top: 10px;
                    background-color: #e3e3e3;
                    padding: 8px 16px 8px 16px;
                    border-radius: 25px;
                    margin-right: 30px
                }
            </style>
            <script>
                function showSnackbar(message, error = false) {
                    const snackbar = document.getElementById("snackbar");
                    if (error) {
                        snackbar.style.backgroundColor = "#f44336"; // Czerwony kolor dla błędów
                    } else {
                        snackbar.style.backgroundColor = "#3edc24";
                    }
                    snackbar.textContent = message;
                    snackbar.style.visibility = "visible";
                    snackbar.style.opacity = "1";
                    snackbar.style.bottom = "50px";
                    setTimeout(function() {
                        snackbar.style.opacity = "0";
                        snackbar.style.bottom = "30px";
                        setTimeout(function() {
                            snackbar.style.visibility = "hidden";
                        }, 500);
                    }, 3000);
                }
            </script>
    
        {% endblock %}
    </head>
    <body>
    {% block header %}
        <header>
            <div class="header-container">
                <nav class="custom-navbar">
                    <a href="/home" class="logo"><img width="14%" style="margin-right: 10px; margin-bottom: 5px;" src="{{ asset('images/SymfonyIcon.png') }}" alt="HomePageTopImage">SymfonyShop</a>
                    <ul class="bar-container">
                        <li class="bar-container-text">
                            <a href="/home">Home</a>
                        </li>
                        <li class="bar-container-text">
                            <a href="/products">Shoes Collection</a>
                        </li>
                        <li class="bar-container-text">
                            <a href="/about">About</a>
                        </li>
                    </ul>
                    <ul class="bar-container-icons">
                        <li class="bar-container-text">
                            <a href="/products"><i class="mdi mdi-magnify"></i></a>
                        </li>
                        <li class="bar-container-text">
                            <a href="/products"><i class="mdi mdi-heart-outline"></i></a>
                        </li>
                        <li class="bar-container-text">
                            <a href="/cart"><i class="mdi mdi-cart-outline" id="cart-icon"></i><span id="cart-count" style="background-color: red; color: white; border-radius: 50%; padding: 2px 8px; font-size: 0.8rem; position: relative; top: -10px; left: -5px;">0</span></a>
                        </li>
                    </ul>
                </nav>
            </div>
        </header>
    {% endblock %}
    <main>
        {% block body %}
        {% endblock %}
    </main>
    <footer class="mt-5">
        <div class="text-center">
            <p class="mb-0">© 2025 Symfony Shop - All rights reserved.</p>
        </div>
    </footer>
    <div id="snackbar" style="
        visibility: hidden;
        min-width: 250px;
        margin-left: -200px;
        color: #fff;
        text-align: center;
        border-radius: 20px;
        padding: 16px;
        position: fixed;
        z-index: 9999;
        left: 50%;
        bottom: 30px;
        font-size: 1rem;
        opacity: 0;
        transition: opacity 0.5s, bottom 0.5s;
    ">
    </div>
    
    {% block javascripts %}
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
    {% endblock %}
    </body>
    </html>
    ```
   - Przykład szablonu dziedziczącego ```product/show.html.twig```
     
  ```twig
    {% extends 'base.html.twig' %}

    {% block title %}
    {{ product.brand }} {{ product.model }}
    {% endblock %}

    {% block stylesheets %}
        {{ parent() }}
        <style>
            .product-show-section {
                max-width: 80%;
                height: 100%;
                margin: 0 auto;
                padding: 3rem 2rem;
            }

            .product-details-wrapper {
                display: flex;
                gap: 3rem;
                align-items: flex-start;
                background-color: #f9f9f9;
                padding: 2rem;
                border-radius: 15px;
            }

            .product-image {
                flex: 1;
            }

            .product-image img {
                width: 100%;
                border-radius: 15px;
                transition: transform 0.3s ease;
            }

            .product-image img:hover {
                transform: scale(1.03);
            }

            .product-info {
                flex: 1.5;
            }

            .product-info h2 {
                font-size: 2rem;
                font-weight: 700;
                margin-bottom: 0.75rem;
            }

            .product-info .price {
                font-size: 1.5rem;
                font-weight: bold;
                color: #023430;
                margin: 1rem 0;
            }

            .product-info .rating {
                color: #FFB400;
                font-weight: bold;
                font-size: 1.1rem;
            }

            .product-info .description {
                margin: 1.5rem 0;
                line-height: 1.6;
            }

            .product-colors, .product-sizes {
                display: flex;
                gap: 0.5rem;
                margin-bottom: 1rem;
            }

            .product-color, .product-size {
                width: 25px;
                height: 25px;
                border-radius: 3px;
                border: 1px solid #ccc;
                display: flex;
                align-items: center;
                justify-content: center;
                font-size: 0.8rem;
                font-weight: bold;
                padding: 0.5rem;
            }


            .add-to-cart-btn {
                background-color: #f1f1f1;
                color: black;
                border: 2px solid black;
                padding: 0.5rem 1rem;
                font-size: 1rem;
                border-radius: 55px;
                cursor: pointer;
                font-weight: bold;
                transition: all 0.25s ease;
            }

            .add-to-cart-btn:hover {
                background-color: #dcdcdc;
                transform: scale(1.05);
            }
        </style>
    {% endblock %}
      {% block body %}
        <section class="product-show-section" style="margin-bottom: 10%">
            <div class="product-details-wrapper">
                <div class="product-image">
                    <img src="{{ asset(product.imageUrl ?: 'images/defaultImage.png') }}" alt="{{ product.brand }} {{ product.model }}">
                </div>
                <div class="product-info">
                    <h2>{{ product.brand }} {{ product.model }}</h2>
                    <div class="rating">
                        <i class="mdi mdi-star"></i> {{ product.rating }}
                    </div>
                    <div class="price">${{ product.price }}</div>
                    <div class="description">{{ product.description ?: 'Brak opisu dla tego produktu.' }}</div>

                    {% if product.colors %}
                        <div>
                            <strong>Kolory:</strong>
                            <div class="product-colors">
                                {% for color in product.colors %}
                                    <div class="product-color" style="background-color: {{ color }}">&nbsp;</div>
                                {% endfor %}
                            </div>
                        </div>
                    {% endif %}

                    {% if product.sizes %}
                        <div>
                            <strong>Rozmiary:</strong>
                            <div class="product-sizes">
                                {% for size in product.sizes %}
                                    <div class="product-size">{{ size }}</div>
                                {% endfor %}
                            </div>
                        </div>
                    {% endif %}

                    <button class="add-to-cart-btn"
                            data-product-id="{{ product.id }}"
                            data-product-name="{{ product.brand }} {{ product.model }}"
                            data-product-price="{{ product.price }}">
                        Dodaj do koszyka
                    </button>
                </div>
            </div>
        </section>
    {% endblock %}
      {% block javascripts %}
        <script>
            document.addEventListener('DOMContentLoaded', function () {
                const cartCount = document.getElementById('cart-count');
                const addToCartButtons = document.querySelectorAll('.add-to-cart-btn');

                function getCart() {
                    const cart = localStorage.getItem('cart');
                    return cart ? JSON.parse(cart) : [];
                }

                function saveCart(cart) {
                    localStorage.setItem('cart', JSON.stringify(cart));
                }

                function updateCartCount() {
                    const cart = getCart();
                    cartCount.textContent = cart.length;
                }

                addToCartButtons.forEach(button => {
                    button.addEventListener('click', function () {
                        const productId = this.dataset.productId;
                        const productName = this.dataset.productName;
                        const productPrice = this.dataset.productPrice;

                        let cart = getCart();

                        if (cart.some(item => item.id === productId)) {
                            showSnackbar('Product already in cart!', true);
                            return;
                        }
                        cart.push({
                            id: productId,
                            name: productName,
                            price: productPrice
                        });
                        saveCart(cart);
                        updateCartCount();
                        showSnackbar(`Product ${productName} was added to cart!`);
                    });
                });

                updateCartCount();
            });
        </script>
    {% endblock %}
  ```
  - Mając już widoki, należy utworzyć routingi oraz kontolery dla danych widoków, przykład użycia ```CartController.php```
    
      ```php
    <?php
    
    namespace App\Controller;
    
    use App\Entity\Product;
    use Doctrine\ORM\EntityManagerInterface;
    use Symfony\Bundle\FrameworkBundle\Controller\AbstractController;
    use Symfony\Component\HttpFoundation\Response;
    use Symfony\Component\HttpFoundation\Request;
    use Symfony\Component\HttpFoundation\JsonResponse;
    use Symfony\Component\Routing\Annotation\Route;
    
    class CartController extends AbstractController
    {
        #[Route('/cart', name: 'app_cart_show')]
        public function show(): Response
        {
            return $this->render('cart/show.html.twig', [
            ]);
        }
    
        #[Route('/cart/save', name: 'app_cart_save', methods: ['POST'])]
        public function save(Request $request, EntityManagerInterface $entityManager)
        {
            $data = json_decode($request->getContent(), true);
            $cart = $data['cart'] ?? [];
        
            $request->getSession()->set('cart', $cart);
        
            $idProducts = array_column($cart, 'id');
            $cartProducts = array();
            if (!empty($idProducts)) {
            $qb = $entityManager->createQueryBuilder();
                $qb->select('p.id, p.brand, p.model, p.price, p.description, p.imageUrl, p.colors, p.sizes')   
                    ->from(Product::class, 'p')
                    ->where($qb->expr()->in('p.id', $idProducts))
                ; 
                $query = $qb->getQuery();
                $cartProducts = $query->getResult();
            }
        
            return new Response(
                json_encode($cartProducts),
                200,
                array('content-type' => 'application/json')
            );
        }
    }
    ```
  - Jak to działa „od środka” dla np. podglądu koszyka?
      - Przeglądarka GET-em prosi /cart.

      - Symfony dopasowuje trasę app_cart_show i wywołuje show().

      - Metoda render():

      - Ładuje templates/cart/show.html.twig, widzi {% extends 'base.html.twig' %},

      - Kompiluje wspólnie z base.html.twig, wstrzykuje odpowiednie bloki.

      - Wynik HTML wraca do przeglądarki.
     

#### 2) Wordpress
---
## Społeczność i dokumentacja
Oficjalne źródła wiedzy obu platform stanowią punkt wyjścia dla programistów i administratorów, jednak różnią się pod względem struktury, przejrzystości i zakresu dostępnych rozwiązań.

WordPress udostępnia kompletną dokumentację na [wordpress.org/documentation](https://wordpress.org/documentation/), w której treści podzielono na sekcje: szybkość startu (getting started), przewodniki dla developerów (developer handbooks), instrukcje użytkownika (user guides) oraz obszerne rozdziały dotyczące motywów i wtyczek. Poszczególne artykuły pisane są przystępnym, nienadmiernie technicznym językiem, co ułatwia zrozumienie osobom o różnym poziomie doświadczenia. Przy większości tematów dostępne są fragmenty kodu, zrzuty ekranu i praktyczne przykłady, co sprawia, że nawet złożone zagadnienia stają się czytelne bez konieczności sięgania po dodatkowe materiały.

Symfony natomiast prezentuje dokumentację na [symfony.com/doc/current](https://symfony.com/doc/current/), podzieloną na przewodniki „from zero to hero”, szczegółowy opis komponentów, najlepsze praktyki oraz instrukcje migracji między wersjami. Struktura materiałów jest bardziej techniczna i modułowa – każdy komponent (Routing, Security, Console itp.) ma odrębny rozdział, co pozwala skupić się na wąskich obszarach funkcjonalności. Przykłady kodu w PHP, YAML i XML są dokładne, lecz wymagają pewnej wprawy w odczycie i adaptacji, co może początkowo spowolnić proces nauki.

Pod względem liczby dostępnych gotowych rozwiązań i fragmentów “gotowego do wdrożenia” kodu WordPress góruje dzięki ogromnemu ekosystemowi wtyczek i motywów oraz aktywnej społeczności publikującej tutoriale i snippet’y w setkach blogów. W efekcie większość typowych zadań (tworzenie formularza kontaktowego, integracja z API, konfiguracja SEO) można zrealizować w kilka minut, korzystając z gotowych materiałów. Symfony oferuje bardziej ustrukturyzowane wskazówki – każdy przykład ilustruje dobre praktyki i wzorce projektowe, ale wdrożenie często wymaga implementacji wielu kroków ręcznie, co zwiększa kontrolę kosztem szybkości.

Ważnym elementem wsparcia są fora i kanały Q&A. WordPress.org/support gromadzi miliony wpisów i odpowiedzi, jednak duża liczba wątków może utrudniać szybkie odnalezienie rozwiązania specyficznego problemu. Symfony natomiast korzysta z oficjalnego forum, Slacka oraz Stack Overflow, gdzie mniejsza, ale wysoce wyspecjalizowana grupa ekspertów dostarcza odpowiedzi bardziej precyzyjne i zgodne z najlepszymi praktykami frameworka.

Pod względem lokalizacji i dostępności materiałów WordPress wygrywa liczbą tłumaczeń (ponad 50 języków), co przekłada się na komfort nauki w rodzimym języku. Dokumentacja Symfony dostępna jest w kilkunastu wersjach językowych, a większość aktualizacji trafia na serwer centralny niemal równocześnie z wydaniem głównym, co zapewnia spójność treści, choć czasem kosztem opóźnień w tłumaczeniach.

Podsumowując, WordPress oferuje bardziej przystępną, bogato ilustrowaną i szybko działającą dokumentację, idealną dla osób szukających szybkich rozwiązań i szerokiego wyboru gotowych fragmentów kodu. Symfony natomiast dostarcza głęboką, modułową dokumentację skupioną na dobrych praktykach i architekturze aplikacji, co może wymagać większego nakładu pracy, lecz jednocześnie gwarantuje solidne, długoterminowe podstawy projektowe.

---
## Podsumowanie
