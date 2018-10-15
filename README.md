#huong dan git

---------------------------------------------- -----
#Thiet lap ban
$ git config --global user.name "<username>"
$ git config --global user.email "<mail address>"

#Note: --global is used for the whole system. You will only be able to customize your file

#Thiet lap editor
$ git config --global core.editor

#Phan mem so su change
$ git config --global merge.tool vimdiff

# soon to be out of git
$ git config --global color.ui auto

#Check the picture
$ git config --list
$ git config {key}

#tro help
$ git help <verb>
$ git <verb> --help
$ man git - <verb>

---------------------------------------------- ----
# I do not regret git
$ git init

# snooping on git
$ git clone [url]
---------------------------------------------- -
#Feel the page
$ git status

#Remove new messages after commit before
$ git add <file>
$ git add.

#command changed
$ git commit -m ""
 
-Them -a commit commits through git add

#Please change your name
$ git log
---------------------------------------------- ---
#Bo pass the information according to the state
$ git rm --cached <file>
#Bo pass the news .gitignore
#Note: The .gitignore file

- Dong or "#" will be over
- There is a state of "/" to make a collection
- Do not follow the message "*"
- The state of the problem "!" in advance
--------------------------------
#Vi Du

# a comment - This line is ignored
# do not track file with .a extension
* .a
# but follow up the lib.a file, although you are ignoring all the .a files above
lib.a
# ignores the TODO file at the root, not subdir / TODO subdirectories
/ TODO
# ignore all files in the build /
build /
# ignore doc / notes.txt, not doc / server / arch.txt
doc / * .txt
# ignores all .txt files in the doc /
doc / ** / * .txt

------------------------------
Check the changes
$ git diff
$ git diff --cached
----------------------------------------------
#disclaimer
$ git rm <file>

#Di file transfer, the file can not be used git add hybrid
$ git mv file_from file_to

------------------------------------------------
#Sign a commit
$ git log

-p: show content changes
--word-diff: see the change of language
--stat: see change in tom tat

$ git log --pretty = oneline

"Oneline" is short, full, and fuller

$ git log --pretty = format:% h -% an,% ar:% s "

% H The hash of the commit
% h The hash code of the commit is more concise
% T The hash tree displays
% t The hash tree shows a more concise tree
% P The root hash
% p The root hash is short
% an Name of the author
% ae E-mail author
% ad Date "author" (format is similar to choice --date =)
% ar Date author, relative
% cn Commissor name
% ce Commer email
% cd On commit
% cr On commit, relative
% s Owner
---------------------------------------------- ----
-p Displays a patch with each commit.
--word-diff Displays a patch in the word format.
--stat Shows the statistics of the edited files in each commit.
--shortstat Show only changes / additions / deletes with the --stat command.
--name-only Displays the list of files that have changed after the commit's information.
--name-status Displays affected files with information such as new add / edit / delete.
--abbrev-commit Show only the first few characters of the SHA-1 hash instead of 40.
--relative-date Displays the date in relative format (for example, "2 weeks ago") instead of the full format.
--graph Displays ASCII histogram of branch and history along with other output information.
--pretty Show commits using a different format. Options include oneline, short, full, fuller and format (allowing you to use custom formats).
--oneline A short, handy option for --pretty = oneline --abbrev-commit.
 
# change password
$ git log --since = 2.weeks

- (n) Only show the latest commit
--since, --after Limit commits made after a certain date.
--until, --before Limit commits made before a certain date.
--author Show only commit that the author name meets certain conditions.
--committer Show only commits whose name matches certain conditions.
---------------------------------------------- --------------------------
# Phuc hoi
