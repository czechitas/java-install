Short description (only for the experienced):
=================================
This guide is only for experienced users who know what they are doing.
We recommend going back up and follow the [detailed guide](index-eng.html).



The installation guide
----------------------
The training course requires installation of Java (OpenJDK), Tomcat, MariaDB and a programming editor IntelliJ IDEA (Ultimate Edition).
**Do not install** it from the **offcial** distribution.
Use our preconfigured archive which you just extract to the fixed folder on the disk (`C:\Java-Training\`) and you are good to go.

Note: In fact, there is no serious installation going on. Files are just extracted to the fixed folder. It is a kind of a *portable distribution*.

Note: If you already have our own JDK or other included software installed on your computer,
it is not a problem but it will not be used for the training course. It is absolutely necessary to use the piece of software from our installation package
as it is all preconfigured. Our examples would not work without the special configuration.

1.  Download [Java-Training.7z](https://github.com/czechitas/java-install-dist/releases/download/2020-jaro/ultimate/win/Java-Training.7z).

2.  If you do not have **7-Zip**, download and install it.

    Warning! Do not use **WinRAR** or **WinZip**, because they cannot extract `.7z` correctly.
    In general we recommend to uninstall **WinRAR** and **WinZip** completely as you must pay for their license.
    We consider it pointless when there is the free and open-source 7-Zip.
3.  Run 7zFM.exe (7-Zip File Manager) and open `Java-Training.7z` in it.
    Extract the archive to `C:\Java-Training`.

    Check that you extracted it correctly:
    You should have
    `C:\Java-Training\Projects\DemoWebApplication`
    folder on your `C:` drive.

4.  Copy `IntelliJ-Ultimate.lnk` from `C:\Java-Training\IntelliJ-Ultimate`
    to your desktop (`C:\Users\YOUR_USERNAME\Desktop`) and possibly to your Start Menu
    (`C:\Users\YOUR_USERNAME\AppData\Roaming\Microsoft\Windows\Start Menu\Programs`)

5.  Run `IntelliJ-Ultimate` using the shortcut from previous step
    or run `C:\Java-Training\IntelliJ-Ultimate\startup.bat`.

6.  Open the demo project selecting the folder
    `C:\Java-Training\Projects\DemoWebApplication`.
    You must be connected to the internet.

7.  When you open the project, IntelliJ IDEA will start indexing JDK and libraries.
    It will take a couple of minutes.
    Progress is displayed on the bottom editor line.

8.  After the indexing finishes, `Main.java` will become mainly violet-blue.

    If it stayed mainly black-grey, you wouldn't have it extracted to the correct folder.
    It must be in `C:\Java-Training`. In such a case, close everything, move it to the correct location and run IntelliJ IDEA again.
    If it was red, follow on to the troubleshooting section of the detailed guide
    (point 17 in the detailed installation guide).

9.  If everyhing is successful, you can run the project using the green arrow on the right top bar.
    An address of a locally started demo web application will appear in console frame.
    The address will look like: http://localhost:54321/DemoWebApplication/

10. If you click the address, your default web browser will open a page with `It works!` label.
