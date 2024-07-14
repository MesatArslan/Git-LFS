# Git-LFS
How can I add files over 100 MB?
(100mb'tın üstündeki dosyaları bu kodları girerek ekleyebilirsin)

You must add the following codes to the terminal of the file in order:
1-) # Install Git LFS
git lfs install

2-)# Track large file types
git lfs track "*.psd"
git lfs track "*.png"
git lfs track "*.jpg"
git lfs track "*.fbx"

3-)# Add all files to the repository
git add .

4-)# Commit the files
git commit -m "Add Unity project with Git LFS tracking"

5-)# Push to GitHub (assuming 'origin' is your remote repository)
git push origin main

işe yaramıyor güncelle
