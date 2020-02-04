Instalační pokyny pro Windows
=============================

Tyto pokyny jsou **výhradně pro Windows**.
Instalaci pro macOS můžete vybrat [o složku výše](../).

Linux **není** podporován. Pokud byste potřebovali instalaci pro Linux,
bylo by nutno se dostatečně dopředu ozvat lektorovi.

Tyto instrukce následujte i pokud už máte nějaké programy v
`C:\Java-Training` z minula. Žádný strach, původní programy se jen aktualizují a vaše vlastní projekty zůstanou zachovány.
Projekty máte v `C:\Java-Training\Projects` a tato složka se nemaže.
Ostatní programy v `C:\Java-Training` buď zůstanou nedotčeny
nebo budou přepsány novější verzí programů, což je v pořádku.

Zkušení uživatelé mohou přeskočit ke [krátkému popisu](advanced.html),
ale doporučujeme to nedělat a držet se tohoto obrázkového návodu.



Detailní postup:
-----------------

1.  Nainstalujte si **7-Zip**, pokud ho ještě nemáte.

    To platí i v případě, že už máte **WinRAR** nebo **WinZip**.
    Především **WinRAR** nedokáže soubory `.7z` správně rozbalit.
    Obecně doporučujeme **WinRAR** nebo **WinZip** úplně odinstalovat
    a používat výhradně **7-Zip**.
    Je zdarma, open-source a funguje výborně.

	![](img/img001.png)

3.  Stažený soubor - instalátor 7-Zipu - spusťte.

4.  ![](img/img002.png)

5.  ![](img/img003.png)

6.  ![](img/img004.png)

7. Pokud se Windows ptá, zda chcete aplikaci povolit provádět změny, dialog odsouhlaste. (Yes/Ano)

    ![](img/img005.png)

8.  ![](img/img006.png)

9. 	![](img/img007.png)

10. Spusťte **7-Zip File Manager**. Spouštění se může lišit v závislosti
    na verzi Windows.

    ![](img/img008.png)

11.	Otevřete nastavení programu.

    ![](img/img009.png)

12.	Zkontrolujte, zda máte 7-Zip asociovaný minimálně se soubory .7z a .zip. Vřele doporučujeme používat ho na všechny archívy. (Všechny typy souborů označíte/odznačíte v dialogu tlačítkem plus +)

    ![](img/img010.png)

13.	Ještě pár nastavení pro přehlednější chování 7-Zipu. Na konci potvrďte změny tlačítkem OK. Všechna otevřená okna potom zavřete.

    ![](img/img011.png)



### Samotný postup instalace

1.  Stáhněte si instalátor
    [Java-Training_setup.exe](https://github.com/czechitas/java-install/releases/download/2020-jaro/ultimate/win/Java-Training_setup.exe)

2.  Najděte na počítači uložený soubor `Java-Training_setup.exe` (pravděpodobně je ve složce
    `Downloads`) a spusťte ho.

    ![](img/img100.png)

3.  Budete upozorněni, že instalátor není digitálně podepsán. To není problém. Schvalte výjimku.

    ![](img/img101.png)

4.  ![](img/img102.png)

5.  Pokud by nešlo výjimku pro instalátor schválit, přejďete na ruční [rozbalení archívu](alternative.html). Jinak pokračujte zde.

6.  ![](img/img103.png)

7.  ![](img/img104.png)

8.  ![](img/img105.png)

9.  ![](img/img106.png)

10. Instalace je hotová.



### <a id="test">Zkouška nainstalovaných programů</a>

1.  Spusťte IntelliJ IDEA - Ultimate Edition. Buďte trpěliví - je normální, že počítač nějakou dobu *nic nedělá*, než naskočí úvodní obrazovka.
    Od tohoto bodu je nutné, abyste byli **připojení na internet**.

    ![](img/img300.png)

2.  Vložte Offline activation code svojí licence, kterou jste si pořídili zdarma na e-shopu JetBrains.

    ![](img/img301.png)

    ![](img/img302.png)

3.  Pokud byste zatím od nás nedostali slevový kupón, lze zvolit Evaluate for free.

4.  IntelliJ IDEA se spustí.

    ![](img/img303.png)

5.  Otevřete ukázkový projekt `C:\Java-Training\Projects\DemoWebApplication`.

    ![](img/img304.png)

6.  Pozor, v otevíracím dialogu rozklikávejte levé šipečky
    **pouze jedním kliknutím**
    a vstupujte tak do podsložek.
    **Neklikejte** na jméno složky **2x**.
    IntelliJ IDEA to čas od času může špatně pochopit a pokusit se složku,
    ve které není javový projekt, importovat.

    ![](img/img305.png)

7.  ![](img/img306.png)

8.  Počkejte, než IntelliJ IDEA po prvním spuštění naindexuje Javu.
    Může to trvat několik minut.

    ![](img/img307.png)

9.  V otevřeném projektu byste měli vidět soubor `Main.java`. Pokud ne, rozklikněte složky v projektu a dvojklikem na jméno souboru ho otevřete v editoru.

    ![](img/img308.png)

10. Správně nastavená IntelliJ IDEA obarvuje zdrojový text v Main.java
    do modrofialova stejně, jak je vidět na obrázku.
    Pokud to tak je, můžete přeskočit na krok 21.

    ![](img/img309.png)

11. Pokud naopak máte v tenhle moment problém s internetovým připojením, může se přihodit, že se nestáhnou všechna potřebná data. V takovém případě budete mít části textu červené - jako na obrázku níže.

    ![](img/img310.png)

12. Náprava: otevřete záložku "Maven" na pravé straně obrazovky.

    ![](img/img311.png)

13. Stiskněte tlačítko se šipkami "Reimport All Maven Projects" a nechte počítač pracovat.

    ![](img/img312.png)

14. Nepomohlo a pořád jsou některé části textu červené? Rozklikněte v záložce Mavenu složku "Lifecycle", označte "clean" a spusťte akci zelenou šipkou. POZOR, nespleťte si tuhle šipku se stejně vyhlížející šipkou o něco výše vedle "Run Main"!

    ![](img/img313.png)

15. Pokud celý proces úspěšně proběhl, vypíše se vám dole v okně "Process finished with exit code 0"

    ![](img/img314.png)

16. To samé, co s `clean`, udělejte ještě pro `package`.

    ![](img/img315.png)

17. Úspěšně skončeno:

    ![](img/img316.png)

18. Znovu zkuste "Reimport All Maven Projects".

    ![](img/img317.png)

19. Žádoucí výsledek: SwingExceptionHandler už není červeně.

    ![](img/img318.png)

20. Žádaný výsledek je ukázán v kroku č. 19. Máte-li modrý a fialový text dle obrázku, můžete přejít k dalšímu kroku.

    Pokud přetrvává červený text, můžete zkusit ještě následující postup:
    - zavřete IntelliJ IDEA
    - spusťte soubor C:\Java-Training\Env\RunCmd.bat
    - do objevivší se příkazové řádky postupně napište (a na konci každé řádky stiskněte [Enter]) tyto tři příkazy:
    - `cd ..\Projects\DemoWebApplication`
    - `mvn clean`
    - `mvn package`
    - znovu zapněte IntelliJ IDEA
    - stiskněte tlačítko pro reimport projektu (viz krok č. 12)

21. Spusťte aplikaci klikem na zelenou šipku vpravo nahoře.

    ![](img/img319.png)

22. Klikněte na vygenerovaný odkaz.

    ![](img/img320.png)

23. Pokud všechno funguje správně:

    ![](img/img321.png)



### Úklid dočasných souborů

Po instalaci je nepovinně možno vymazat dočasné soubory v Downloads (Java-Training a instalátor 7-Zipu), aby nezabíraly místo.



### A to je vše. Tešíme se na vás na akci.
