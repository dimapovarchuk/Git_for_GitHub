# Git_for_GitHub

Git - login to GitHub via SSH Key 

SSH key generation 
ssh-keygen 
cat ~/.ssh/id_rsa.pub  
 
#To change https on ssh for access (Code) 
git remote -v 
origin	https://github.com/dimapovarchuk/git_test.git (fetch) 
origin	https://github.com/dimapovarchuk/git_test.git (push) 
 
git remote set-url origin git@github.com:dimapovarchuk/git_test.git  
 

Git - configuration .gitconfig 
 

git config --global user.name "Dima Povarchuk" 

git config --global user.email "povarchukdima007@gmail.com" 

git config -l 
 

Output 

 <img width="322" alt="image" src="https://user-images.githubusercontent.com/52627259/223723964-2c592a0c-6262-46f1-aa50-af4c8e198dcc.png">

 
Git - work with local repository 

git init 
git add . 
git status  
git commit -m "Comments" 
 
 <img width="389" alt="image" src="https://user-images.githubusercontent.com/52627259/223724177-b67eaf9a-491d-4a78-9078-d23b92c02302.png">


Git - change history, .gitignore, file restoring 

git log 
git log -p 
git log -p -1 
git diff --staged 
git checkout -- file.txt 
 
<img width="352" alt="image" src="https://user-images.githubusercontent.com/52627259/223724320-96ce59a0-07f4-4f82-9242-28dbd048a862.png">
 

Git - upload project to GitHub 

git clone 
git push origin 
 
<img width="337" alt="image" src="https://user-images.githubusercontent.com/52627259/223724396-adc61034-a5da-4979-a9cf-e25d746d3bdd.png">
 

Git - Branch 

git branch 
git branch test 
git checkout test 
#or 
git checkout -b test 

<img width="332" alt="image" src="https://user-images.githubusercontent.com/52627259/223724518-ddbd3811-23e0-431b-b40a-a8423c59f4d4.png">

<img width="349" alt="image" src="https://user-images.githubusercontent.com/52627259/223724588-39ee9cfe-5f2b-4616-9f31-3e434be9b34d.png">
 
#Merge  
git checkout main 
git megre test 
 
 <img width="335" alt="image" src="https://user-images.githubusercontent.com/52627259/223724669-d2f9f343-158a-476f-b5ea-886f8857af03.png">
 
<img width="343" alt="image" src="https://user-images.githubusercontent.com/52627259/223724745-eb35a5c3-318d-4a84-abdf-d3d658c5c76e.png">

 
#Delete branch 
git branch -d test 
#If branch is not merged 
git branch -D test 

 <img width="349" alt="image" src="https://user-images.githubusercontent.com/52627259/223724838-312a88e9-538c-4eee-ada0-0084c8b9cdd7.png">
 

Git - return to previous version 

git log 
git log checkout 1ba4 
git chechout main 

 <img width="364" alt="image" src="https://user-images.githubusercontent.com/52627259/223724964-6c29dee9-f62d-47ff-a13e-928a6cfadf04.png">
 
 
#Delete commits 
git reset --hard HEAD~2 
 
#Delete commit logs 
git reset --soft HEAD~3 
 
#To change last commit  
git commit --amend 
 
<img width="361" alt="image" src="https://user-images.githubusercontent.com/52627259/223725034-d18d7c8b-4f99-4a60-b7e2-74412d8c24e9.png">
 

Git and GitHub - full working cycle 

git clone git@github.com:dimapovarchuk/git_test.git 
git checkout -b dimapovarchuk777 
git push origin 
git push --set-upstream origin dimapovarchuk777 
 

 <img width="360" alt="image" src="https://user-images.githubusercontent.com/52627259/223725151-cc3d4de8-ca1e-46cb-ae97-152d8aa51f1a.png">


 
git checkout main 
git branch -d dimapovarchuk777 
git push origin --delete dimapovarchuk777 
 

 <img width="326" alt="image" src="https://user-images.githubusercontent.com/52627259/223725225-13c11465-cb10-4606-82fd-bbd4a9adb648.png">
 

Git - tags on GitHub 

git tag 
git tag v1.0.0 
git tag -a v1.2.0 7h54f 
git push origin v1.0.0 
 
git chechout v2.0.0 
 
git tag -d v1.1.1 
git push origin --delete v1.1.1 
 
git log --pretyy=online 

 
