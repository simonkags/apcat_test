Welcome to Git (version 1.8.1.2-preview20130201)


Run 'git help git' to display the help index.
Run 'git help <command>' to display help for specific commands.
strato-g@STRATO-G-PC ~
$ pwd
/c/xampp/htdocs/clients
strato-g@STRATO-G-PC ~
$ ls
+HM_tax_return_website                      makgooglehome
+Jimat                                      musendo
+applicatalyst                              ospaces
+aturistica                                 pass all.txt
+hartman_house                              pbr
+lendme                                     propertygonemobi
+letstalk                                   ps.txt
+marriagecentre                             quotes
B2C                                         setting up on outlook.txt
IMG_21112011_170500.png                     sms gateway.xlsx
Setting Up An Email Account On Outlook.pdf  standard_template_common.css
Works 151012.xlsx                           standard_template_indexfile.html
_git                                        strato-g_creative
acestar                                     strato-g_uk
apcat_test                                  strato-g_zim
backup_tabes_write_to_db.php                strato_g_uk-SEO.ppt
dataform builder                            strato_g_uk.ppt
db_form_builder2                            swagg_nation
f                                           test
findaquote                                  vebraclients.txt
homes2let                                   vebraproperties.txt
homes2leterror_log.txt                      viyex
iafrican                                    xls2sql-full
invoices                                    xls_functions.xls
jjt                                         zepad
jtp                                         zimble
strato-g@STRATO-G-PC ~
$ rm apcat_test/
rm: `apcat_test' is a directory
strato-g@STRATO-G-PC ~
$ git clone git@github.com:simonkags/apcat_test.git
fatal: destination path 'apcat_test' already exists and is not an empty director
y.
strato-g@STRATO-G-PC ~
$ rm -rf apcat_test
strato-g@STRATO-G-PC ~
$ git clone git@github.com:simonkags/apcat_test.git
Cloning into 'apcat_test'...
The authenticity of host 'github.com (204.232.175.90)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,204.232.175.90' (RSA) to the list of know
n hosts.
Enter passphrase for key '/c/xampp/htdocs/clients/.ssh/id_rsa':
Enter passphrase for key '/c/xampp/htdocs/clients/.ssh/id_rsa':
Enter passphrase for key '/c/xampp/htdocs/clients/.ssh/id_rsa':
Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
strato-g@STRATO-G-PC ~
$ git clone https://github.com/simonkags/apcat_test.git
Cloning into 'apcat_test'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (3/3), done.
strato-g@STRATO-G-PC ~
$ cd apcat_test/
strato-g@STRATO-G-PC ~/apcat_test (master)
$ GIT STATUS
fatal: cannot handle STATUS.exe internally
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git status
# On branch master
nothing to commit, working directory clean
strato-g@STRATO-G-PC ~/apcat_test (master)
$ ls
README.md
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git status
# On branch master
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#       modified:   README.md
#
no changes added to commit (use "git add" and/or "git commit -a")
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git commit -am 'new test'
[master 8ff4daf] new test
 1 file changed, 3 insertions(+), 1 deletion(-)
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git status
# On branch master
# Your branch is ahead of 'origin/master' by 1 commit.
#   (use "git push" to publish your local commits)
#
nothing to commit, working directory clean
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git push
warning: push.default is unset; its implicit value is changing in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the current behavior after the default changes, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': simon@applicatalyst.com
Password for 'https://simon@applicatalyst.com@github.com':
Counting objects: 5, done.
Writing objects: 100% (3/3), 274 bytes, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/simonkags/apcat_test.git
   cfcc9ef..8ff4daf  master -> master
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git pull
Already up-to-date.
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git checkout -b new_feature
Switched to a new branch 'new_feature'
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git branch -a
  master
* new_feature
  remotes/origin/HEAD -> origin/master
  remotes/origin/master
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git status
# On branch new_feature
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#       modified:   README.md
#
no changes added to commit (use "git add" and/or "git commit -a")
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git commit -am @new feature complete@
fatal: Paths with -a does not make sense.
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git commit -am 'new feature complete'
[new_feature 72185f1] new feature complete
 1 file changed, 3 insertions(+), 1 deletion(-)
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git push origin new_feature
Username for 'https://github.com': simon@applicatalyst.com
Password for 'https://simon@applicatalyst.com   @github.com':
fatal: Authentication failed
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git push origin new_feature
Username for 'https://github.com': simon@applicatalyst.com
Password for 'https://simon@applicatalyst.com@github.com':
Counting objects: 5, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 296 bytes, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/simonkags/apcat_test.git
 * [new branch]      new_feature -> new_feature
strato-g@STRATO-G-PC ~/apcat_test (new_feature)
$ git checkout master
Switched to branch 'master'
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git merge new_feature
Updating 8ff4daf..72185f1
Fast-forward
 README.md | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git status
# On branch master
# Your branch is ahead of 'origin/master' by 1 commit.
#   (use "git push" to publish your local commits)
#
nothing to commit, working directory clean
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git push
warning: push.default is unset; its implicit value is changing in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the current behavior after the default changes, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': simon@applicatalyst.com
Password for 'https://simon@applicatalyst.com@github.com':
Total 0 (delta 0), reused 0 (delta 0)
To https://github.com/simonkags/apcat_test.git
   8ff4daf..72185f1  master -> master
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git branch -D new_feature
Deleted branch new_feature (was 72185f1).
strato-g@STRATO-G-PC ~/apcat_test (master)
$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/master
  remotes/origin/new_feature
strato-g@STRATO-G-PC ~/apcat_test (master)
$