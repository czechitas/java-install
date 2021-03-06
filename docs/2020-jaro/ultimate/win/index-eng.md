Installation Guide for Windows
==============================

This guide is **only for Windows**.
You can choose macOS guide [here](../).

Linux **is not** supported. If you needed Linux installation guide, please, contact us.

Follow the instructions even if you already have some of the software installed
(including `C:\Java-Training`). Existing software will just update and any previous projects will not be lost. The `C:\Java-Training\Projects` folder is not erased.
All other files and subfolders of `C:\Java-Training` will either stay intact or will be overwritten by a newer version of the software.


If you are an experienced user, you can skip to the short [description](advanced-eng.html),
but we recommend to follow this version.



Detail guide:
-------------

1.  Install **7-Zip**.

    Watch out: 7-Zip is better than **WinRAR** or **WinZip**.
    Install it even if you already have them.
    Especially we noticed **WinRAR** being unable to extract `.7z` correctly.
    We recommend avoid **WinRAR** and **WinZip** altogether and use exclusively **7-Zip** as it is free and open-source.

	![](img/img001.png)

3.  Run the downloaded installator for 7-Zip.

4.  ![](img/img002.png)

5.  ![](img/img003.png)

6.  ![](img/img004.png)

7. If you are asked by Windows to permit admin changes, go ahead. (Yes/Ano)

    ![](img/img005.png)

8.  ![](img/img006.png)

9. 	![](img/img007.png)

10. Run **7-Zip File Manager**.

    ![](img/img008.png)

11. Open app settings.

    ![](img/img009.png)

12.	Check whether you have 7-Zip associated with .7z a .zip. We recommend using it for all types of supported archives. (All types can be selected by the plus + button)

    ![](img/img010.png)

13.	A couple of convenient settings. Confirm by clicking OK and close all settings dialogs.

    ![](img/img011.png)



<br/><br/><br/><br/><br/>



### The installation procedure itself

1.  Download the installer
    [Java-Training_setup.exe](https://github.com/czechitas/java-install/releases/download/2020-jaro/ultimate/win/Java-Training_setup.exe)

2.  Find the downloaded file `Java-Training_setup.exe` (probably in
    `Downloads`) and run it.

    ![](img/img100.png)

3.  You will probably hit the warning of missing digital signature. This is not a problem. Accept the exception.

    ![](img/img101.png)

4.  ![](img/img102.png)

5.  If you were unable to run the installer anyway or your antivirus does not allow to run it,
    **switch to the manual [extraction of an archive](alternative-eng.html)**. Otherwise, follow on.

6.  ![](img/img103.png)

7.  ![](img/img104.png)

8.  ![](img/img105.png)

9.  ![](img/img106.png)

10. Installation is finished.



<br/><br/><br/><br/><br/>



### <a id="test">Test the installation</a>

1.  Run IntelliJ IDEA - Ultimate Edition. Be patient - the computer will look like it is "doing nothing" after double click, but the splash screen should appear shortly.
    It is necessary to be connected to the internet at this point.

    ![](img/img300.png)

2.  Make sure you are **connected to the internet**.

3.  Choose Evaluate for free.

4.  IntelliJ IDEA will start.

    ![](img/img303.png)

5.  Open the demo project `C:\Java-Training\Projects\DemoWebApplication`.

    ![](img/img304.png)

6.  Watch out! Always expand the arrows in the open dialog
    **using single click only**
    to drill down to subfolder.
    **Never click twice** on the folder name.
    Sometimes it could be mistakenly understood by IntelliJ IDEA to import the entire double-clicked folder and not just expanding the folder.

    ![](img/img305.png)

7.  ![](img/img306.png)

8.  Wait for IntelliJ IDEA to index the entire Java runtime.
    When first run, it can take several minutes.
    It is necessary to still be connected to the internet.

    ![](img/img307.png)

9.  You should see `Main.java` in the open project. If not, expand the folders in the left panel (clicking on the arrows again) and double-click on the `Main.java`.

    ![](img/img308.png)

10. If IntelliJ IDEA is correctly set up, the source code in `Main.java`
    should be blue-violet as on the picture.
    If you see it you can skip to step 21.

    ![](img/img309.png)

11. If you had a problem with internet connection, it could happen that you would see errors like bellow. If not, skip the corrective steps.

    ![](img/img310.png)

12. Corrective steps: When finally on the internet, open "Maven" tab.

    ![](img/img311.png)

13. Click `Reimport All Maven Projects` button.

    ![](img/img312.png)

14. Still not fixed? Open Maven `Lifecycle`, choose `clean` and run the action. Watch out! It is a **different arrow then `Run Main`**!

    ![](img/img313.png)

15. It it went OK, you will see `Process finished with exit code 0`

    ![](img/img314.png)

16. Follow on with `package` goal.

    ![](img/img315.png)

17. Success:

    ![](img/img316.png)

18. Repeat `Reimport All Maven Projects`.

    ![](img/img317.png)

19. Look for `SwingExceptionHandler` not being red now.

    ![](img/img318.png)

20. Check the correct situation on picture 19. If it is OK, follow on.

    If not, try more heavy duty steps:
    - Close IntelliJ IDEA
    - Run `C:\Java-Training\Env\RunCmd.bat`
    - Write to the (black) command line (and confirm each line with `Enter`):
    - `cd ..\Projects\DemoWebApplication`
    - `mvn clean`
    - `mvn package`
    - Run IntelliJ IDEA again
    - Click `Reimport All Maven Projects` (as in step 12)
    - If it doesn't help, we will fix it at the workshop.

21. Run the application

    ![](img/img319.png)

22. Click on the generated link.

    ![](img/img320.png)

23. Everything should work now:

    ![](img/img321.png)



### Temporary files clean up

You can erase files from `Downloads` (`Java-Training.7z` and `7-Zipu` installer), to save some disk space.



### And that's it. We are looking forward to meet you at the workshop.
