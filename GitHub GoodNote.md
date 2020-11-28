
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

git config --global alias.co commit
git config --global alias.lg "log --color --graph --all --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --"

#基本操作
pwd				            顯示路徑
mkdir "Name"			    新增資料夾
git init			        初始化
git help init			    取得說明
git status			        取得未被追蹤的資料
git add "File"		    	追蹤檔案 (Working Directory -> Staging area)
git reset "File"		    取消追蹤檔案(Staging area -> Working Directory)
git diff --cached		    查看存於Staging Area的檔案內容
git commit			       將檔案存入 (Staging Area -> Repository)
git log				        顯示Commit Messenge
git commit -a 			    輸送帶 (Working Directory -> Staging Area -> Repository)
git show "revision"		    顯示版本差異 (Working Directory & Repostitory "Ver")
git diff			        顯示版本差異 (Working Directory & Staging Area)
git checkout "revision"		將檔案回朔至revision版本
git reset --hard ^HEAD		刪除最新版本
( git stash			        暫存 )

#連上GitHub
git remote add origin		連上GitHub
git remote -v			    確認連線
git remote show origin		確認伺服器
git push -u origin master	上傳!

#從GitHub上下載
git clone "SSH" "New Name"	下載!
git pull			        更新本地資料