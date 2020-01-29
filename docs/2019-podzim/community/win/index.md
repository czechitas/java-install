Instalační pokyny pro Windows
=============================

Tyto pokyny jsou **výhradně pro Windows**.
Instalaci pro macOS najdete [zde](../mac/).

Linux **není** podporován. Pokud byste potřebovali instalaci pro Linux,
byl by to problém, se kterým je nutno se ozvat lektorovi.

Tyto instrukce následujte i pokud už máte nějaké programy v
`C:\Java-Training` z minula. Žádný strach, původní projekty si tím nepřepíšete.
Ty máte v `C:\Java-Training\Projects` a tato složka se nemaže.
Složku `C:\Java-Training\Projects` si nicméně před touto instalací
můžete zazálohovat do jiné složky (např. `Dokumenty` ve svém uživatelském profilu).
Soubory v `C:\Java-Training` buď zůstanou nedotčeny
nebo budou přepsány novější verzí programů, což je v pořádku.

Pokud by kterýkoliv program,
který si stáhnete v archívu `Java-Training.7z`,
nabízel update, prosím, odmítněte to.
Programy jsou přesně vybrané, aby spolu fungovaly, a jsou předkonfigurované.
Updatované verze by ztratily konfiguraci a materiály z kurzu by nešly spustit.

Poznámka: **7-Zip** není součástí `Java-Training.7z` a můžete ho tedy updatovat dle libovůle.


<a id="detailni">Detailní postup:</a>
-------------------------------------

Zkušené uživatelky mohou přeskočit ke krátkému [popisu](#kratky),
ale doporučujeme to nedělat a držet se tohoto obrázkového návodu.

1.  Stáhněte si archív s instalací
    [Java-Training.7z](https://github.com/czechitas/java-install/releases/download/2019-podzim/community/win/Java-Training.7z)

2.  Nainstalujte si **7-Zip**.

    To platí i v případě, že už máte **WinRAR** nebo **WinZip**.
    Především **WinRAR** nedokáže soubory `.7z` správně rozbalit.
    Obecně doporučujeme **WinRAR** nebo **WinZip** úplně odinstalovat
    a používat výhradně **7-Zip**.
    Je zdarma, open-source a funguje výborně.

	![](img/img01.png)

3.  Stažený soubor - instalátor 7-Zipu - spusťte.

4.  ![](img/img02.png)

5.  ![](img/img03.png)

6.  ![](img/img04.png)

7. Pokud se Windows ptá, zda chcete aplikaci povolit provádět změny, dialog odsouhlaste. (Yes/Ano)

    ![](img/img05.png)

8.  ![](img/img06.png)

9. 	![](img/img07.png)

10. Spusťte **7-Zip File Manager**. Spouštění se může lišit v závislosti
    na verzi Windows.

    ![](img/img08.png)

11.	Otevřete nastavení programu.

    ![](img/img09.png)

12.	Zkontrolujte, zda máte 7-Zip asociovaný minimálně se soubory .7z a .zip. Vřele doporučujeme používat ho na všechny archívy. (Všechny typy souborů označíte/odznačíte v dialogu tlačítkem plus +)

    ![](img/img10.png)

13.	Ještě pár nastavení pro přehlednější chování 7-Zipu. Na konci potvrďte změny tlačítkem OK. Všechna otevřená okna potom zavřete.

    ![](img/img11.png)

### Samotný postup instalace

14. Najděte na počítači uložený soubor `Java-Training.7z` (pravděpodobně je ve složce
    `Downloads`), klikněte pravým tlačítkem
    a vyberte 7-Zip -> Open archive

15. ![](img/img12.png)

16. ![](img/img13.png)

17. ![](img/img14.png)

18. Tlačítkem "Extract" spusťte rozbalovací dialog.

    ![](img/img15.png)

19. Archív vybalte do cesty `C:\Java-Training`. Tato cesta je **povinná**.
    Je nutné mít na disku `C:` alespoň 3 GB volného místa.
    Pokud byste neměly na disku dostatek místa, je nutné něco smazat.
    Dobrý kandidát jsou velké soubory ze složky `Downloads`.

    ![](img/img16.png)

20. ![](img/img17.png)

    Po rozbalení zavřete 7-Zip.

21. Pro kontrolu, že jste archív rozbalily do správného umístění:
    Po rozbalení musíte mít na disku `C:` tuto složku
    `C:\Java-Training\Projects\DemoApplication`.

    ![](img/img18.png)

21. Ve složce IntelliJ-Community najdete zástupce pro spouštění editoru IntelliJ IDEA. Doporučujeme zkopírovat ho na plochu.

    ![](img/img19.png)

22. ![](img/img20.png)

23. ![](img/img21.png)

24. ![](img/img22.png)

25. Spusťte IntelliJ IDEA. (Buďte trpěliví - je normální, že počítač nějakou dobu "nic nedělá", než naskočí úvodní obrazovka.)
    Od tohoto bodu je nutné, abyste byli **připojení na internet**.

    ![](img/img23.png)


26. ![](img/img24.png)

27. Otevřete ukázkový projekt `C:\Java-Training\Projects\DemoApplication`.

    ![](img/img25.png)

28. Pozor, v otevíracím dialogu rozklikávejte levé šipečky
    **pouze jedním kliknutím**
    a vstupujte tak do podsložek.
    **Neklikejte** na jméno složky **2x**.
    IntelliJ IDEA to čas od času může špatně pochopit a pokusit se složku,
    ve které není javový projekt, importovat.

    ![](img/img26.png)

29. ![](img/img27.png)

30. Počkejte, než IntelliJ IDEA po prvním spuštění naindexuje Javu.
    Může to trvat několik minut.

    ![](img/img28.png)

31. V otevřeném projektu byste měli vidět soubor Main.java. Pokud ne, rozklikněte složky v projektu a dvojklikem na jméno souboru ho otevřete v editoru.

    ![](img/img29.png)

32. Správně nastavená IntelliJ IDEA obarvuje zdrojový text v Main.java
    do modrofialova stejně, jak je vidět na obrázku:

    ![](img/img30.png)

33. Pokud máte v tenhle moment problém s internetovým připojením, může se přihodit, že se nestáhnou všechna potřebná data. V takovém případě budete mít části textu červené - jako na obrázku níže.

    ![](img/img31.png)

34. Náprava: otevřete záložku "Maven" na pravé straně obrazovky.

    ![](img/img32.png)

35. Stiskněte tlačítko se šipkami "Reimport All Maven Projects" a nechte počítač pracovat.

    ![](img/img33.png)

36. Nepomohlo a pořád jsou některé části textu červené? Rozklikněte v záložce Mavenu složku "Lifecycle", označte "clean" a spusťte akci zelenou šipkou. POZOR, nespleťte si tuhle šipku se stejně vyhlížející šipkou o něco výše vedle "Run Main"!

    ![](img/img34.png)

37. Pokud celý proces úspěšně proběhl, vypíše se vám dole v okně "Process finished with exit code 0"

    ![](img/img35.png)

38. To samé, co s "clean, udělejte ještě pro "package".

    ![](img/img36.png)

39. Úspěšně skončeno:

    ![](img/img37.png)

40. Znovu zkuste "Reimport All Maven Projects".

    ![](img/img38.png)

41. Žádoucí výsledek: SwingExceptionHandler už není červeně.

    ![](img/img39.png)

42. Žádoucí výsledek je ukázán v kroku č. 32. Máte-li modrý a fialový text dle obrázku, můžete přejít k dalšímu kroku.

    Pokud přetrvává červený text, můžete zkusit ještě následující postup:
    - zavřete IntelliJ IDEA
    - spusťte soubor C:\Java-Training\Env\RunCmd.bat
    - do objevivší se příkazové řádky postupně napište (a na konci každé řádky stiskněte [Enter]) tyto tři příkazy:
    - `cd ..\Projects\DemoApplication`
    - `mvn clean`
    - `mvn package`
    - znovu zapněte IntelliJ IDEA
    - stiskněte tlačítko pro reimport projektu (viz krok č. 28)

43. Spusťte aplikaci klikem na zelenou šipku vpravo nahoře.

    ![](img/img40.png)

44. Pokud všechno funguje správně:

    ![](img/img41.png)


### Úklid dočasných souborů
Po instalaci je nepovinně možno vymazat dočasné soubory v Downloads (Java-Training a instalátor 7-Zipu), aby nezabíraly místo.


### A to je vše. Tešíme se na vás na akci.



<a id="kratky">Krátký popis (pouze pro zkušené):</a>
----------------------------------------------------
Tento popis je jen pro experty a popisuje jen slovně, co je potřeba provést pro úspěšnou instalaci.
Doporučujeme tento popis nepoužít a postupovat podle obrázků [výše](#detailni).

Na kurzu budete potřebovat Javu (OpenJDK) a programátorský editor IntelliJ IDEA (Community Edition).
**Nesmíte** si je ale nainstalovat z **oficiální** distribuce.
Místo toho si stáhněte 1 přednastavený archív, který se jen rozbalí do povinného umístění (`C:\Java-Training\`) a vše bude fungovat.

Poznámka: Nic se doopravdy neinstaluje, všechno se jen rozbalí pomocí 7-Zipu. Jde vlastně o *portable distribuci*.

Poznámka: Pokud už máte nainstalované **vlastní** JDK nebo IntelliJ IDEA, nevadí to, ale na kurzu je **používat nebudeme**.
Je opravdu nutné, abyste provedli instalaci dle těchto pokynů. Výukové programy z naší instalace nijak neovlivní
vaše už nainstalované programy. Pokud byste ale instalaci neprovedli, nešly by vám spouštět ukázkové příklady.

1.  Stáhněte si [Java-Training.7z](https://github.com/czechitas/java-install/releases/download/2019-podzim/community/win/Java-Training.7z).

2.  Pokud nemáte nainstalovaný **7-Zip**, nainstalujte si ho.

    Pozor! Nepoužívejte **WinRAR** ani **WinZip**, protože ty nedokáží správně rozbalit archívy `.7z`.
    Obecně doporučujeme **WinRAR** nebo **WinZip** úplně odinstalovat
    a používat výhradně **7-Zip**.
    Je zdarma, open-source a funguje výborně.

3.  Spusťte 7zFM.exe (7-Zip File Manager) a otevřete v něm `Java-Training.7z`.
    Rozbalte jej do `C:\Java-Training` (Extract to `C:\Java-Training`).

    Kontrola, že jste archív rozbalili do správného umístění:
    Po rozbalení musíte mít na disku `C:` tuto složku
    `C:\Java-Training\Projects\DemoApplication`

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
    `C:\Java-Training\`. Řešení - viz bod 33 v obrázkovém popisu instalace.

9.  Vpravo nahoře v editoru zezelená šipka pro spuštění ukázkového projektu. Tak jej spusťte.
    Projekt musí otevřít okno s nápisem `It works!`.
