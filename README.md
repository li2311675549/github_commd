# github新建文件及上传指令

### 1. 创建一个 README.md 文件，并把github端建立的仓库名写进去
```
echo "# arm_openpi05" >> README.md
```
### 2. 把当前文件夹初始化为 Git 本地仓库
```
git init
```
### 3. 把刚创建的 README 文件添加到准备上传的暂存区（💡提示：如果你本地文件夹里已经有了你写的 Python 脚本或其他代码，请把这句改成 `git add .` ，这样就能把所有文件一起添加了）
```
git add README.md
```
### 4. 提交本次操作，并写一句备注
```
git commit -m "first commit"
```
### 5. 将默认分支名统一设置为 main
```
git branch -M main
```
### 6. 把本地仓库和这个 GitHub 云端仓库连接起来（注意：下面这行已经帮你换成了 SSH 格式的链接）
```
git remote add origin git@github.com:li2311675549/arm_openpi05.git
```
### 7. 正式把本地的东西推送到 GitHub 云端
```
git push -u origin main
```

# 更新github仓库的操作
### 1. 告诉 Git：把当前目录下所有“新增”和“修改”的文件都放到暂存区（准备提交）
```
git add .
```
### 2. 告诉 Git：把刚才放到暂存区的东西打个包，并贴上一张便签（备注）
```
git commit -m "commd"
```
### 3. 告诉 GitHub：把本地的新版本推送到云端保存
```
git push
```
