#  1.上传本地文件到Github库的基本步骤：

* **下面仅供了解，具体命令行代码在后面，如果时间紧迫，下面可以不看，直接跳到第一步**

1. 注册一个 GitHub 账号：如果你还没有 GitHub 账号，你需要先注册一个。前往 GitHub 官网，点击“Sign up”按钮，填写必要信息并创建账号。
2. 创建一个新仓库：登陆 GitHub 后，点击右上角的“+”号，然后选择“New repository”来创建一个新仓库。填写仓库名称、描述等信息，并选择仓库类型（公开或私有）。
3. 在本地计算机上设置 Git：Git 是一个版本控制工具，你需要在本地计算机上安装并设置 Git，才能使用 GitHub。你可以在 Git 官网上下载 Git。
4. 在本地计算机上创建一个本地仓库：使用 Git 在本地计算机上创建一个本地仓库，作为代码的存储和版本控制。
5. 将本地仓库与 GitHub 远程仓库连接：使用 Git 将本地仓库与 GitHub 远程仓库进行连接。你需要将本地仓库的内容推送到远程仓库，才能在 GitHub 上查看和管理代码。
6. 使用 Git 进行版本控制：使用 Git 进行代码的版本控制。通过 Git 命令，你可以将代码提交到本地仓库，并进行版本回退、分支管理等操作。
7. 在 GitHub 上管理代码：在 GitHub 上，你可以查看、编辑、删除代码，管理分支、合并请求、Issues等。你可以通过网页界面或命令行工具进行管理。

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

   ```
   git init
   ```

3. 将 Django 项目文件夹添加到本地仓库中，执行以下命令：

   ```
   git add django_project/
   #或者输入
   git add .
   ```

   使用 `git add` 命令将代码添加到本地仓库的暂存区中，这些文件并不会立即被提交到 Github 仓库中，而是等待下一操作,将本地仓库与远程仓库进行关联。

4. 将当前工作目录中的更改保存到本地代码仓库中，执行以下命令：

   ```
   git commit -m "Initial commit"
   ```

5. 在 GitHub 上创建一个新的远程仓库，获取复制该仓库的 SSH 或 HTTPS 链接。

6. 将本地仓库与远程仓库进行关联，执行以下命令：

   ```
   git remote add origin <远程仓库链接>
   #<远程仓库链接>就是你刚才复制的仓库的 SSH 或 HTTPS 链接，例如我的就是：
   #https://github.com/Thomas-b-programmer/djangoProject_for_ResearchGroup(库的名称).git
   #完整命令
   git remote add origin https://github.com/Thomas-b-programmer/Github-tutorial.git
   ```

7. 将本地仓库中的代码推送到远程仓库中，执行以下命令：

   ```
   #git push origin 分支名
   #完整命令
   git push -u origin master
   ```

		此时，你的 Django 项目文件夹应该已经被推送到了 GitHub 远程仓库中啦。你可以在 GitHub 上查看和管理你的代码，
		
		我希望这篇文章能够为你提供一些帮助，帮助你在成为一名顶尖程序员的道路上迈出一小步，如果您觉得这个文章对您有帮助或者让您感到开心，请不要吝啬您的赞哟，这将是我最好的鼓励和支持。我也欢迎您留下您的宝贵意见和建议，以便在今后的创作中不断进步。谢谢大家的支持！
