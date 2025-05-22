# Git-LFS
Firstly dont forget to install homebrew and git lfs

How can I add files over 100 MB?
(100mb'tın üstündeki dosyaları bu kodları girerek ekleyebilirsin)

First, you should create a repository on GitHub. After that, add the repository to your desktop. Once you've done this, you can follow the the steps below
You must add the following codes to the terminal of the file in order:

1-) Open secret files (Shift+Command+point)

2-) Add .gitignore if file doesn't have (When you creating a repository don2t forget to add gitignore)(gitignore kısmı "Unity" olucak)

3-) In the file that has git, right click and find the .gitignore file path

Write the terminal this path 
cd /Users/Desktopowner/Desktop/JSprojects/Inventory-System

Now we are in the git file

4-) # Install Git LFS
git lfs install

5-)# Track large file types
git lfs track "*.psd"
git lfs track "*.png"
git lfs track "*.jpg"
git lfs track "*.fbx"

6-) Add this codes in .gitattribute file after delete everything ( 2 çizgi arası
----------------------
## Unity ##

*.cs diff=csharp text
*.cginc text
*.shader text

*.mat merge=unityyamlmerge eol=lf
*.anim merge=unityyamlmerge eol=lf
*.unity merge=unityyamlmerge eol=lf
*.prefab merge=unityyamlmerge eol=lf
*.physicsMaterial2D merge=unityyamlmerge eol=lf
*.physicMaterial merge=unityyamlmerge eol=lf
*.asset merge=unityyamlmerge eol=lf
*.meta merge=unityyamlmerge eol=lf
*.controller merge=unityyamlmerge eol=lf


## git-lfs ##

#Image
*.jpg filter=lfs diff=lfs merge=lfs -text
*.jpeg filter=lfs diff=lfs merge=lfs -text
*.png filter=lfs diff=lfs merge=lfs -text
*.gif filter=lfs diff=lfs merge=lfs -text
*.psd filter=lfs diff=lfs merge=lfs -text
*.ai filter=lfs diff=lfs merge=lfs -text
*.tif filter=lfs diff=lfs merge=lfs -text

#Audio
*.mp3 filter=lfs diff=lfs merge=lfs -text
*.wav filter=lfs diff=lfs merge=lfs -text
*.ogg filter=lfs diff=lfs merge=lfs -text

#Video
*.mp4 filter=lfs diff=lfs merge=lfs -text
*.mov filter=lfs diff=lfs merge=lfs -text

#3D Object
*.FBX filter=lfs diff=lfs merge=lfs -text
*.fbx filter=lfs diff=lfs merge=lfs -text
*.blend filter=lfs diff=lfs merge=lfs -text
*.obj filter=lfs diff=lfs merge=lfs -text

#ETC
*.a filter=lfs diff=lfs merge=lfs -text
*.exr filter=lfs diff=lfs merge=lfs -text
*.tga filter=lfs diff=lfs merge=lfs -text
*.pdf filter=lfs diff=lfs merge=lfs -text
*.zip filter=lfs diff=lfs merge=lfs -text
*.dll filter=lfs diff=lfs merge=lfs -text
*.unitypackage filter=lfs diff=lfs merge=lfs -text
*.aif filter=lfs diff=lfs merge=lfs -text
*.ttf filter=lfs diff=lfs merge=lfs -text
*.rns filter=lfs diff=lfs merge=lfs -text
*.reason filter=lfs diff=lfs merge=lfs -text
*.lxo filter=lfs diff=lfs merge=lfs -text

-------------------

7-) Add the Unity project in file
and also put the gitignore file in the Unity project file

8-) Do commit and push origin


Thanks ORKUN HACILAR this is the link;
https://www.youtube.com/watch?v=AQI7RDWONmo
