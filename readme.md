# Verkefni 6

## Lýsing

Nú er eigandi _Bókabúðarinnar_ kátur með útlitið en hefur áhyggjur af viðhaldi á vefnum.

Loka verkefnið (í bili) er að setja upp tól og koma verkefninu fyrir á GitHub fyrir þá vefforritara sem taka við í framtíðinni.

## Útlit

Útlit skal vera það sama og í [verkefni 5](https://github.com/vefforritun/vef1-2020-v5/)

## Tól

Setja skal upp node-sass, browser-sync, stylelint og concurrently til að nýta Sass og geta gert breytingar sem sjást strax í vafra.

### Sass

Skipta skal CSS upp í mismunandi skrár undir `styles/`, sjá viðeigandi komment í hverju og einu skjali.

Í `styles/config.scss` skal geyma allar stillingar fyrir verkefni og nota þær á viðeigandi stöðum.

Nota skal _nesting_ en aðeins upp á eitt level.

```scss
.book {
  .title {
    // ok

    .item {
      // ekki ok, þriðja level
    }
  }
}
```

### Browser sync & concurrently

Þegar skipunin `npm run dev` er keyrð skal verkefnið keyra upp vefþjón með browser-sync, þýða sass skrár og fylgjast með breytingum á HTML og Sass.

### Linting

Setja skal upp stylelint með `stylelint-config-sass-guidelines` og `stylelint-config-standard`.

Þegar skipunin `npm run lint -s` er keyrð skal keyra stylelint með þessum reglum og ættu engar villur að koma fram.

## GitHub

Búa skal til Git repo fyrir verkefni og færa yfir á GitHub. Til að passa upp á samræmi eru skrárnar `.gitignore`, `.gitattributes` og `.editorconfig` gefnar. Sækja skal plugin til að tekið sé tillit til `.editorconfig`, t.d. _EditorConfig for VS Code_.

## Mat

* 40% – CSS flutt yfir í Sass skv forskrift
* 40% – stylelint uppsett og engar villur skv forskrift
* 10% – browser sync og concurrently sett upp og virkar skv forskrift
* 10% – Verkefni skilað á GitHub

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 5. október 2020.

## Skil

Skila skal í Canvas í seinasta lagi fyrir lok dags þriðjudaginn 13. október 2020.

Skilaboð skulu innihalda slóð á GitHub repo fyrir verkefni, og dæmatímakennurum skal hafa verið boðið í repo ([sjá leiðbeiningar](https://docs.github.com/en/free-pro-team@latest/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository)). Notendanöfn þeirra eru:

* `GaddiSunshine`
* `boxandri`
* `StimmiKex`
* `jonnigs`
* `Tobbasn`
* `thth168`

Hver dagur eftir skil dregur verkefni niður um 10%, allt að 30% ef skilað föstudaginn 16. október 2020 en þá lokar fyrir skil.

## Einkunn

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

## Myndir

* [Stanislav Kondratiev](https://unsplash.com/@technobulka)
* [Francesca Tirico](https://unsplash.com/@fra99)
* [Toa Heftiba](https://unsplash.com/@heftiba)
* [Andrew Neel](https://unsplash.com/@andrewtneel)
* [Christine Keller](https://unsplash.com/@christinekeller)

> Útgáfa 0.1
