Instalace pro kurzy Java
========================

Tato repository obsahuje:
-   Ve složce `docs/` webové stránky <https://javainstall.czechitas.cz/>.
-   Release Tags se všemi archívy instalaček (Java-Training.7z) ke stažení (i historickými).
-   Ve složce `Pro lektory` informace o tom, proč a jak je instalace strukturovaná.
-   (V budoucnu) Ve složce `Patched_files` bude obsahovat všechny změněné soubory proti výchozím distribucím jednotlivých softwarů.

----

Pozor, odkazujte studenty vždy na stránku https://javainstall.czechitas.cz/community/
nebo https://javainstall.czechitas.cz/ultimate/
protože při přístupu na ně bude webový prohlížeč automaticky přesměrován na aktuální stránky.



Datum releasu nové verze
------------------------
Release se provádí vždycky posledního května a posledního listopadu.
Do té doby je nutné, aby všichni lektoři zadali na GitHubu všechny požadované Issues
nebo zaslali návrhy Kamilu Ševečkovi, který tuto instalaci udržuje.



Aktuální verze distribučních archívů:
------------------------------------
- Community
    - Windows
        - Java-Training.7z (2019-10-11 12:52)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2020-jaro/community/win/Java-Training.7z
    - macOS
        - Java-Training.zip (2019-10-11 14:47)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2020-jaro/community/mac/Java-Training.zip
- Ultimate
    - Windows
        - Java-Training.7z (2019-10-11 12:02)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2020-jaro/ultimate/win/Java-Training.7z
    - macOS
        - Java-Training.zip (2019-10-11 13:45)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2020-jaro/ultimate/mac/Java-Training.zip



### Kde a jak jsou uložené distribuční archívy:

Distribuční archívy jsou publikované jako binární soubory v určitém githubovém [**releasu**](https://github.com/czechitas/java-install/releases).
**Release** na GitHubu je sada souborů (**assets**) asociovaná s gitovým **tagem**.
Pro naše účely jsou vytvořeny tagy `2019-podzim/community/win`, `2019-podzim/community/mac`,
`2019-podzim/ultimate/win`, `2019-podzim/ultimate/mac` atd.
Jsou nastaveny na **commit** v **masteru**, který byl aktuální, když vznikly, ale to není důležité.
Není třeba to měnit a i přesto je možné ve webovém rozhraní GitHubu vyměnit dané asociované soubory **releasu** (**assets**).
Jinými slovy, soubory **releasu** (**assets**) nejsou uložené v gitové repozitoři, ale někde mimo na GitHubu a nejsou tudíž verzované.

### Názvy **tagů**
Názvy **tagů** se promítají do URL pro stažení. Mohou obsahovat lomítko, takže to vypadá, jako by soubory **releasu** (**assets**)
byly v podadresářích.
Například: `https://github.com/czechitas/java-install-dist/releases/download/`**NAZEV_TAGU**`/Java-Training.7z`.



Tech tip
--------
Aby fungoval redirect z https://javainstall.czechitas.cz/community/ na konkrétní stránku s pokyny (např. https://javainstall.czechitas.cz/2020-jaro/community/),
je v Jekyllu přidán plugin `redirect`. V cílové stránce (např. `/docs/2020-jaro/community/index.md`) musí být uvedeno:
~~~~
---
redirect_from: "/community/"
---
~~~~
