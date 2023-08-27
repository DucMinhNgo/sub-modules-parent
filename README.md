Sub Module Parent
resource: https://techmaster.vn/posts/36659/tai-su-dung-code-cho-nhieu-project-voi-git-submodules

git submodule add https://github.com/DucMinhNgo/sub-module-child-1
git submodule add https://github.com/DucMinhNgo/sub-module-child-2

# add sub and rename
git submodule add https://github.com/DucMinhNgo/sub-module-child-1 src/library

# Remove subtree
git rm -rf my-library
rm -rf .git/modules/my-library

# Pull
git subtree pull --prefix=./sub-module-child-1 --squash https://github.com/DucMinhNgo/sub-module-child-1 main
git subtree pull --prefix=<folder>/<repo_name> --squash <git_url> <branch>