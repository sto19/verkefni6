# Verkefni 6

## Lýsing

Nú er eigandi _Bókabúðarinnar_ kátur með útlitið en hefur áhyggjur af viðhaldi á vefnum.

Loka verkefnið (í bili) er að setja upp tól og koma verkefninu fyrir á GitHub fyrir þá vefforritara sem taka við í framtíðinni.

## Útlit

Útlit skal vera það sama og í [verkefni 5](https://github.com/vefforritun/vef1-2020-v5/)

## Tól

Til þess að geta notað þessi tól þarf að [setja upp Node.js, sækið „Recommended For Most Users“](https://nodejs.org/en/). Eftir að þið hafið keyrt uppsetningar forrit getið þið opnað Command prompt/terminal/skel og keyrt:

```bash
> node -v
v12.18.4 # eða sú útgáfa sem þið sóttuð
> npm -v
6.14.8 # eða álíka
```

Ef þið fáið villu eftir að hafa keyrt annað hvort og uppsetning á Node.js gekk sem skildi skulið þið prófa að endurræsa tölvu. Ef ennþá ekki að virka, leitið hjálpar hjá Óla.

Setja skal upp node-sass, browser-sync, stylelint og concurrently til að nýta Sass og geta gert breytingar sem sjást strax í vafra.

Fyrst þarf að búa til `package.json` með því að keyra `npm init` í verkefnamöppu.

Síðan þarf að sækja hvert tól með `npm install <nafn á tóli>`.

[Sjá nánar í efni fyrirlesturs](https://github.com/vefforritun/vef1-2020/blob/master/fyrirlestrar/06/06.2.npm.md#t%C3%B3l-%C3%AD-verkefnum).

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

[Sjá dæmi í fyrirlestri](https://github.com/vefforritun/vef1-2020/tree/master/fyrirlestrar/06/daemi/node-sass).

### Browser sync & concurrently

Þegar skipunin `npm run dev` er keyrð skal verkefnið keyra upp vefþjón með browser-sync, þýða sass skrár og fylgjast með breytingum á HTML og Sass.

[Sjá dæmi í fyrirlestri](https://github.com/vefforritun/vef1-2020/tree/master/fyrirlestrar/06/daemi/node-sass-browser-sync).

### Linting

Setja skal upp stylelint með `stylelint-config-sass-guidelines` og `stylelint-config-standard`.

Þegar skipunin `npm run lint -s` er keyrð skal keyra stylelint með þessum reglum og ættu engar villur að koma fram.

[Sjá dæmi í fyrirlestri](https://github.com/vefforritun/vef1-2020/tree/master/fyrirlestrar/06/daemi/stylelint).

## GitHub

Búa skal til Git repo fyrir verkefni og færa yfir á GitHub. Til að passa upp á samræmi eru skrárnar `.gitignore`, `.gitattributes` og `.editorconfig` gefnar. Sækja skal plugin til að tekið sé tillit til `.editorconfig`, t.d. _EditorConfig for VS Code_.

Ef þið viljið nota _þetta_ repo sem grunn þá gerið þið eftirfarandi (þurfið að vera búin að setja upp GitHub):

```bash
# Farið í Command prompt/terminal/skel inn í möppu þar sem verkefnin ykkar eru á ykkar tölvu
> cd vefforritun

# "git clone" sækir repo og býr til á ykkar tölvu með öllu
> git clone https://github.com/vefforritun/vef1-2020-v6.git

# Farið inn í möppuna sem git cloneaði
> cd vef1-2020-v6

# Þar sem þetta repo er clone frá repo sem ég (Óli) á, þá þurfið þið að slíta þau tengsl og tengja við ykkar repo
> git remote remove origin

# Búið til repo undir ykkar account á slóðinni https://github.com/<NOTENDANAFN>?tab=repositories og smellið á "New"
# Takið síðan slóðina á repo og bætið við repo á tölvunni ykkar
> git remote add origin https://github.com/<NOTENDANAFN>/vef1-2020-v6.git

# Sendið það sem þið sóttuð héðan (á Óla repo) á ykkar repo
> git push origin master

# Vinnið verkefnið, breytið skrám etc og bætið svo öllum við "staged"
> git add .

# Committið í ykkar repo
> git commit -m "Vinna í verkefni 6"

# Sendið á repoið ykkar á GitHub
> git push origin master
```

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

> Útgáfa 0.2
