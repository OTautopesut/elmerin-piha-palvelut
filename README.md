# Elmerin Piha-apu – nettisivu

Yhden sivun (`index.html`) staattinen sivusto. Ei rakennusvaihetta eikä riippuvuuksia.

## Julkaisu GitHub Pagesilla
1. Lisää kaikki tiedostot repositorion juureen.
2. Repositoriossa: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Valitse branch `main` ja kansio `/ (root)`, paina **Save**.
4. Sivu avautuu hetken kuluttua osoitteessa `https://KÄYTTÄJÄ.github.io/REPO/`.

## Sisällön muokkaaminen (`index.html`)
- **Hinnat ja alennukset:** etsi tiedostosta `/* ===== Muokattavat tiedot ===== */`.
  - `FENCE` = pensasleikkuun hinta (perushinta + hinta/m). Nyt 30 m ≈ 150 €, 100 m ≈ 400 €.
  - `LAWN` = nurmikonleikkuun hinta-arviot kokoluokittain (`to` = yläraja m², `a`–`b` = haarukka €).
  - `DISCOUNTS` = alennukset. Aseta `on:false`, kun kampanja päättyy. Ponnahdusikkunan ensikertalaisalennus käyttää alennusta, jonka `id` on `uusi`.
- **Asiakaspalautteet:** `REVIEWS`-lista samassa kohdassa.
- **Ennen/jälkeen-kuvat:** korvaa tiedostot kansiossa `images/` samannimisillä, 4:3-kuvasuhteen kuvilla (esim. 640 × 480 px).
- **4H-stipendin todiste:** `images/4h-stipendi-julkaisu.jpg`.
- **Ajanvaraus (Vello):** osio `<section id="varaa">`. Liitä Vellon upotuskoodi elementtiin `#vello-varaus` ja poista paikkamerkki `vello-ph`.
- **Ponnahdusikkuna:** `id="pop"` sivun alussa. Se aukeaa joka kerta sivun avautuessa. Poista rivi `setTimeout(openPop,500);`, jos haluat ottaa sen pois.
- **Logo:** 4H-logo on vielä paikkamerkki ("4H"-merkki) sivun ylävalikossa.
