# Slova, která se často používají v CSS classech

## Obrázky

`image`, `img`, `picture`, `pic` — obrázek

`icon` — ikonka

`logo` — logo

`userpic`, `avatar` — avatar, malý obrázek uživatele (fotka..)

## Text

`title`, `subject`, `heading`, `headline`, `caption` — nadpis

`subtitle` — podnadpis

`lead`, `tagline` — perex

`text` — textový obsah

`desc` — popis, textový obsah

`excerpt` — úryvek textu, obvykle se používá před odkazem "Číst dál..."

`link` — odkaz

## Seznamy

`list`, `items` — seznam

`item` — položka v seznamu

## Rozložení

`page` — základní prvek stránky

`wrapper` — tzv. obálka stránky

`container`, `box` — kontejner

`grid` — rozložení (stránky nebo prvku) v podobě sloupců (obvykle obsahuje `row` - řádek a `col` - sloupec)

`row` — řádek v gridu

`col`, `column` — sloupec v gridu

`section` — tématická část obsahu (jedna z několika)

`inner` — vnitřní prvek

`header` — hlavička (stránky nebo prvku)

`footer` — patička (stránky nebo prvku)

`body` — hlavní část (stránky nebo prvku)

`content` — obsah prvku

`sidebar` — postranní sloupec (stránky nebo prvku)

`aside` — blok s doplňujícími informacemi

`widget` — samostatný prvek například v postranním sloupci

## Prvky ovládání

`button`, `btn` —  tlačítko, příklad: pro odeslání formuláře

`control` — prvek ovládání, příklad: šipky "Další / Předchozí" v galerii

`dropdown` — vyjíždějící seznam

## Výrazy pro media

`phone`, `mobile` — pro mobilní zařízení

`tablet` — pro tablety

`desktop` — pro stolní počítače

## Ostatní

`user`, `author` — uživatel, autor článku či komentáře

`search` — vyhledávání

`socials` — blok s ikonkami soc. sítí

`features` — seznam přednostních vlastností daného zboží nebo služby

`active`, `current` — aktivní prvek, příklad: aktuální položka v menu

`meta` — blok s doplňující informací, příklad: blok se štítky (tagy) nebo datumem napsání článku

`slider`, `carousel` — posuvník, interaktivní prvek s měnícím se obsahem

`modal` — modální (dialogové) okno

`popup` — vyskakující okno


## Příklady použití

### Obyčejný seznam

```html
<ul class="list">
  <li class="item">Notebooky</li>
  <li class="item">PC a komponenty</li>
  <li class="item">Mobily a tablety</li>
</ul>
```

### Obrázek uživatele (avatar / userpic)

```html
<div class="user">
  <img class="user__img" src="userpic.png" alt="Pavel Novák">
  <a class="user__link" href="#">Pavel Novák</a>
</div>
```

### Galerie

```html
<div class="gallery">
  <ul class="gallery__list">
    <li class="gallery__item">
      <img class="gallery__img" src="phones.jpg" alt="Novinky na trhu mobilních telefonů">
    </li>
    <li class="gallery__item">
      <img class="gallery__img" src="tablets.jpg" alt="Novinky na trhu tabletů">
    </li>
  </ul>
</div>
```

### Navigace

```html
<nav class="nav">
  <a class="nav__link nav__link--active">Úvodní stránka</a>
  <a class="nav__link" href="#">Hračky</a>
  <a class="nav__link" href="#">Parfémy</a>
  <a class="nav__link" href="#">Drogerie</a>
  <a class="nav__link" href="#">Sport</a>
</nav>
```

```html
<nav class="nav">
  <ul class="nav__list">
    <li class="nav__item nav__item--current">
      <a class="nav__link">Úvod</a>
    </li>
    <li class="nav__item">
      <a class="nav__link" href="#">Novinky</a>
    </li>
    <li class="nav__item">
      <a class="nav__link" href="#">Fotogalerie</a>
    </li>
    <li class="nav__item">
      <a class="nav__link" href="#">Kontakt</a>
    </li>
  </ul>
</nav>
```

### Widget v postranním panelu

```html
<div class="widget">
  <h4 class="widget__tilte">Winehouse má 32% nárůst v online platbách</h4>

  <div class="widget__content">
    <p>O výhodách online plateb není třeba dlouze uvažovat - 
    na jedné straně jsou to zákazníci, kteří mohou za zboží 
    zaplatit okamžitě a vyhnout se ...</p>

    <a class="widget__link" href="#">Číst dál...</a>
  </div>
</div>
```

### Blok novinek

```html
<div class="news">
    <h3 class="news__title">Čerstvé zprávy</h3>

    <ul class="news__list">
        <!-- ke classu prvku přidáváme nový class bloku
             pro vytvoření nového oboru názvů -->
        <li class="news__item item-news">
            <h4 class="item-news__title">Václav Bělohradský chce do Senátu za ČSSD a zelené</h4>
            <div class="item-news__text">
              <p>Filozof Václav Bělohradský (72) bude v říjnových volbách do Senátu v Praze 6 
              společným kandidátem ČSSD a Strany zelených. Potvrdil...</p>

              <a href="#" class="item-news__link">Pokračovat ve čtení</a>
            </div>
        </li>

        <li class="news__item item-news">
            <h4 class="item-news__title">Airbus podepsal dohodu o stavbě závodu na vrtulníky v Číně</h4>
            <div class="item-news__text">
              <p>Airbus Helicopters, který je největším světovým dodavatelem komerčních vrtulníků, 
              dokončil dohodu o prodeji 100 helikoptér H135 čínskému...</p>

              <a href="#" class="item-news__link">Pokračovat ve čtení</a>
            </div>
        </li>
    </ul>
</div>
```

### Článek nebo příspěvek v blogu (obyčejná varianta)

```html
<article class="article">
  <h3 class="article__title">Je Osvětim symbolem holokaustu?</h3>
  <time class="article__datetime">25. 04. 2016 8:54:28</time>

  <div class="article__author author-article">
    <img class="author-article__img" src="userpic.png" alt="Lenka Hoffmannová">
    <a class="author-article__link" href="#">Lenka Hoffmannová</a>
    <div class="author-article__desc">hoffmannova.blog.idnes.cz</div>
  </div>

  <div class="article__content">
    Hitler ve 30. letech usiloval o spojenectví s Polskem, které mu mělo pomoci 
    dobýt Sovětský svaz. V té době Polsko usilovalo o vystěhování svých asi 3 milionů 
    Židů do Palestiny pod správou Velké Británie. Představitelé Polska spolupracovali 
    s polskými Židy a žádali Velkou Británii o zvýšení kvót přistěhovalectví do Palestiny.
  </div>
</article>
```

### Článek nebo příspěvek v blogu (složitá varianta)

```html
<article class="entry">
  <header class="entry__header">
    <h3 class="entry__title title-entry">
      <a class="title-entry__link" href="#">Moudrý děda všeuměl</a>
    </h3>

    <time class="title-entry__datetime">13. 06. 2016 13:24:20</time>
  </header>

  <div class="entry__author author-entry">
    <img class="author-entry__img" src="userpic.png" alt="Tomáš Flaška">

    <a class="author-entry__link" href="#">Tomáš Flaška</a>
  </div>

  <div class="entry__content">
    "Všeci tu kradú", praví on. Jeden vtip dodává: "jenom já dotujem". 
    Ale ministr financí je v našich zemích přeci jen rarita. Rozumí 
    všemu. Teda aspoň se tak tváří. Chápu že strážce státní kasy musí 
    mít názor na financování sociálních dávek, hasičů, školství a dalších 
    položek. Proto musí vyjednávat se všemi zúčastněnými.
  </div>

  <div class="entry__tags tags-entry">
    <h4 class="tags-entry__tilte">Tagy</h4>

    <ul class="tags-entry__list">
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">dotace</a>
      </li>
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">blog</a>
      </li>
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">názor</a>
      </li>
    </ul>
  </div>

  <div class="entry__actions actions-entry">
    <ul class="actions-entry__list">
      <li class="actions-entry__item actions-entry__item--read">
        <a class="actions-entry__link" href="#">238 komentářů</a>
      </li>
      <li class="actions-entry__item actions-entry__item--write">
        <a class="actions-entry__link" href="#">Komentovat</a>
      </li>
      <li class="actions-entry__item actions-entry__item--share">
        <a class="actions-entry__link" href="#">Sdílet</a>
      </li>
    </ul>
  </div>
</article>
```

Zdroj: github.com/yoksel/common-words/
