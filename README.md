# Responsive Portfolio

## Om projektet

Det här projektet är en personlig portfolio som visar mina kunskaper inom webbutveckling, programmering och cybersäkerhet.

Portfolion består av fyra HTML-sidor:

- Hem
- Om mig
- Projekt
- Kontakt

Sidorna är länkade med en gemensam navigation och innehåller realistiskt innehåll, bilder och ett kontaktformulär.

## Responsiv design

Jag har arbetat mobile-first. Grundlayouten är anpassad för smala skärmar och ändras sedan med media queries när det finns mer utrymme.

Jag använder två huvudsakliga breakpoints:

- 700px – används när navigation, hero och kort behöver mer utrymme.
- 1000px – används för att visa tre projektkolumner på bredare skärmar.

Breakpoints valdes utifrån när innehållet behövde ändra layout och inte utifrån en specifik mobil eller dator.

## Flexbox

Jag använder Flexbox bland annat för navigationen och kortlistan.

Navigationen börjar som en kolumn på mindre skärmar och ändras till en rad vid 700px.

Även kortlistan använder Flexbox för att kunna gå från en kolumn till flera kort bredvid varandra.

## CSS Grid

Jag använder CSS Grid för bland annat:

- Hero-sektionen
- Projektkorten
- Kontaktsektionen

Projektkorten börjar med en kolumn på små skärmar, två kolumner från 700px och tre kolumner från 1000px.

## Två lösta problem

### Problem 1 – Navigation på mindre skärmar

**Problem:**  
Navigationen blev svår att använda när skärmen var smal eftersom det fanns mindre plats för länkarna.

**Observation:**  
På en liten skärm fungerade det bättre att placera navigationslänkarna under varandra. På en större skärm fanns det tillräckligt med plats för att placera dem bredvid varandra.

**CSS:** 
Jag använde Flexbox och en min-width-media query.

**Change:**  
Navigationen använder `flex-direction: column` i grundläget och ändras till `row` vid 700px.

**Test:**  
Jag testade sidan på både smalare och bredare skärmar och kontrollerade att navigationen ändrade layout utan horisontell scroll.

**Explanation:**  
Jag använde mobile-first och ändrade layouten när innehållet behövde mer utrymme.

### Problem 2 – Projektkorten på olika skärmstorlekar

**Problem:**  
Projektkorten behövde fungera på både små och stora skärmar utan att innehållet blev trångt.

**Observation:**  
På en smal skärm fungerade ett projekt per rad bäst. När skärmen blev bredare fanns det plats för fler projekt bredvid varandra.

**CSS:**  
Jag använde CSS Grid och två min-width-media queries.

**Change:**  
Projektkorten använder en kolumn i grundläget, två kolumner från 700px och tre kolumner från 1000px.

**Test:**  
Jag testade vid ungefär 650px, 700px och 1000px och kontrollerade även storlekar mellan breakpoints.

**Explanation:**  
Grid gör att projektkorten kan ändra antal kolumner beroende på hur mycket utrymme som finns.

## Tillgänglighet och användbarhet

Jag har testat navigationen med tangentbord och kontrollerat att fokus syns tydligt på länkar, formulärfält och knappar.

Jag har även kontrollerat att bilderna har relevanta alt-texter och att länkarna fungerar.

## Validering

Alla egna HTML-sidor har validerats och kontrollerats utan fel eller varningar.

CSS-filen har också validerats utan fel.

## Testning

Jag har testat webbplatsen på olika skärmstorlekar och kontrollerat:

- Responsiv layout
- Navigation
- Länkar
- Bilder
- Formulär
- Tangentbordsfokus
- Horisontell scroll
- Media queries

Projektet är byggt med HTML5 och CSS och använder semantisk HTML, Flexbox, CSS Grid och responsive design.
