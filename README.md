Sub Module Parent
resource: https://techmaster.vn/posts/36659/tai-su-dung-code-cho-nhieu-project-voi-git-submodules

git submodule add https://github.com/DucMinhNgo/sub-module-child-1
git submodule add https://github.com/DucMinhNgo/sub-module-child-2

# add sub and rename
git submodule add https://github.com/DucMinhNgo/sub-module-child-1 src/library

# Remove subtree
git rm -rf my-library
rm -rf .git/modules/my-library