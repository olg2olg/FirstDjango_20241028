#--------------------------------------------------------------
#0) Зарегистрироваться на github


#--------------------------------------------------------------
#1)установить на ОС linux
sudo apt install git
git --version
    git version 2.43.0

#--------------------------------------------------------------
#2)Работа
git init
    hint: Using 'master' as the name for the initial branch. This default branch name
    hint: is subject to change. To configure the initial branch name to use in all
    hint: of your new repositories, which will suppress this warning, call:
    hint: 
    hint: 	git config --global init.defaultBranch <name>
    hint: 
    hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
    hint: 'development'. The just-created branch can be renamed via this command:
    hint: 
    hint: 	git branch -m <name>
    Initialized empty Git repository in /home/user/Projects/FirstDjango/.git/

git config --global user.name "olg2olg"
git config --global user.email "olga17573@gmail.com"
git config --list
    user.name=olg2olg
    user.email=olga17573@gmail.com
    core.repositoryformatversion=0
    core.filemode=true
    core.bare=false
    core.logallrefupdates=true
git add .
git commit -m "Day1-Dz"
    [master (root-commit) 4929eda] Day1-Dz
    17 files changed, 344 insertions(+)
    create mode 100644 .gitignore
    create mode 100644 FirstDjango/__init__.py
    create mode 100644 FirstDjango/asgi.py
    create mode 100644 FirstDjango/settings.py
    create mode 100644 FirstDjango/urls.py
    create mode 100644 FirstDjango/wsgi.py
    create mode 100644 MainApp/__init__.py
    create mode 100644 MainApp/admin.py
    create mode 100644 MainApp/apps.py
    create mode 100644 MainApp/migrations/__init__.py
    create mode 100644 MainApp/models.py
    create mode 100644 MainApp/tests.py
    create mode 100644 MainApp/views.py
    create mode 100644 README.md
    create mode 100644 README_Git.txt
    create mode 100755 manage.py
    create mode 100644 requirements.txt

ssh-keygen -o
    Generating public/private ed25519 key pair.
    Enter file in which to save the key (/home/user/.ssh/id_ed25519):           
    Enter passphrase (empty for no passphrase): 
    Enter same passphrase again: 
    Your identification has been saved in /home/user/.ssh/id_ed25519
    Your public key has been saved in /home/user/.ssh/id_ed25519.pub
    The key fingerprint is:
    SHA256:OQRFwr+TqRjsgkRindQWC6peS+ECq4Od5EVHc+0NDv0 user@usercomp
    The key's randomart image is:
    +--[ED25519 256]--+
    |   ..o*o+o       |
    |  ...+o=. +      |
    |..o.+....+ +     |
    |++.+.. ...o E    |
    |*..=.   S+       |
    |+=+o+   =.       |
    |=o+o o . .       |
    |... o .          |
    |   .             |
    +----[SHA256]-----+   
ls ~/.ssh
    authorized_keys  id_ed25519  id_ed25519.pub
#cat ~/.ssh/id_rsa.pub
cat ~/.ssh/id_ed25519.pub 
   ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIH6rD8Y7YLrHH8XcJNEGMHVFbLXA5xta85ZNhajDADBj user@usercomp


git add FirstDjango/urls.py MainApp/views.py README.md README_Git.txt 
git commit -m "Day1-Dz"
    [master cf690d3] Day1-Dz
    4 files changed, 98 insertions(+), 31 deletions(-)

git remote add origin git@github.com:olg2olg/FirstDjango_20241028.git
git push -u origin master

git add .
git commit -m "Done.Day1.Module1.Task3"
git push
#--------------------------------------------------------------
#3) все удалить
rm -rf .git
#--------------------------------------------------------------
#4) высвинивание для проваерки
mkdir Studens
cd $_  #=== cd Studens/HodylevaO
git clone https://github.com/olg2olg/*****  FirstDjango  

source ~/Students/FirstDjango/django_venv/bin/activate
python manage.py runserver
#--------------------------------------------------------------
#--------------------------------------------------------------
#--------------------------------------------------------------
https://github.com/olg2olg/python3Django

ssh   git@github.com:olg2olg/python3Django.git

…or create a new repository on the command line
    echo "# python3Django" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin git@github.com:olg2olg/python3Django.git
    git push -u origin main

…or push an existing repository from the command line
git remote add origin git@github.com:olg2olg/FirstDjango_20241028.git
git branch -M main
git push -u origin main
