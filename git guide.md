# Getting Started with Git and Github

This guide helps you install and get started with Git and Github.

Using Git is essential for version control and collaboration in software development. It allows multiple developers to work on the same project simultaneously without conflicts and helps track changes over time. GitHub is the premier online Git collaboration platform. Its importance in a personal portfolio lies in showcasing your ability to work collaboratively on projects, giving potential employers or collaborators an insight into your abilities.

# Git Installation

Git is a version control software that lets people keep track of changes to their work and incorporate changes from others easily. It runs on your laptop, and while there are apps that let you manage Git, it's best understood by using the command line.

## Windows

Please download the Git installer from this link:**[https://git-scm.com/download/win](https://git-scm.com/download/win)**. You'll want to select **64-bit Git for Windows Setup**.


![Alt text](image.png)

Run the Git installer.

![Alt text](image-1.png)

The only change you should make from the default installation options is to **"Use Notepad as Git's default editor"**.

![Alt text](image-2.png)


Once Git is installed, make sure you can access the **Git Bash** program. This will be the terminal we will use for the git tutorial.
![Alt text](image-3.png)

## Mac

Please download Homebrew, a program for Mac that makes downloading software development tools easier, by following the instructions at this link: [https://brew.sh](https://brew.sh)

Open a Terminal window, and copy paste the following and run:

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`


This process will prompt for your password, and may install XCode. That is expected. After it completes, it will display something like the following:

```
==> Next steps:
- Run these two commands in your terminal to add Homebrew to your PATH:

    (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/<YOUR USERNAME>/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"

- Run brew help to get started
- Further documentation:
    https://docs.brew.sh
```

Copy the two commands given and run them. This installs Homebrew, which can be accessed by running the `brew` command in the Terminal.

Once Homebrew is installed, please run: `brew install git`. This will install git.

### Can't find Terminal on a Mac?
It'll be under Applications > Utilities > Terminal


# Github Account Setup

We will create a Github account, which will help you use Git to collaborate with other people at Fordham and in the workplace. Github is also a great place to showcase your professional skills.

To create a Github account, go to [Github.com](https://github.com/signup) and click on sign up.

**Some notes**:
* Use an email that you will have consistent access to. Fordham email is good, a professional email is better.
* Your username should reflect you, and be something you're comfortable using in the workplace. Don't have it be something like "funkymonkey123".

Once you've made your Github account, you will need a **Personal Access Token**. This is because Github does not allow password based authentication anymore.

From your GitHub account, go to **Settings → Developer Settings → Personal Access Token → Generate New Token (classic) →** (Give your password) **→** Check all boxes for "repo" and set the Expiration to "No Expiration" **→** click **Generate token → Copy the generated Token**, it will be something like `ghp_sFhFsSHhTzMDreGRLjmks4Tzuzgthdvfsrta`. This is your Github Personal Access Token.

Now follow the below method based on your operating system:

## Windows

Go to Credential Manager from **Control Panel → Windows Credentials → find** `git:https://github.com` **→ Edit →** On Password replace with with your **Github Personal Access Token** →** You are Done

If you don’t find `git:https://github.com` → Click on **Add a generic credential →** Internet address will be `git:https://github.com`. You need to type in your username, and the password will be your **Github Personal Access Token** → Click Ok and you are done.

## MacOS

Temporarily save this password in a secure note location. You will be prompted for it in the Terminal when running commands that interact with Github.

When running commands that interact with Github, you will be asked for your Github username and then your password. Instead of your Github password, use your **Github Personal Access Token**.

---

Once your Github account is setup, run the following commands in your Terminal.

```
git config --global user.name "YOUR GITHUB USERNAME"
git config --global user.email "YOUR GITHUB EMAIL"
```

This associates the commands you run on your computer to your Github account.
