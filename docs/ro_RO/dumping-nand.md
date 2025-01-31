# Copiere NAND

Această pagină este pentru creerea unei copii NAND, ce este o copie a datelor de pe stocarea interna a Nintendo DSi. Ea poate fi folosit pentru a seta hiyaCFW, precum și no$gba și melonDS pentru emularea DSi.

::: tip

Make sure the SD card has at least 250MB of free space, or else you'll run into an error message in dumpTool.

:::

::: tip

It is highly recommended that you do this. A NAND backup can be used as a restore point in the future, in case of a brick.

:::

## Secțiunea I - Setarea cardului SD

::: tip

If you have already downloaded dumpTool from another section of this guide, you can skip this section.

:::

1. Download the latest release of [dumpTool](https://github.com/zoogie/dumpTool/releases/latest/download/dumpTool.nds)
2. Place `dumpTool.nds` anywhere on your SD card

## Secțiunea II - Creerea unei copii NAND

1. Launch `dumpTool` through TWiLight Menu++
2. Apasă butonul <kbd class="face">A</kbd> pe Nintendo DSi pentru a începe creerea unei copii NAND
   - O copiere NAND durează de obicei 7 minute
3. Când copierea NAND este completă, apasă butonul <kbd>START</kbd> pe Nintendo DSi pentru a ieși din dumpTool
4. Oprește-ți consola și inserează cardul SD înapoi în dispozitiv
5. Păstrează această copie undeva în siguranță, unde nu-l poți pierde
   - Dacă este posibil, creează mai multe copii pe mai multe dispozitive
   - Odată ce ai salvat-o în alt loc, poți să o ștergi de pe cardul SD

::: warning

The SHA1 hash of the `nand.bin` will not match the hash stored in `nand.bin.sha1`. This is because dumpTool adds additional data known as a no$gba footer to the `nand.bin` file after the SHA1 hash is calculated. You can use the [hiyaCFW Helper](https://github.com/mondul/HiyaCFW-Helper/releases) to create a copy without the footer.

:::

::: tip

Continue to [Installing Unlaunch](installing-unlaunch.html) (Optional)

:::
