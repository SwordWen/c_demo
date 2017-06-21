# c_demo

# git command

github: https://github.com/
git remote set-url [--push] <name> <newurl> [<oldurl>]
git remote set-url origin <newurl> [<oldurl>]


git: revert (reset) a single file
This one is hard to find out there so here it is. If you have an uncommitted change (its only in your working copy) that you wish to revert (in SVN terms) to the copy in your latest commit, do the following:
> git checkout filename

This will checkout the file from HEAD, overwriting your change. This command is also used to checkout branches, and you could happen to have a file with the same name as a branch. All is not lost, you will simply need to type:

> git checkout -- filename

You can also do this with files from other branches, and such. man git-checkout has the details.
The rest of the Internet will tell you to use git reset --hard, but this resets all uncommitted changes you’ve made in your working copy. Type this with care.


# gcc commands:

compile src code :
gcc -o ev_timeout  -I ./ sample/ev_timeout.c .libs/libev.a -lm

Macro expansion and Assembly code
gcc sample/ev_timeout.c -I ./ -E


# cmake examples:

CMakeLists.txt : https://cmake.org/examples/

mkdir build && cd build
cmake ..     # Default to Unix Makefiles.
make
make verify  # (optional)

# linux(ubuntu) include folder

/usr/include/x86_64-linux-gnu: sys/epoll.h
/usr/include: stdio.h

# use nc command to connect server
nc ip port : nc 127.0.0.1 8000

# reference

markdown : https://en.wikipedia.org/wiki/Markdown
linux man-pages : https://www.kernel.org/doc/man-pages/
The largest Tutorials Library on the web : https://www.tutorialspoint.com/
