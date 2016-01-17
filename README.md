Push to user github page
1. Add build_folder to git

    $ git add build_folder; git commit -a

2. Push subtree

    $ git subtree push --prefix build_folder origin gh-pages

3. If gh-pages branch already exists, use below command to overwrite

    $ git push origin `git subtree split --prefix build_folder master`:gh-pages --force
