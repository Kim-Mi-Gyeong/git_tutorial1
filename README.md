# git clone 사용

github
1) VSCODE
2) 처음부터 올릴생각 : repo 만들고, git clone해서 커밋

D:\chatbot>git clone https://github.com/Kim-Mi-Gyeong/git_tutorial1.git
Cloning into 'git_tutorial1'...
warning: You appear to have cloned an empty repository.

D:\chatbot>cd git_tutorial1

D:\chatbot\git_tutorial1>git add .

D:\chatbot\git_tutorial1>git commit -m "테스트"
[main (root-commit) 5c63c8f] 테스트
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 "\354\225\204\353\254\264\352\261\260\353\202\230.txt"

D:\chatbot\git_tutorial1>git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 231 bytes | 231.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Kim-Mi-Gyeong/git_tutorial1.git
 * [new branch]      main -> main


3) repo 만들고, 로컬에서 작업한 것을 (갑자기) 연동 : 
 - git inti
 - git remote add 내꺼
 - git branch -M main
 - git add, commit, push

D:\chatbot\git_tutorial1>git init
Reinitialized existing Git repository in D:/chatbot/git_tutorial1/.git/

D:\chatbot\git_tutorial1>git remote add origin https://github.com/Kim-Mi-Gyeong/git_tutorial1.git
error: remote origin already exists.

D:\chatbot\git_tutorial1>git add .

D:\chatbot\git_tutorial1>git commit -m "테스트"
[main ff2783b] 테스트
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename "\354\225\204\353\254\264\352\261\260\353\202\230.txt" => "\353\215\260\354\235\264\354\275\230_\355\227\210\354\234\204\353\247\244\353\254\274.txt" (100%)

D:\chatbot\git_tutorial1>git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 464 bytes | 232.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Kim-Mi-Gyeong/git_tutorial1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

4)  repo 안만들어놓고, 로컬에서 작업한 것을 연동
