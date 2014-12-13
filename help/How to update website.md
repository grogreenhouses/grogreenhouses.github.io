**How to update website**

Last login: Wed Dec  3 11:04:04 on ttys001
Edwards-MacBook-Air:~ edwardchan$ ls
AndroidStudioProjects	Desktop			Documents		Dropbox			Movies			Pictures
Applications		Dev			Downloads		Library			Music			Public
Edwards-MacBook-Air:~ edwardchan$ cd Dev
Edwards-MacBook-Air:Dev edwardchan$ ls
Brett				grogreenhouses.github.io
Edwards-MacBook-Air:Dev edwardchan$ cd grogreenhouses.github.io
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ ls
CNAME		README.md	_config.yml	_includes	_posts		_site		combo.css	img		index.html	site.js
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ jekyll serve
Configuration file: /Users/edwardchan/Dev/grogreenhouses.github.io/_config.yml
            Source: /Users/edwardchan/Dev/grogreenhouses.github.io
       Destination: /Users/edwardchan/Dev/grogreenhouses.github.io/_site
      Generating... 
                    done.
 Auto-regeneration: enabled for '/Users/edwardchan/Dev/grogreenhouses.github.io'
Configuration file: /Users/edwardchan/Dev/grogreenhouses.github.io/_config.yml
    Server address: http://0.0.0.0:4000/
  Server running... press ctrl-c to stop.
      Regenerating: 1 files at 2014-12-13 14:38:34 ...done.
      Regenerating: 1 files at 2014-12-13 14:39:12 ...done.
      Regenerating: 1 files at 2014-12-13 14:39:14 ...done.
      Regenerating: 1 files at 2014-12-13 14:39:15 ...done.
      Regenerating: 1 files at 2014-12-13 14:39:17 ...done.
      Regenerating: 1 files at 2014-12-13 14:39:20 ...done.
      Regenerating: 1 files at 2014-12-13 14:40:13 ...done.
      Regenerating: 1 files at 2014-12-13 14:41:15 ...done.
      Regenerating: 1 files at 2014-12-13 14:42:28 ...done.
      Regenerating: 1 files at 2014-12-13 14:43:10 ...done.
      Regenerating: 1 files at 2014-12-13 14:43:11 ...done.
      Regenerating: 1 files at 2014-12-13 14:45:31 ...done.
^CEdwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   _posts/2014-11-14-home.md
	deleted:    _posts/2014-11-14-what-we-do.md
	deleted:    _posts/2014-11-15-product.md
	modified:   _posts/2014-11-16-contact-us.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	_posts/2014-11-14-product.md
	_posts/2014-11-15-past-experience.md
	img/logo.jpeg

no changes added to commit (use "git add" and/or "git commit -a")
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git rm _posts/2014-11-14-what-we-do.md
rm '_posts/2014-11-14-what-we-do.md'
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git rm _posts/2014-11-15-product.md
rm '_posts/2014-11-15-product.md'
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git add _posts/2014-11-14-product.md
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git add _posts/2014-11-15-past-experience.md
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git add img/logo.jpeg
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   _posts/2014-11-14-product.md
	deleted:    _posts/2014-11-14-what-we-do.md
	new file:   _posts/2014-11-15-past-experience.md
	deleted:    _posts/2014-11-15-product.md
	new file:   img/logo.jpeg

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   _posts/2014-11-14-home.md
	modified:   _posts/2014-11-16-contact-us.md

Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git add -u
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   _posts/2014-11-14-home.md
	new file:   _posts/2014-11-14-product.md
	deleted:    _posts/2014-11-14-what-we-do.md
	new file:   _posts/2014-11-15-past-experience.md
	deleted:    _posts/2014-11-15-product.md
	modified:   _posts/2014-11-16-contact-us.md
	new file:   img/logo.jpeg

Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git commit -m "Added Video, Logo, and Content"
[master 8b14c30] Added Video, Logo, and Content
 7 files changed, 39 insertions(+), 32 deletions(-)
 create mode 100644 _posts/2014-11-14-product.md
 delete mode 100644 _posts/2014-11-14-what-we-do.md
 create mode 100644 _posts/2014-11-15-past-experience.md
 delete mode 100644 _posts/2014-11-15-product.md
 create mode 100644 img/logo.jpeg
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ git push -u origin master
Counting objects: 17, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 70.72 KiB | 0 bytes/s, done.
Total 9 (delta 2), reused 0 (delta 0)
To https://github.com/grogreenhouses/grogreenhouses.github.io.git
   f9e3ae3..8b14c30  master -> master
Branch master set up to track remote branch master from origin.
Edwards-MacBook-Air:grogreenhouses.github.io edwardchan$ 
