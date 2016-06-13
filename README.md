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
    <p>O výhodách online plateb není třeba dlouze uvažovat - na jedné straně jsou to zákazníci, kteří mohou za zboží zaplatit okamžitě a vyhnout se tak nepříjemným dobírkám či zdlouhavé platbě bankovním převodem, na druhé straně jsou to obchodníci, kterým neleží ...</p>

    <a class="widget__link" href="#">Číst dál...</a>
  </div>
</div>
```

### Blok novinek

```html
<div class="news">
    <h3 class="news__title">Čerstvé zprávy</h3>

    <ul class="news__list">
        <!-- к классу элемента добавляем класс блока,
             чтобы создать новое пространство имён -->
        <li class="news__item item-news">
            <h4 class="item-news__title">Соревнования среди воблы по конькобежному спорту</h4>
            <div class="item-news__text">
              <p>Победила команда килек из Петрозаводска</p>

              <a href="#" class="item-news__link">Читать дальше</a>
            </div>
        </li>

        <li class="news__item item-news">
            <h4 class="item-news__title">Учёные уточнили роль напильника в уходе за ногтями</h4>
            <div class="item-news__text">
              <p>Британские учёные высоко оценили вклад
                напильника в отращивание полутораметровых ногтей.</p>

              <a href="#" class="item-news__link">Не читать дальше</a>
            </div>
        </li>
    </ul>
</div>
```

### Статья или пост в блоге (простой вариант)

```html
<article class="article">
  <h3 class="article__title">Нащупываем чакры у пучка петрушки</h3>
  <time class="article__datetime">32 мая, 10:87</time>

  <div class="article__author author-article">
    <img class="author-article__img" src="userpic.png" alt="Клешня Андреевна">
    <a class="author-article__link" href="#">Клешня Андреевна Долгорукая</a>
    <div class="author-article__desc">Наш эксперт по чакрам</div>
  </div>

  <div class="article__content">
    Сходите на рынок и купите у старушек пучок петрушки грамм на 100.
    Как следует переберите, очистите от жуков и гусениц. Жуков отдайте поиграться
    коту, гусениц поселите в горшок с кактусами, пусть одна будет Джоном,
    вторая Билли, а у вас в горшке теперь будет Дикий Запад. Вернитесь
    к пучку петрушки. Ласково взгляните на него и как следует почешите
    за ухом, можно себе или коту. Перевяжите атласной ленточкой,
    непременно завяжите бант. Поздравляем! Теперь у вас есть полностью
    одомашненный пучок петрушки, который будет весело бегать за вами
    по пятам и проращивать свои семена в ваших тапках.
  </div>
</article>
```

### Статья или пост в блоге (сложный вариант)

```html
<article class="entry">
  <header class="entry__header">
    <h3 class="entry__title title-entry">
      <a class="title-entry__link" href="#">Резиновые уточки как способ самопознания</a>
    </h3>

    <time class="title-entry__datetime">32 мая, 10:87</time>
  </header>

  <div class="entry__author author-entry">
    <img class="author-entry__img" src="userpic.png" alt="Василиса Сергеевич">

    <a class="author-entry__link" href="#">Василиса Сергеевич</a>
  </div>

  <div class="entry__content">
    Достаньте с чердака коробку с полусотней резиновых уточек,
    оставшихся после празднования нового года. Из уточек
    и горящих свечей выложите пентаграмму на полу комнаты.
    Сядьте посередине в позу лотоса, в каждую руку возьмите
    по немецко-бразильскому словарю, прокашляйтесь, наберите
    полную грудь воздуха и громко и уверенно,
    с полной самоотдачей скажите "Кря!"
  </div>

  <div class="entry__tags tags-entry">
    <h4 class="tags-entry__tilte">Метки</h4>

    <ul class="tags-entry__list">
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">хоровод своими руками</a>
      </li>
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">фарфоровые тапки</a>
      </li>
      <li class="tags-entry__item">
        <a class="tags-entry__link" href="#">гуталин в кулинарии</a>
      </li>
    </ul>
  </div>

  <div class="entry__actions actions-entry">
    <ul class="actions-entry__list">
      <li class="actions-entry__item actions-entry__item--read">
        <a class="actions-entry__link" href="#">238 ответов</a>
      </li>
      <li class="actions-entry__item actions-entry__item--write">
        <a class="actions-entry__link" href="#">Написать в спортлото</a>
      </li>
      <li class="actions-entry__item actions-entry__item--share">
        <a class="actions-entry__link" href="#">Поделиться</a>
      </li>
    </ul>
  </div>
</article>
```

Zdroj: github.com/yoksel/common-words/
