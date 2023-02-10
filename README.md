# UE5-Git-Init

Xist's UE5 Git Init -- Initial Contents for a New Git Repo

You can copy the `.gitignore` and `.gitattributes` files from this empty repo
into your new empty repo to initialize it for a UE5 project before you import
any files.

This `.gitattributes` enables LFS for binary project assets.
You could potentially use a different setup if you do not want
to use LFS for some reason.

Make sure you keep the text file settings RE `*.bat`, `*.sh` at the top,
those are important for UE5 projects to function correctly on different platforms.

```powershell
git init

git add .gitignore .gitattributes

git commit -m "Initialize UE5 Git Repo"
```
