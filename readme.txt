Command line instructions


Git global setup
git config --global user.name "刘婧婷"
git config --global user.email "liujingting@corp.netease.com"

# Create a new repository
git clone ssh://git@g.hz.netease.com:22222/matting/deeplab_v3plus.git
cd deeplab_v3plus
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

Existing folder
cd existing_folder
git init
git remote add origin ssh://git@g.hz.netease.com:22222/matting/deeplab_v3plus.git
git add .
git commit -m "Initial commit"
git push -u origin master

Existing Git repository
cd existing_repo
git remote rename origin old-origin
git remote add origin ssh://git@g.hz.netease.com:22222/matting/deeplab_v3plus.git
git push -u origin --all
git push -u origin --tags
