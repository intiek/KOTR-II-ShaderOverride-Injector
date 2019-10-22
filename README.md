# KOTR-II-ShaderOverride-Injector
A script to fix issues with fog in Star Wars: Knights of the Old Republic II: The Sith Lords caused by a Steam patch. See https://www.reddit.com/r/kotor/comments/67578l/aspyr_wont_patch_the_fog_on_dxun_but_a_fan_made/.

As posted by TonyKaku on Reddit thread https://www.reddit.com/r/kotor/comments/8rfm1l/kotor_1_and_2_mod_builds_guaranteed_compatibility/e0qxp2x/, a patch released for
Star Wars: Knights of the Old Republic II: The Sith Lords caused issues with fog. HappyFunTimes released ShaderOverride, a fix that addresses this issues at https://github.com/HappyFunTimes01/ShaderOverride. The fix requires pasting new lines of codes into multiple generated text files. In order to make the process easier I have created this simple script. (Install Steps Originally by TonyKaku)

Using the Script:
1. Download the ShaderOverride DLL HappyFunTime's GIT and put it into your KOTOR2 root folder.

2. Start the game.

3. You should now have two folders called shaders_original and shadow_override in your KOTOR folder.

4. Run ShaderOverrideFix.exe.

5. Browse to your shaders_original folder when asked. 

6. When the script is complete copy all text files into the shader_override folder.

7. Launch the game.

This script automates the following steps for you: 

-Go into the shaders_original folder and open the first file with a program like Notepad++

-locate the line that says "MOV result.color, r0" (second to last line usually)

-right above that line paste the content of the quote under "Fog Issue" that starts with PARAM p =.... Your file should look like this.

-Repeat this step for every text file in the folder that has the MOV result.color, r0 line. That can take some time and there might be ways to automate the process but explaining it might take so long that you're probably just better off doing the whole thing manually.
