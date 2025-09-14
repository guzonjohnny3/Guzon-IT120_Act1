 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 
$ git config --global user.name "Johnny Guzon" 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 
$ git config --global user.email "guzonjohnny3@gmail.com" 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 
$ git config --list diff.astextplain.textconv=astextplain filter.lfs.clean=git-lfs clean -- %f filter.lfs.smudge=git-lfs smudge -- %f filter.lfs.process=git-lfs filter-process filter.lfs.required=true http.sslbackend=schannel core.autocrlf=true core.fscache=true core.symlinks=false pull.rebase=false credential.helper=manager credential.https://dev.azure.com.usehttppath=true init.defaultbranch=master user.name=Johnny Guzon user.email=guzonjohnny3@gmail.com 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 
$ git init 
Initialized empty Git repository in C:/Users/Admin/Desktop/Guzon_IT120_Act1/.git 
/ 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) $ touch Profile.txt Education.txt Background.txt Readme.txt Test.py 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ echo -e "First Name: Johnny 
> Middle Name: N/A 
> Last Name: Guzon 
> Age: 24 
> Birth Date: December 20, 2000" > Profile.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ echo -e "Elementary School: Salvacion Elementary School 
> Year Graduated: 2013 
> High School: Cabadbaran City National High School 
> Year Graduated: 202" > Education.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ echo "Languages Known: Cebuano, Tagalog, Engliah, Portugues, Spanish" > Background.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) $ echo "" > Readme.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ echo -e "import os 
> print('Hello, World')" > Test.py 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ git add . 
warning: in the working copy of 'Background.txt', LF will be replaced by CRLF th e next time Git touches it warning: in the working copy of 'Education.txt', LF will be replaced by CRLF the  next time Git touches it warning: in the working copy of 'Profile.txt', LF will be replaced by CRLF the n ext time Git touches it warning: in the working copy of 'Readme.txt', LF will be replaced by CRLF the ne xt time Git touches it warning: in the working copy of 'Test.py', LF will be replaced by CRLF the next time Git touches it 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ git commit -m "Initial commit with basic files" 
[master (root-commit) 871ebbd] Initial commit with basic files 
 5 files changed, 13 insertions(+)  create mode 100644 Background.txt  create mode 100644 Education.txt  create mode 100644 Profile.txt  create mode 100644 Readme.txt  create mode 100644 Test.py 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ git checkout -b Guzon_B1 
Switched to a new branch 'Guzon_B1' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B1) 
$ echo -e "Birth Place: Butuan City 
> Religion: Members Church of God International (MCGI) 
> Father's Name: Abraham B. Polloso 
> Occupation: Farmer 
> Mother's Name: Juneta M. Guzon 
> Occupation: House Wife" >> Profile.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B1) 
$ git add Profile.txt warning: in the working copy of 'Profile.txt', LF will be replaced by CRLF the n ext time Git touches it 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B1) 
$ git commit -m "Added additional profile information" 
[Guzon_B1 16297f9] Added additional profile information 
 1 file changed, 6 insertions(+) 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B1) 
$ git checkout master 
Switched to branch 'master' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ git checkout -b Guzon_B2 
Switched to a new branch 'Guzon_B2' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B2) 
$ echo -e "College: Caraga State University Cbadbaran City Campus 
> Program: BS Information Technology 
> Year Graduated: 2028 if God's Will" >> Education.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B2) 
$  git add Education.txt warning: in the working copy of 'Education.txt', LF will be replaced by CRLF the  next time Git touches it 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B2) 
$ git commit -m "Added college education info" 
[Guzon_B2 2cff523] Added college education info 
 1 file changed, 3 insertions(+) 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B2) 
$ git checkout master 
Switched to branch 'master' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ git checkout -b Guzon_B3 
Switched to a new branch 'Guzon_B3' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B3) 
$ echo -e "Person to Contact: Maria Fe Guzon 
> Address: Sabang 3, Cabadbaran City 
> Contact Number: 09773936865" >> Background.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B3) 
$ git rm Test.py rm 'Test.py' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B3) 
$ git add Background.txt warning: in the working copy of 'Background.txt', LF will be replaced by CRLF th e next time Git touches it 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B3) 
$ git commit -m "Added contact details and removed Test.py" 
[Guzon_B3 c3a05ea] Added contact details and removed Test.py 
 2 files changed, 3 insertions(+), 2 deletions(-)  delete mode 100644 Test.py 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B3) 
$ git checkout master 
Switched to branch 'master' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (master) 
$ git checkout -b Guzon_B4 
Switched to a new branch 'Guzon_B4' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) $ echo -e "Git Commands Used: 
> 1. git init > 2. git add . 
> 3. git commit -m 'message' 
> 4. git checkout -b branch_name 
> 5. git rm Test.py 
> 6. git push origin branch_name" > Readme.txt 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git rm Test.py rm 'Test.py' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git add Readme.txt warning: in the working copy of 'Readme.txt', LF will be replaced by CRLF the ne xt time Git touches it gi 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git commit -m "Added Git commands to Readme and removed Test.py" 
[Guzon_B4 e5731fd] Added Git commands to Readme and removed Test.py 
 2 files changed, 7 insertions(+), 3 deletions(-)  delete mode 100644 Test.py 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git remote remove origin error: No such remote: 'origin' 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) $ git remote add origin https://github.com/guzonjohnny3/Guzon_IT120_Act1.git 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git push -M master error: unknown switch `M' usage: git push [<options>] [<repository> [<refspec>...]] 
 
    -v, --[no-]verbose    be more verbose 
    -q, --[no-]quiet      be more quiet     --[no-]repo <repository>                           repository 
    --[no-]all            push all branches 
    --[no-]branches       alias of --all 
    --[no-]mirror         mirror all refs 
    -d, --[no-]delete     delete refs 
    --[no-]tags           push tags (can't be used with --all or --branches or - 
-mirror) 
    -n, --[no-]dry-run    dry run 
    --[no-]porcelain      machine-readable output 
    -f, --[no-]force      force updates 
    --[no-]force-with-lease[=<refname>:<expect>] 
                          require old value of ref to be at this value 
    --[no-]force-if-includes                           require remote updates to be integrated locally     --[no-]recurse-submodules (check|on-demand|no)                           control recursive pushing of submodules 
    --[no-]thin           use thin pack 
    --[no-]receive-pack <receive-pack>                           receive pack program     --[no-]exec <receive-pack>                           receive pack program     -u, --[no-]set-upstream                           set upstream for git pull/status     --[no-]progress       force progress reporting 
    --[no-]prune          prune locally removed refs 
    --no-verify           bypass pre-push hook 
    --verify              opposite of --no-verify 
    --[no-]follow-tags    push missing but relevant tags 
    --[no-]signed[=(yes|no|if-asked)] 
                          GPG sign the push 
    --[no-]atomic         request atomic transaction on remote side 
    -o, --[no-]push-option <server-specific>                           option to transmit 
    -4, --ipv4            use IPv4 addresses only     -6, --ipv6            use IPv6 addresses only 
 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git push -u origin master info: please complete authentication in your browser... remote: Repository not found. 
fatal: repository 'https://github.com/guzonjohnny3/Guzon_IT120_Act1.git/' not fo und 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git push -u origin master info: please complete authentication in your browser... remote: Repository not found. 
fatal: repository 'https://github.com/guzonjohnny3/Guzon_IT120_Act1.git/' not fo und 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) 
$ git remote add origin https://github.com/guzonjohnny3/Guzon_IT120_Act1.git error: remote origin already exists. 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (Guzon_B4) $ git branch -M main 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git push -u origin main info: please complete authentication in your browser... remote: Repository not found. 
fatal: repository 'https://github.com/guzonjohnny3/Guzon_IT120_Act1.git/' not fo und 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git removed origin git: 'removed' is not a git command. See 'git --help'. 
 
The most similar command is         remote-fd 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git remote remove origin 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git remote add origin https://github.com/guzonjohnny3/Guzon_IT120_Act1.git 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git branch -M main 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git push -u origin main info: please complete authentication in your browser... 
remote: Repository not found. 
fatal: repository 'https://github.com/guzonjohnny3/Guzon_IT120_Act1.git/' not fo und 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git remote remove origin 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) $ git remove add origin https://github.com/guzonjohnny3/Guzon-IT120_Act1.git git: 'remove' is not a git command. See 'git --help'. 
 
The most similar command is 
        remote 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git remote add origin https://github.com/guzonjohnny3/Guzon-IT120_Act1.git 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git branch -M main 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$ git push -u origin main info: please complete authentication in your browser... 
Enumerating objects: 10, done. 
Counting objects: 100% (10/10), done. Delta compression using up to 4 threads Compressing objects: 100% (8/8), done. 
Writing objects: 100% (10/10), 1010 bytes | 26.00 KiB/s, done. Total 10 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0) remote: Resolving deltas: 100% (1/1), done. 
To https://github.com/guzonjohnny3/Guzon-IT120_Act1.git 
 * [new branch]      main -> main branch 'main' set up to track 'origin/main'. 
 
Admin@DESKTOP-08E71T3 MINGW64 ~/Desktop/Guzon_IT120_Act1 (main) 
$  
 
