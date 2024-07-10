---
title: "Kezdeti lépések"
---

A fő homebrew alkalmazás, amit ez az útmutató telepít a **TW**i**L**ight Menu++, ami egy feljavítása/cseréje a Nintendo DSi Menu-nek, és ami lehetővé teszi más homebrew-ok, kereskedelmi DS játékok, más régebbi rendszerek emulátorainak és egyebeknek a futtatását.

A letöltésével fogunk kezdeni, illetve más homebrew eszköz(ök) letöltésével, hogy előkészüljünk az exploit lépéseire.

## Követelmények

- Egy mód arra, hogy a letöltött fájlokat az SD kártyádra másold
- Egy alkalmazás, ami ki tud tömöríteni csomagolt állományokat, mint például a [7-Zip](https://www.7-zip.org/) (Windows), a [The Unarchiver](https://apps.apple.com/us/app/the-unarchiver/id425424353) (macOS) vagy a [ZArchiver](https://play.google.com/store/apps/details?id=ru.zdevs.zarchiver) (Chromebook)
    - Azt tanácsoljuk, hogy ne használj WinRAR-t, mert ismert arról, hogy elront dolgokat
    - Ha Windows 11-et használsz javasoljuk, hogy ne használd a beépített csomagolót (Windows Explorer), mert hibát okoz azzal, hogy azt mondja a fájlnév túl hosszú vagy nem érvényes

## I. rész - Előkészületek

::: warning

Biztosítsd, hogy az SD kártyád [megfelelően formázott](sd-card-setup.html) legyen.

:::

1. Tedd be az SD kártyád a PC számítógépedbe
1. Töltsd le a [TWiLight Menu++](https://github.com/DS-Homebrew/TWiLightMenu/releases/latest/download/TWiLightMenu-DSi.7z) legfrissebb kiadását
    - Ha nem tölt le, nyisd meg a [release oldalt](https://github.com/DS-Homebrew/TWiLightMenu/releases/latest), és töltsd le a `TWiLightMenu-DSi.7z` fájlt
1. Töltsd le a [dumpTool](https://github.com/zoogie/dumpTool/releases/latest/download/dumpTool.nds) legfrissebb kiadását
1. Nyisd meg a `TWiLightMenu-DSi.7z` fájlt
    - Ha Windows-t használ, biztosítsd, hogy a 7-Zip telepítve van, majd kövesd a következő lépéseket:
        1. Kattints jobb gombbal a `TWiLightMenu-DSi.7z` fájlra
        1. Ha Windows 11-et használsz, kattints a `Több lehetőség megjelenítése` opcióra
        1. Menj a `7-zip` felé
        1. Kattints az `Archívum megnyitása` opcióra
1. Másold ki az `_nds` mappát `TWiLightMenu-DSi.7z` fájlból az SD kártyád gyökerébe
1. Másold ki a `BOOT.NDS` fájlt `TWiLightMenu-DSi.7z` fájlból az SD kártyád gyökerébe
1. Zárd be a `TWiLightMenu-DSi.7z` fájlt
1. Másold a `dumpTool.nds` fájlt az SD kártyád gyökerébe

::: tip

Nem tudod, mi az SD "gyökér"? [Tekintsd meg ezt a képet](/assets/images/sdroot/en_US.png)

:::


## II. rész - Az exploit kiválasztása

Innentől kezdve három lehetőséged van, egy kis különbséggel, hogy melyik mivel jár.


### Az Unlaunch telepítése Memory Pit-tel

A Memory Pit egy exploit ami a DSi Camera-t használja és kompatibilis minden firmware verzióval. Opcionálisan, ez az exploit használható az Unlaunch telepítésére, ami egy bootcode exploit és teljes hozzáférést ad a konzolhoz bootoláskor.

A Memory Pit valamennyire korlátozott homebrew kompatibilitással rendelkezik, ajánlott, hogy telepítsd az Unlaunch-öt, a Memory Pit önálló használata helyett. Ez a legkönnyebb metódusa az Unlaunch telepítésének, így ez az ajánlott módja. Azonban van egy nagyon kicsi kockázata a konzolod **brickelésének** az Unlaunch telepítésekor, így ha ez számít, akkor válassz másik metódust alább.

::: tip

Folytatás [Az Exploit indítása](launching-the-exploit.html) útmutatóval

:::


### stylehax

A stylehax egy olyan exploit, ami a DSi Browser alkalmazást használja és alternatívaként használható a Memory Pit helyett az Unlaunch telepítéséhez (részletezve fentebb) ha a DSi-d kamerája hibás.

Az Unlaunch mentes élményhez ez az exploit ajánlott, mert a Memory Pit problémát okoz néhány játéknál vagy homebrew-nál.

::: tip

Folytatás [Az Exploit indítása (stylehax)](launching-the-browser-exploit.html) útmutatóval

:::


### Flipnote Lenny

A Flipnote Lenny egy exploit ami a Flipnote Studio alkalmazást használja.

Ha van Flipnote Studio-d és nem tervezed az Unlaunch (fentebb bemutatva) telepítését, akkor ez az exploit ajánlott, ugyanazon okból, mint a stylehax.

Mindig teleptheted az Unlaunch-öt később, ha úgy döntenél, hogy szeretnéd.

::: tip

Folytatás [Az Exploit indítása (Flipnote Lenny)](launching-the-flipnote-exploit.html) útmutatóval

:::

Részletesebb előnyök és hátrányok összehasonltásért az elérhető exploitokról tekints meg a [Melyik a legjobb exploit?](faq.html#which-is-the-best-exploit) GYIK-et.
