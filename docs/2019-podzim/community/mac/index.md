Instalační pokyny pro macOS
===========================

Tyto pokyny jsou **výhradně pro macOS**.
Instalaci pro Windows najdete [zde](../win/).

Linux **není** podporován. Pokud byste potřebovali instalaci pro Linux,
byl by to problém, se kterým je nutno se ozvat lektorovi.

Pokud už jste instalaci na Java kurz někdy prováděly,
nejspíš máte v `/Users/VASE_UZIVATELSKE_JMENO/Java-Training/Projects`
projekty z minula. Doporučujeme vám je zazálohovat zkopírováním například do `Dokumenty` ve vašem uživatelském profilu
a po dokončení instalace je přesunout zpět do složky
`/Users/VASE_UZIVATELSKE_JMENO/Java-Training/Projects`.

Pokud by kterýkoliv program,
který si nainstalujete v rámci této instalace,
nabízel update, prosím odmítněte to.
Programy jsou přesně vybrané, aby spolu fungovaly, a jsou předkonfigurované.
Updatované verze by ztratily konfiguraci a materiály z kurzu by nešly spustit.


<a id="detailni">Detailní postup:</a>
-------------------------------------
Zkušené uživatelky mohou přeskočit ke krátkému [popisu](#kratky),
ale doporučujeme to nedělat a držet se tohoto [video návodu](https://youtu.be/PmgJeo8iiK0).

Stáhnout archív s instalací [Java-Training.zip](https://1drv.ms/u/s!AijQjx8qkEJYea_n4JwaDrBA2y0?e=u2bsR7).

<a id="kratky">Krátký popis (pouze pro zkušené):</a>
----------------------------------------------------
Tento popis je jen pro experty a dokumentuje slovně, co se provádí během instalace.
Doporučujeme tento popis nepoužít a postupovat podle video návodu [výše](#detailni).

Na kurzu budete potřebovat Javu (JDK) a programátorský editor IntelliJ IDEA (Community Edition).
**Neinstalujte** si je **ručně**, stáhněte si předpřiravený archív.

1.  Stáhněte si [Java-Training.zip](https://1drv.ms/u/s!AijQjx8qkEJYea_n4JwaDrBA2y0?e=u2bsR7).
   
2.  Pokud už jste někdy instalaci na Java kurzy prováděli, zazálohujte si složku
    `/Users/VASE_UZIVATELSKE_JMENO/Java-Training/Projects` (například do Documents),
    abyste o starší projekty nepřisli.

2.  Vybalte obsah `Java-Training.zip` do `/Users/VASE_UZIVATELSKE_JMENO/Java-Training`.

    Pozor! Pokud už jste někdy instalaci na Java kurz prováděli,
    nenahrazujte celou složku Java-Training novou verzí.
    (**Nedělejte Replace**.)
    Složky nechejte sloučit. (Původní soubory přepsat novými.)
    **Finder** to umožní při podržení klávesy Option (Alt) při přetahování.
    Nicméně rozhodně doporučujeme použití nějakého pořádného programu
    typu **Commander One** nebo **Midnight Commander**.

    Pro kontrolu správného umístění zkontrolujte, že máte přítomnu tuto složku:
    `/Users/VASE_UZIVATELSKE_JMENO/Java-Training/Projects/DemoApplication`.
   
3.  Připojte instalační medium `ideaIC-2018.3.5.1.dmg`
    (které najdete v `/Users/VASE_UZIVATELSKE_JMENO/Java-Training/ideaIC-2018.3.5.1.dmg`)
    a nainstalujte z něj aplikaci `IntelliJ IDEA CE - Java-Training`.
   
4.  Spusťte tuto aplikaci, aby se zkontroloval její digitální podpis a ihned ji zavřete.
    Před skutečným používáním je totiž potřeba jí nastavit nové umístění konfiguračních souborů.
   
5.  Ve složce `/Applications` vstupte do složky
    `IntelliJ IDEA CE - Java-Training.app` (Show package contents)
   
6.  <a id="config">Přidejte</a> do
    `/Applications/IntelliJ IDEA CE - Java-Training.app/Contents/bin/idea.properties`
    tyto řádky:
    ~~~~
    idea.config.path=~/Java-Training/User-Config/IntelliJ-Community/config
    idea.plugins.path=~/Java-Training/User-Config/IntelliJ-Community/config/plugins
    idea.system.path=~/Java-Training/User-Config/IntelliJ-Community/system
    idea.log.path=~/Java-Training/User-Config/IntelliJ-Community/system/log
    ~~~~
    Změníte tím složku s konfiguračními soubory pro IntelliJ IDEA.
    Je nutné nastavit právě tyto konfigurační soubory,
    jinak by nešly otevírat materiály z kurzu.

7.  Dále je nutné změnit zástupné cesty uvnitř konfiguračních souborů IntelliJ IDEA.
    Najdete je v `/Users/VASE_UZIVATELSKE_JMENO/Java-Training/User-Config/IntelliJ-Community/config/options/path.macros.xml`

    ~~~~
    JAVATRAINING           /Users/VASE_UZIVATELSKE_JMENO/Java-Training
    ~~~~
    Změňte zástupný text `VASE_UZIVATELSKE_JMENO` na vaše skutečné jméno složky.
    Toto umístění je specifické pro váš počítač, proto je nutné to udělat ručně.
     
8.  Otevřete ukázkový projekt v
    `/Users/VASE_UZIVATELSKE_JMENO/Java-Training/Projects/DemoApplication`.

9.  Po otevření se začne indexovat JDK, což bude pár minut trvat.

10. Až se to dokončí, zdrojový text v `Main.java` musí být převážně modrofialový.

    Pokud by byl naopak převážně černý, byl by to problém.
    Nejspíš byste totiž nenastavili správně cesty ke konfiguračním souborům IntelliJ IDEA
    (viz [tento bod](#config)).

11. Vpravo nahoře zezelená šipka pro spuštění ukázkového projektu, tak jej spusťte.
