# Clone a git repository and retain directory structure

Simple but handy if you want to keep your source tree in a tidy structure.

Before:

    user@host:~/ $ git clone https://scm.com/repo.git
    Cloning into 'repo'...

After:

    user@host:~/ $ git dolly https://scm.com/repo.git
    Cloning into '/home/user/src/scm.com/repo'...

_Disclaimer: no sheep was harmed while making this clone tool._
