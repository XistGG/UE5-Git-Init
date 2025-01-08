# UE5-Git-Init

Xist's UE5 Git Init: Initial Contents for a New Git Repo

You can copy the `.gitignore` and `.gitattributes` files from this empty repo
into your new empty repo to initialize it for a UE5 project before you import
any files.

This `.gitattributes` enables LFS for binary project assets.
You could potentially use a different setup if you do not want
to use LFS for some reason.

Make sure you keep the text file settings RE `*.bat`, `*.sh` at the top of `.gitattributes`,
those are important for UE5 projects to function correctly on different platforms.


## Download Instructions

```powershell
$GitInitRepoUrl = "https://raw.githubusercontent.com/XistGG/UE5-Git-Init/main"

# REQUIRED: Copy .gitignore and .gitattributes
curl -O $GitInitRepoUrl/.gitignore
curl -O $GitInitRepoUrl/.gitattributes

# OPTIONAL: Copy Github/Rider/VS .editorconfig
curl -O $GitInitRepoUrl/.editorconfig

# OPTIONAL: Copy MIT LICENSE (free use for anyone including commercial)
curl -O $GitInitRepoUrl/LICENSE
```


## Example Usage

```powershell
git init

git lfs install

git add .gitignore .gitattributes

git commit -m "Initialize UE5 Git Repo"
```


These files are used by
[Xist's How to Create a Lyra Repo](https://x157.github.io/UE5/LyraStarterGame/Tutorials/How-to-Create-a-Lyra-Repo)
tutorial.
