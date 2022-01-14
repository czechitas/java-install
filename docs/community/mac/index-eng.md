Installation guide for macOS
============================

This guide is **only for macOS**.
You can choose Windows or Linux guide [here](../).

Follow the instructions even if you already have some of the software installed
(including `/Users/YOUR_USERNAME/Java-Training`). You will not lose any previous `Projects` because this folder is not being erased.
Although, you might want to backup `/Users/YOUR_USERNAME/Java-Training` to e.g. `Documents` folder temporarily.
All other files and subfolders of `/Users/YOUR_USERNAME/Java-Training` will either stay intact or will be overwritten by a newer version of the software.



Installation
------------

1. Download the installation archive:
   [Java-Training.zip](https://github.com/czechitas/java-install/releases/download/2022-jaro/community/mac/Java-Training.zip)


2. Follow the video guide:

    <a href="https://www.youtube.com/watch?v=MJ5fcocKc-0">
        <img src="img/video-screenshot.png"/>
    </a>


3. Try to open and run the Demo project:

    <a href="https://www.youtube.com/watch?v=4lOfLpJDp3c">
        <img src="img/video-demo_project-screenshot.png"/>
    </a>


### Removal of Temporary Files

After the installation is finished, you may optionally remove redundant files in `Downloads` (`Java-Training`) to reclaim some disk space.



<br/><br/><br/><br/>



### Troubleshooting

1.  Problem: You open `Downloads` folder (instead of a valid project `DemoApplication`). Also `Maven` tab is missing on the right hand side bar.

    <a href="img/imported-wrong-folder.png">
        <img src="img/imported-wrong-folder-thumbnail.png"/>
    </a>

    Reason: You misclicked in the open dialog and accidentally clicked on a wrong folder to open.

    Solution: In **IntelliJ IDEA**, choose menu **File** -> **Open...** and choose the correct folder. Pay attention to the correct treatment of the open dialog in the regular video guide.


2.  Problem: Maven build failed or the source code remained red.

    <a href="img/missing-dependencies.png">
        <img src="img/missing-dependencies-thumbnail.png"/>
    </a>

    There may be multiple reasons:
    - You are currently disconnected from the internet.

      Solution: You need to be connected to the internet the entire time. It will be useful during the programming as well.
      Go through the entire installation video guide once more while connected to the internet.

    - VPN (i.e. on a company computer).

      Reason: You may have your Windows set up so that **Maven** should use your company private Java library repository, accessible only via VPN. Such a configuration would be in `/Users/YOUR_USERNAME/.m2/settings.xml`.

      Solution: Compilation using **Mavenem** (`clean` and `package`) is necessary to be done with internet connection via VPN. Better stay connected to the internet via VPN the whole time.

    - Prior points are fixed but there is still a problem that **IntelliJ IDEA** displays the code with incorrect color.

      Solution: If red colors remain even after repeated execution of **Maven** goals (`clean` a `package`), you may try somewhat more heavy duty approach:
        - Close **IntelliJ IDEA**
        - Run `$HOME/Java-Training/Env/RunCmd.command` in terminal (**Open with** -> **Terminal**)
        - A Command line will appear. Write following commands into it (and finish each by pressing [Enter]):
            - `cd $HOME/Java-Training/Projects/DemoApplication`
            - `mvn clean package exec:java`
        - This time the `It works` window should appear.
        - Start up **IntelliJ IDEA**.
        - Click on Reimport Maven project again.

        You can follow the video guide:

        <a href="https://www.youtube.com/watch?v=eTjTplwQSyE">
            <img src="img/video-maven_troubleshooting-screenshot.png"/>
        </a>


3. Maven build was OK, everything in the file `Main.java` is blue / violet,
   especially line 3 in the green box `import net.sevecek.util.SwingExceptionHandler;`
   is blue (as opposed to the red error), but the project still fails to start.

    <a href="img/maven-ok-compiler-fail.png">
        <img src="img/maven-ok-compiler-fail-thumbnail.png"/>
    </a>

   Solution: Restart IntelliJ IDEA. When IntelliJ IDEA restarts, it should already work.
   Perhaps an error in Matrix.


4. If none of the prior worked, will will fix the problem in person before the training.



<br/><br/><br/><br/>



Uninstallation
--------------

The only thing installation in fact does is extract the files to `/Users/YOUR_USERNAME/Java-Training` and spawns a Start menu shortcut for **IntelliJ IDEA**.
To remove the software package, backup your projects in `/Users/YOUR_USERNAME/Java-Training/Projects`, e.g. to `/Users/YOUR_USERNAME/Documents`.
Afterwards, just delete the entire `/Users/YOUR_USERNAME/Java-Training`.
Also, delete the **IntelliJ IDEA** app in `/Users/YOUR_USERNAME/Applications`.

Almost done.

**Maven** downloads Java libraries to its cache folder in `/Users/YOUR_USERNAME/.m2/repository`. Delete it too.
And that is all.



<br/><br/><br/><br/>



Notes for those curious
-----------------------

You will use **Javu** during the training course (namely **AdoptOpenJDK**) and programmer's editor **IntelliJ IDEA** (**Community Edition**).
You **must not** install it from the **official** sources.
Use our bundled archive, which is just extracted to (`/Users/YOUR_USERNAME/Java-Training`) and everything works automatically.
If you installed software from the official sources, you wouldn't have it configured properly for the training.

Note: The software is not really *installed* at all. All files are just extracted from the zip archive (which is bundled inside `Java-Training.zip`).
Software configuration is diverted to `/Users/YOUR_USERNAME/Java-Training/User-Config` and does not use the user profile folder.
therefore it is very much a *portable distribution*.

Note: If you already have a *regular* **JDK** or **IntelliJ IDEA** installed, it is not a problem. We will just *not use it*.
The software from our installation does not interfere with your regular applications.
