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
        - Java-Training.7z (2022-01-13)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2022-jaro/community/win/Java-Training.7z
    - macOS
        - Java-Training.zip (2022-01-13)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2022-jaro/community/mac/Java-Training.zip
- Ultimate
    - Windows
        - Java-Training.7z (2020-01-29)<br/>
          https://github.com/czechitas/java-install-dist/releases/download/2020-jaro/ultimate/win/Java-Training.7z
    - macOS
        - Java-Training.zip (2021-03-24)<br/>
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
Aby fungoval redirect z verzovaných stránek https://javainstall.czechitas.cz/2022-jaro/community/ na aktuální stránku s pokyny (např. https://javainstall.czechitas.cz/community/),
je v Jekyllu přidáno nastavení ve Front matter v cílové stránce (např. `/docs/2022-jaro/community/index.md`):
~~~~
---
redirect_to: "/community/"
---
~~~~
