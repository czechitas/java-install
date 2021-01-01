Krátký popis (pouze pro zkušené):
=================================
Tento popis je určen pro zkušené a popisuje jen slovně, co je potřeba provést pro úspěšnou instalaci.
Doporučujeme tento popis nepoužít a postupovat podle [obrázkového postupu](index.html).



Samotný popis
-------------

Na kurzu budete potřebovat Javu (OpenJDK) a programátorský editor IntelliJ IDEA (Community Edition).
**Nesmíte** si je ale nainstalovat z **oficiální** distribuce.
Místo toho si stáhněte 1 přednastavený archív, který se jen rozbalí do povinného umístění (`C:\Java-Training\`) a vše bude fungovat.
Kdybyste si nainstalovali software z oficiální distribuce, neměli byste je správně nakonfigurované pro školení.

Poznámka: Nic se doopravdy neinstaluje, všechno se jen rozbalí pomocí 7-Zipu. Jde vlastně o *portable distribuci*.

Poznámka: Pokud už máte nainstalované **vlastní** JDK nebo IntelliJ IDEA, nevadí to, ale na kurzu je **používat nebudeme**.
Je opravdu nutné, abyste provedli instalaci dle těchto pokynů. Výukové programy z naší instalace nijak neovlivní
vaše už nainstalované programy. Pokud byste ale instalaci neprovedli, nešly by vám spouštět ukázkové příklady.

1.  Stáhněte si [Java-Training.7z](https://github.com/czechitas/java-install/releases/download/2021-jaro/community/win/Java-Training.7z).

2.  Pokud nemáte nainstalovaný **7-Zip**, nainstalujte si ho.

    Pozor! Nepoužívejte **WinRAR** ani **WinZip**, protože ty nedokáží správně rozbalit archívy `.7z`.
    Obecně doporučujeme **WinRAR** i **WinZip** úplně odinstalovat
    a používat výhradně **7-Zip**.
    Je zdarma, open-source a funguje výborně.

3.  Spusťte 7zFM.exe (7-Zip File Manager) a otevřete v něm `Java-Training.7z`.
    Rozbalte jej do `C:\Java-Training` (Extract to `C:\Java-Training`).

    Kontrola, že jste archív rozbalili do správného umístění:
    Po rozbalení musíte mít na disku `C:` tuto složku
    `C:\Java-Training\Projects\DemoApplication`.

4.  Ze složky `C:\Java-Training\IntelliJ-Community` si přetáhněte
    zástupce `IntelliJ-Community.lnk`
    na plochu a/nebo do nabídky Start (což je složka `C:\Users\VASE_UZIVATELSKE_JMENO\AppData\Roaming\Microsoft\Windows\Start Menu\Programs`).

5.  Spusťte IntelliJ-Community buď pomocí zástupce z minulého kroku
    nebo spuštěním `C:\Java-Training\IntelliJ-Community\startup.bat`.

6.  Otevřete v IntelliJ-Community složku s ukázkovým projektem (Open project)
    `C:\Java-Training\Projects\DemoApplication`.
    Je nutné, abyste byli připojeni na internet.

7.  Po otevření se začne indexovat JDK, což bude pár minut trvat. Průběh je zobrazen na dolní liště editoru.

8.  Až se to dokončí, původně šedý zdrojový text v `Main.java` se přebarví převážně do modrofialova.

    Pokud by zůstal převážně šedý, byl by to problém.
    Nejspíš byste totiž neměli archív vybalen ve správné složce
    `C:\Java-Training\`. Řešení - viz bod 17 v obrázkovém popisu instalace.

9.  Vpravo nahoře v editoru zezelená šipka pro spuštění ukázkového projektu. Tak jej spusťte.
    Projekt musí otevřít okno s nápisem `It works!`.
