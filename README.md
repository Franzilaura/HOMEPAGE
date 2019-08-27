# Upload Homepage unter Windows
throw your end user device out of the next window. Especially if its deep - the deeper the better.

see also this [article on ssh on windows](https://www.howtogeek.com/336775/how-to-enable-and-use-windows-10s-built-in-ssh-commands/).


# Upload Homepage unter besser
if interested, backup relevant files via command line commands defined in [`get_old_files.sh`](./get_old_files.sh). Keep in mind, this takes the tutors pictures all in once and the other files only on an item base (so only a selection if there is more). WARNING: Dont try to get the whole folder, in the servers subfolder `old` there is a lot of stuff. DONT!

then execute (assuming you're in directory `orientierungseinheit/homepage`)

    scp -r $(pwd)/ fmtx218@login1.math.uni-hamburg.de:/afs/math.uni-hamburg.de/www/oe
    ssh fmtx218@login1.math.uni-hamburg.de rm /afs/math.uni-hamburg.de/www/oe/get_old_files.sh
    ssh fmtx218@login1.math.uni-hamburg.de rm /afs/math.uni-hamburg.de/www/oe/README.md

Don't forget to change the user name.

TODO: fix scp bug (rather use tar).
