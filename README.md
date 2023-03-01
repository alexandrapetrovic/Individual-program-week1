# Individual-program-week1

📖: dokumentacija ili clanak
🛠: online alati / alati za testiranje
📹: slika ili video sadrzaj
Osnovne Frontend Tehnologije
HTML
HTML
HEAD
BODY
CSS
JAVASCRIPT
HTML - Hyper Text Markup Language
HTML nam omogućava da definišemo strukturu i sadržaj web stranice.

Minimalna struktura stranice
Svaki HTML dokument ima sledecu strukturu:

<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Title</title>
    </head>
    <body>
        <!-- content here -->
    </body>
</html>
Doctype: Deklaracija koju navodimo na početku svakog HTML dokumenta. Govori pretraživaču kog je tipa dokument kojeg čita, na taj način pretraživač zna kako da interpretira sadržaj. Deklaracija nije HTML tag i nije case sensitive.

<!DOCTYPE html> <!-- Označava da je u pitanju HTML5 -->
⬆ back to top

HTML
Ceo dokument se nalazi unutar <html> taga. Ovaj tag se navodi odmah nakon doctype deklaracije. Unutar html taga nalaze se head i body tag. 

Note: Uvek uključi lang atribut unutar <html> taga. Ovo treba da pomogne pretraživačima.

› Language atribut: Definiše jezik na kom je napisan sadržaj dokumenta.

<html lang="en">
HEAD
Neki od elemenata koji se mogu naci unutar <head> taga su: meta, title, link, style, script.

tag	element
title	page title
meta	metadata
link	link to external source
script	Jacascript code
Preporučeni minimum tagova koje treba uključiti
Ispod su osnovni elementi za bilo koji web dokument:

<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
  Ova 2 meta taga koja su navedena iznad,
  treba da dodju prvi unutar <head> taga
  kako bi obezbedili pravilno renderovanje dokumenta.
  Svi ostali elementi dolaze posle ovih tagova.
 -->
<title>Page Title</title>
meta charset - defines the encoding of the website, utf-8 je standard. (Omogućava prikazivanje nestandardih simbola - emoji, slova sa kvačicama)

meta name="viewport" - viewport settings utiče na responsivnost mobilnih uređaja

width=device-width - koristi fizičku širinu uređaja (odlično za mobilne uređaje!)

initial-scale=1 - inicijalni zoom, 1 znači nema inicijalnog zumiranja

Note: Moguće je upotpunosti isključiti mogućnost korisniku da uvećava stranicu, međutim to nije preporučljivo. Mnogi ljudi koriste opciju zumiranja prilikom korišćenja web sajta ili aplikacije. Isključivanje je ponekad zaista neophodno za određene vrste igrica i aplikacija.

📖:  Meta charset
meta
› description: kratak opis dokumenta (do 150 karaktera). Može da se koristi kao za optimizaciju search engine rezultata. 

<meta name="description" content="A description of the page">
📖 Meta Description
› keywords: ključne reči za search engine, ključne reči se razdvajaju zarezom.

  <meta name="keywords" content="HTML, CSS, JavaScript">
Many search engines do not consider such keywords, because this feature has historically been used unreliably and even misleadingly as a way to spam search engine results in a way that is not helpful for users.

› author: omogućava da se navede autor web stranice.

<meta name="author" content="John Doe">
title
Title tag se koristi na svim stranicama (dužina title-a je bitna i utiče na SEO: Google računa širinu pixela karaktera koji se koristi u title-u. Prosečan broj za limit broja karaktera koji se koriste u title tagu je oko 55.)

<!-- Nalov dokumenta -->
<title>My First Page</title>
📖:  The Document Title element
🛠: SERP Snippet Generator
link
Link tag sastoji se od sledećih atributa:

<link rel="" type="" sizes="" href="">
rel - koristi se za definisanje veze između html dokumenta i povezanog resursa. 

type - tip povezanog resursa

sizes - za definisanje velicine ikonice

href - putanja do resursa

Primer - favicon
favicon je mala ikonica koja se prikazuje na početku tab-a pored naslova dokumenta.

 <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
📖: https://bitsofco.de/all-about-favicons-and-touch-icons/
📖: https://github.com/audreyfeldroy/favicon-cheat-sheet
BODY
Unutar <body> taga korisnimo tagove kako bismo kreirali sadržaj dokumenta. Možemo reći i da predstavlja konterjner za sve elemente koji su vidljivi na stranici kao sto su naslovi, paragrafi, slike, hiperveze, tabele, liste itd.

W3School
Komentari u HTML
Komentar je moguće posstaviti na bilo kom mestu unutar HTML dokumenta. 

Uloga komentara je da bliže objasne HTML tekst. Takođe ukoliko želimo da sakrijemo deo stranice koji ne želimo da se više prikazuje za koji još uvek nismo spremni da obrišemo.

<!-- Ovo je komentar i on se ne vidi  -->
<div class="card">
    <h2>Title</h2>
    <img src="" alt ="" >
</div>
CSS
CSS - Cassading Style Sheet

Tri načina kako uključiti css u HTML dokument
Inline style
Unutar style taga
External fajl
Inline style
Inline stilizacija direktno utiču na tag, bez korišćenja selektora.

<p style="color:red;">This is a paragraph.</p>
Style tag
<!-- Used for adding in-document CSS -->
<style>
  /* ... */
</style>
External fajl
<!-- Link to an external CSS file -->
<link rel="stylesheet" href="styles.css">
⬆ back to top
Komentari u CSS
Komentari nemaju uticaja na layout HTML dokumenta. Služe da bliže objasne kod ili da spreče pretraživač da interpretira određena pravila koja su deo css-a.

/* Jednolinijski komentar */

/*
Komentar može da
se piše i u
više linija
*/

/* Komentar ispod služi da onemogući definisanu stilizaciju */

/*
.card {
    padding: 1rem; 
}
*/
Javascript
Programski jezik - izvršava se u onom trenutku kada web čitač naiđe na njega.

Skripte možemo pisati unutar <head> i <body> taga.

Umetanje scripte na kraj <body> taga omogućava brže loadovanje html stranice. 

Pisanje skripte u eksternom fajlu je praktično jer isti kod možemo kosistiti na različitim web stranicama.

Eksterne skripte ne sadrže <script> tag.

<script src="script.js"></script>
<script>
 // function(s) go here
</script>
Komentari u JavaScriptu

Komentari se koriste da objasne JavaScript kod, kako bi bio čitljiviji programerima. Takođe se koriste da spreče izvršavanje koda.

//Ovo je jednoliniski komentar

/* 
Ovo je
višelinijsi komentar
*/
**[⬆ back to top](#)**
