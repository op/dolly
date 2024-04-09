# 🐑 Dolly the VCS clone tool

**Dolly** clones repositories with scientific precision. Handy if you want to keep your source tree pristine.

Before:

```bash
user@host:~/ $ mkdir -p /home/user/src/scm.com
user@host:~/ $ git clone https://scm.com/repo.git \
  /home/user/src/scm.com/repo
Cloning into '/home/user/src/scm.com/repo'...
```

After:

```bash
user@host:~/ $ git dolly https://scm.com/repo.git
Cloning into '/home/user/src/scm.com/repo'...
```

## ✨ Features

* 📇 Keep your source tree tidy
* 📦 Clone with a single command
* 🍱 Supports Git and Mercurial (hg)

## ⚡ Requirements

* Git
* Python >= **3.6**

## 📦 Installation

Classic clone:
```bash
$ git clone https://github.com/op/dolly
$ install dolly/dolly /usr/local/bin
```

git:
```bash
# create symlink in PATH (or GIT_EXEC_PATH)
$ ln -s /usr/local/bin/{,git-}dolly
```

Mercurial (hg):
```bash
# add to ~/.hgrc or eg XDG_CONFIG_HOME, see hg help config
cat <<EOF >> $XDG_CONFIG_HOME/hg/hgrc
[alias]
dolly = !/usr/local/bin/dolly $@
EOF
```

## ⚰️ Disclaimer

No sheep was harmed while making this tool. [Dolly], rest in peace!

[Dolly]: https://en.wikipedia.org/wiki/Dolly_(sheep)
