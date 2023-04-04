<<<<<<< HEAD
#  1.上传本地文件到Github库的基本步骤：

* **下面仅供了解，具体命令行代码在后面，如果时间紧迫，下面可以不看，直接跳到第一步**
=======
[TOC]

#  1.GitHub 的一些基本步骤：
>>>>>>> 3f36f7f03e5a57d584c948afa41f9bf597a469c9

1. 注册一个 GitHub 账号：如果你还没有 GitHub 账号，你需要先注册一个。前往 GitHub 官网，点击“Sign up”按钮，填写必要信息并创建账号。
2. 创建一个新仓库：登陆 GitHub 后，点击右上角的“+”号，然后选择“New repository”来创建一个新仓库。填写仓库名称、描述等信息，并选择仓库类型（公开或私有）。
3. 在本地计算机上设置 Git：Git 是一个版本控制工具，你需要在本地计算机上安装并设置 Git，才能使用 GitHub。你可以在 Git 官网上下载 Git。
4. 在本地计算机上创建一个本地仓库：使用 Git 在本地计算机上创建一个本地仓库，作为代码的存储和版本控制。
5. 将本地仓库与 GitHub 远程仓库连接：使用 Git 将本地仓库与 GitHub 远程仓库进行连接。你需要将本地仓库的内容推送到远程仓库，才能在 GitHub 上查看和管理代码。
6. 使用 Git 进行版本控制：使用 Git 进行代码的版本控制。通过 Git 命令，你可以将代码提交到本地仓库，并进行版本回退、分支管理等操作。
7. 在 GitHub 上管理代码：在 GitHub 上，你可以查看、编辑、删除代码，管理分支、合并请求、Issues等。你可以通过网页界面或命令行工具进行管理。

<<<<<<< HEAD
# 2.(第一步)在GitHub上创建仓库（远程仓库）

* 具体操作步骤如下：

  1. 在 GitHub 上创建一个新的代码仓库。
     - 打开 GitHub 网站，登录账号。
     - 点击页面右上角的加号图标，选择 "New repository" 创建新的仓库。
     - 输入仓库名称、描述等信息，选择公开或私有，然后点击 "Create repository" 完成创建。

# 3.(第二步)安装Git

* **安装 Git 可以按照以下步骤进行：**

  1. 在 Git 官网（https://git-scm.com/downloads）下载适用于你的操作系统的 Git 安装包，例如 Windows 或 macOS 系统。该软件包包含了 Git Bash、Git GUI 等常用工具。

  2. 安装 Git。在 Windows 操作系统中，双击下载的 Git 安装包，按照提示进行安装即可。在 macOS 操作系统中，双击下载的 dmg 文件，将 Git 拖动到“应用程序”文件夹中即可完成安装。

  3. 配置 Git。安装完成后，打开终端或 Git Bash（Windows 系统），输入以下命令来配置 Git：

     ```
     git config --global user.name "Your Name"
     git config --global user.email "your_email@example.com"
     ```

     这里的 `"Your Name"` 和 `"your_email@example.com"` 分别为你的用户名和邮箱地址，将它们替换为你自己的即可。这些信息将用于标识你提交的代码的作者。

  4. 在安装配置完Git,任意右击你电脑的文件夹都能看到Git Gui Here和Git Bush Here

     * Git Bash：Git Bash 是 Git 在 Windows 操作系统上的命令行工具，它提供了一种与 Linux 和 macOS 终端类似的界面，可以通过命令行执行 Git 的各种操作。使用 Git Bash 可以快速、方便地操作 Git，而不需要在 Windows 上安装类 Unix 的命令行工具。
     * Git GUI：Git GUI 是 Git 提供的图形界面工具，它提供了一个可视化的界面，可以用来执行 Git 的大多数操作。Git GUI 支持各种 Git 操作，包括提交、分支管理、版本控制等。相对于 Git Bash，Git GUI 更加直观易用，可以方便地执行一些常见的 Git 操作。

  5. 检查 Git 是否已经安装：

     ```
     git --version
     ```

     如果 Git 已经安装，则会显示 Git 的版本号，例如：`git version 2.33.0`.

  6. 检查 Git 是否已经配置用户名和邮箱：

     ```
     git config --global user.name
     git config --global user.email
     ```

     如果输出了你的用户名和邮箱地址，则说明 Git 已经配置完成。如果没有输出，则说明你还需要配置用户名和邮箱。则需要执行上面配置Git步骤。

# 4.(第三步)上传文件到Github步骤（本地仓库-->远程仓库）
* 以简单上传django_project项目文件夹为案例。

1. 在本地电脑上创建一个文件夹，用于存储django_project项目文件。

2. 在该文件夹下初始化 Git 仓库，（右击文件夹，点击Git Bsuh Here进入终端，前提是在 Git 官网下载适用于你的操作系统的 Git 安装包）执行以下命令：
=======


# 2.电脑中的git Bush和GUI

* 下载最新的 Git 安装程序：在 Git 官网（https://git-scm.com/downloads）上下载最新的 Git for Windows 软件包，该软件包包含了 Git Bash、Git GUI 等常用工具。
* Git Bash：Git Bash 是 Git 在 Windows 操作系统上的命令行工具，它提供了一种与 Linux 和 macOS 终端类似的界面，可以通过命令行执行 Git 的各种操作。使用 Git Bash 可以快速、方便地操作 Git，而不需要在 Windows 上安装类 Unix 的命令行工具。
* Git GUI：Git GUI 是 Git 提供的图形界面工具，它提供了一个可视化的界面，可以用来执行 Git 的大多数操作。Git GUI 支持各种 Git 操作，包括提交、分支管理、版本控制等。相对于 Git Bash，Git GUI 更加直观易用，可以方便地执行一些常见的 Git 操作。

# 3.上传的简单的步骤

* 简单的叙述步骤，如果想弄懂原理，请看下面的细讲

​	简单上传jango项目文件夹案例，这是把一个文件夹作为一个整体上传到github库里面

1. 在本地电脑上创建一个文件夹，用于存储django_project项目文件。

2. 在该文件夹下初始化 Git 仓库，执行以下命令：（右击文件，点击git bsuh进入终端）
>>>>>>> 3f36f7f03e5a57d584c948afa41f9bf597a469c9

   ```
   git init
   ```

3. 将 Django 项目文件夹添加到本地仓库中，执行以下命令：

   ```
   git add django_project/
   #或者输入
   git add .
   ```

<<<<<<< HEAD
   使用 `git add` 命令将代码添加到本地仓库的暂存区中，这些文件并不会立即被提交到 Github 仓库中，而是等待下一操作,将本地仓库与远程仓库进行关联。

4. 将当前工作目录中的更改保存到本地代码仓库中，执行以下命令：
=======
4. 提交代码到本地仓库，执行以下命令：
>>>>>>> 3f36f7f03e5a57d584c948afa41f9bf597a469c9

   ```
   git commit -m "Initial commit"
   ```

<<<<<<< HEAD
5. 在 GitHub 上创建一个新的远程仓库，获取复制该仓库的 SSH 或 HTTPS 链接。
=======
5. 在 GitHub 上创建一个新的远程仓库，获取该仓库的 SSH 或 HTTPS 链接。
>>>>>>> 3f36f7f03e5a57d584c948afa41f9bf597a469c9

6. 将本地仓库与远程仓库进行关联，执行以下命令：

   ```
   git remote add origin <远程仓库链接>
<<<<<<< HEAD
   #<远程仓库链接>就是你刚才复制的仓库的 SSH 或 HTTPS 链接，例如我的就是：
   #https://github.com/Thomas-b-programmer/djangoProject_for_ResearchGroup(库的名称).git
   #完整命令
   git remote add origin https://github.com/Thomas-b-programmer/Github-tutorial.git
   ```

=======
   #例如我的就是
   #https://github.com/Thomas-b-programmer/djangoProject_for_ResearchGroup(库的名称).git
   
   git remote add origin https://github.com/Thomas-b-programmer/ResearchGroup_web.git
   ```

​		如果本地远程仓库origin指向的是一个不存在的github仓库地址，需要修改的话可以使用以下命令:

```
#修改本地仓库指向github地址
git remote set-url origin https://github.com/Thomas-b-programmer/ResearchGroup_web.git
```

​		git remote set-url origin <new-url>

​		其中，`<new-url>`是您需要修改为的正确地址。然后再尝试使用第七步的命令进行推送

>>>>>>> 3f36f7f03e5a57d584c948afa41f9bf597a469c9
7. 将本地仓库中的代码推送到远程仓库中，执行以下命令：

   ```
   #git push origin 分支名
<<<<<<< HEAD
   #完整命令
   git push -u origin master
   ```

		此时，你的 Django 项目文件夹应该已经被推送到了 GitHub 远程仓库中啦。你可以在 GitHub 上查看和管理你的代码，
		
		我希望这篇文章能够为你提供一些帮助，帮助你在成为一名顶尖程序员的道路上迈出一小步，如果您觉得这个文章对您有帮助或者让您感到开心，请不要吝啬您的赞哟，这将是我最好的鼓励和支持。我也欢迎您留下您的宝贵意见和建议，以便在今后的创作中不断进步。谢谢大家的支持！
=======
   git push -u origin master
   ```

​		此时，你的 Django 项目文件夹应该已经被推送到了 GitHub 远程仓库中。你可以在 GitHub 上查看和管理你的代码。

# 4.细讲上面的步骤

* **安装 Git 可以按照以下步骤进行：**

  1. 在 Git 官网下载适用于你的操作系统的 Git 安装包，例如 Windows 或 macOS 系统。

  2. 安装 Git。在 Windows 操作系统中，双击下载的 Git 安装包，按照提示进行安装即可。在 macOS 操作系统中，双击下载的 dmg 文件，将 Git 拖动到“应用程序”文件夹中即可完成安装。

  3. 配置 Git。安装完成后，打开终端或 Git Bash（Windows 系统），输入以下命令来配置 Git：

     ```
     git config --global user.name "Your Name"
     git config --global user.email "your_email@example.com"
     ```

     这里的 `"Your Name"` 和 `"your_email@example.com"` 分别为你的用户名和邮箱地址，将它们替换为你自己的即可。这些信息将用于标识你提交的代码的作者。

* **在终端或命令行窗口中输入以下命令来检查 Git 是否已经安装和配置**：

  1. 检查 Git 是否已经安装：

     ```
     git --version
     ```

     如果 Git 已经安装，则会显示 Git 的版本号，例如：`git version 2.33.0`.

  2. 检查 Git 是否已经配置用户名和邮箱：

     ```
     git config --global user.name
     git config --global user.email
     ```

     如果输出了你的用户名和邮箱地址，则说明 Git 已经配置完成。如果没有输出，则说明你还需要配置用户名和邮箱。则需要执行上面配置Git步骤。

* **在本地计算机上创建一个本地仓库**

  1. 第一种：打开终端或命令行窗口，进入要存储代码的目录：使用 `cd` 命令进入要存储代码的目录。例如，如果要将代码存储在 `~/Documents/project` 目录下，则可以使用以下命令：

     ```
     cd ~/Documents/project
     ```

     第二种（推荐）：右击文件夹并选择“Git Bash Here”或“Open PowerShell window here”等选项，可以在所选目录下打开 Git Bash 或 PowerShell 窗口，进而执行 Git 命令。这样可以避免在命令行窗口中手动输入路径的步骤，提高操作效率。但是，这种方法需要先安装 Git Bash 或 PowerShell 等软件，否则无法使用。

  2. 初始化 Git 仓库：使用 `git init` 命令初始化 Git 仓库。这将在当前目录（项目群的根目录)创建一个 `.git` 目录，用于存储 Git 仓库的元数据和对象。

     ```
     git init
     ```

  3. 添加代码到本地仓库：使用 `git add` 命令将代码添加到本地仓库的暂存区中，这些文件并不会立即被提交到 Git 仓库中，而是等待下一次提交操作。。例如，如果要添加所有代码文件，则可以使用以下命令：

     ```
     git add .
     ```

     在执行 `git add` 命令时，Git 会将当前目录下的所有文件和子目录都添加到暂存区中，包括被删除的文件或被修改的文件等。如果你只想添加某个文件，可以在命令中指定文件的路径。

     ```
     git add my-project/index.html
     ```

     常见报错：warning: in the working copy of 'django_Curriculum_Design/.idea/inspectionProfiles/Project_Default.xml', LF will be replaced by CRLF the next time Git touches it
     解决办法：在bush输入`$ git config --global core.autocrlf true`这会自动将换行符从 LF 转换为 CRLF，并在检出时将其转换回 LF。这将帮助确保文件中的换行符与操作系统的默认设置一致，并减少潜在的行尾问题。

  4. 提交代码到本地仓库：使用 `git commit` 命令将代码提交到本地仓库中。需要为提交添加一条提交信息，描述本次提交的修改内容。例如：

     ```
     git commit -m "Initial commit"
     ```

     这将创建一个新的提交，包含添加到暂存区的所有文件。

     `commit message` 表示本次提交的提交信息。这个信息可以是任何你觉得有意义的描述，例如：

     ```
     git commit -m "Add  file to project"
     ```

     这个提交信息表明本次提交是将 `index.html` 文件添加到项目中。这条提交信息对于以后回顾项目历史记录和了解每次修改所做的更改非常重要。

     在 Git 中，本地仓库是存储版本控制历史记录的地方，每一次提交都会将更改记录在本地仓库中。因此，`git commit` 命令会将暂存区中的代码提交到本地仓库中。这样，你就可以在需要时随时从本地仓库中恢复历史版本的代码。

* **本地仓库与 GitHub 远程仓库连接**

  具体操作步骤如下：

  1. 在 GitHub 上创建一个新的代码仓库。
     - 打开 GitHub 网站，登录账号。
     - 点击页面右上角的加号图标，选择 "New repository" 创建新的仓库。
     - 输入仓库名称、描述等信息，选择公开或私有，然后点击 "Create repository" 完成创建。
  2. 将本地仓库中的代码添加到 GitHub 远程仓库中。
     - 打开本地仓库所在的文件夹，在该文件夹中打开命令行窗口或者 Git Bash。
     - 输入 `git remote add origin <remote repository URL>`，其中 `<remote repository URL>` 是刚才在 GitHub 上创建的代码仓库的地址。例如：`git remote add origin https://github.com/Thomas-b-programmer/-.git`
     - 输入 `git push -u origin master`，其中 `-u` 参数用于将本地仓库的分支与远程仓库的分支关联起来，`origin` 是连接的名称，`master` 是本地仓库中的主分支名称。
     - 当你创建一个新的 Git 仓库时，Git 会自动创建一个名为 master 的主分支。你可以在 master 分支上进行开发，并将你的代码提交到该分支中。如果你希望创建一个新的分支，可以使用 `git branch` 命令创建一个新分支，并使用 `git checkout` 命令切换到该分支。或者直接在github上面创建是的，在你的项目页面中，点击上方的 "Branch: main" 按钮，输入你要创建的新分支的名称，然后点击 "Create branch" 即可创建新分支。
  3. 在 GitHub 上查看和管理代码。
     - 打开 GitHub 网站，进入刚才创建的代码仓库页面。
     - 可以在页面上查看代码、提交历史记录、拉取代码等操作。

# 5 github常见操作

### 1.清空github的库

* 在 Github 上清空一个仓库，需要进行以下步骤：

  1. 进入需要清空的仓库的页面。
  2. 点击 "Settings" 选项卡。
  3. 向下滚动，找到 "Danger Zone" 区域。
  4. 点击 "Delete this repository" 按钮。
  5. 输入仓库名称，再次确认删除操作。

  请注意，删除仓库将永久删除该仓库及其所有内容，包括代码、分支、标签、提交、问题、合并请求等，不可恢复。如果您不确定是否要删除，请先备份您的仓库内容。

## 2.查看当前已经添加到本地仓库的文件列表：

* 你可以使用以下命令来查看当前已经添加到本地仓库的文件列表

  ```
  git ls-files
  ```


### 3. 把文件从本地仓库移除

* 有时候已经把文件放入本地仓库了（已经指定了githubd仓库地址），但是你突然,想换一个github仓库上传，可以选着输入一下命令

  ```
  #查看本地仓库已经存放了哪些文件
  git ls-files
  
  #强制移除根目录
  git rm -r djangoProject_for_ResearchGroup
  #强制移除指令
  git rm -rf djangoProject_for_ResearchGroup(文件名字)
  ```

  你需要进入子仓库目录，执行 `rm -rf .git` 命令将子仓库的 `.git` 目录删除，然后再回到父仓库目录，再次执行 `git add .` 命令即可重新将不包含 `djangoProject_for_ResearchGroup` 目录的工作区内容添加到暂存区中。

### 4.文件的状态从暂存改为未追踪

* ```
  git reset
  #或者
  git reset djangoProject_for_ResearchGroup
  ```

* 可以使用 `git status` 命令来查看暂存区中的文件状态，被修改但未暂存的文件会被列在 "Changes not staged for commit" 中，而已经暂存的文件会被列在 "Changes to be committed" 中。如果想要查看具体哪些文件被暂存，可以在 `git status` 命令的输出中找到 "Changes to be committed" 部分，其中会列出被暂存的文件路径

### 5.代码与远程仓库不同步

* 本地的代码与远程仓库不同步。你可以先执行以下命令将远程仓库的变更拉取到本地：

  ```
  git pull origin master
  ```

  如果有冲突需要手动解决。然后再执行 `git push` 将本地代码推送到远程仓库。

  如果报错，通常是因为本地仓库和远程仓库的历史不一致所导致的，你可以尝试添加一个`--allow-unrelated-histories`选项，强制合并两个仓库的历史记录。

  ```
  git pull --allow-unrelated-histories origin master
  ```

  
>>>>>>> 3f36f7f03e5a57d584c948afa41f9bf597a469c9
