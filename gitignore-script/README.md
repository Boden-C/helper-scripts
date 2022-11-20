## GitIgnore Script
This is to be used with the project to submit the tar file of git

To be used in bash, verion alpha - untested

```
cd ~/.config
mkdir git
cd ~/Merlin/M2222-10\ \(01\)\ Recursion/
git init
echo !!!!! NOTE - The next section will create the gitignore file for extraneous files. If you want a log before the extraneous, commit before this and remove the files later.
touch .gitignore
echo *~ >> .gitignore
echo "\#*\#" >> .gitignore
echo .merlin/ >> .gitignore
echo .merlin0/ >> .gitignore
echo .build/ >> .gitignore
echo !!!!! NOTE - The next line will copy this .gitignore file to become global. If you do not want this, remove the next line.
cp .gitignore /.config/git/ignore
git add .
git commit -m "initial commit"
```
There should be change to be seen, so rewrite the code now and commit whenever you feel there should be an update.

The gitignore file should ignore any future extraneous files.

When you want to commit, do
```
git add .
git commit -m "insert commit message here"
```

When you are done and want to zip the .git, use the commands below and you can dowload the zip from your website at 
www.codermerlin.com/users/your-username/Digital%20Portfolio/M2222.tar.gz
```
tar -czvf M2222-10.tar.gz .git
cp M2222.tar.gz ~/Digital\ Portfolio/M2222.tar.gz
chmod -R a+rx ~/Digital\ Portfolio
```

Remove the file later if you don't want it in your portfolio
```
rm ~/Digital\ Portfolio/M2222.tar.gz
```
