# How-to-install-ripgen-in-Parrotsec-Kali-Ubuntu-Debian-Linux
How to install ripgen in Parrotsec Kali Ubuntu Debian Linux
# apt remove cargo
# apt autoremove
# apt update
# apt-get update
# apt install build-essential
# apt install cargo
# rustc --version
rustc 1.48.0 Same Old Shit Version :-(
rustc 1.48.0 Same Old Shit Version :-(
rustc 1.48.0 Same Old Shit Version :-(
Now do this to get latest rustc verison :-)
# apt remove rustc
# rustc --version
bash: /usr/bin/rustc: No such file or directory
# curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
1) Proceed with installation (default)
2) Customize installation
3) Cancel installation
>1
root@cyberghazi-vmwarevirtualplatform:/# cargo install ripgen
    Updating crates.io index
     Ignored package `ripgen v0.1.3` is already installed, use --force to override
root@cyberghazi-vmwarevirtualplatform:/# cargo install ripgen --force
root@cyberghazi-vmwarevirtualplatform:/# source $HOME/.cargo/env
root@cyberghazi-vmwarevirtualplatform:/# source $HOME/.bashrc  // This is only for bash shell users 
root@cyberghazi-vmwarevirtualplatform:/# source $HOME/.profile

That's It - AlhamdulilAllah

See below for full Process to understand above steps and commands.

root@cyberghazi-vmwarevirtualplatform:/# rustc --version
rustc 1.48.0
root@cyberghazi-vmwarevirtualplatform:/# rustup update
bash: rustup: command not found
root@cyberghazi-vmwarevirtualplatform:/# rustup self uninstall
bash: rustup: command not found
root@cyberghazi-vmwarevirtualplatform:/# apt remove cargo
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  figlet insserv libgit2-1.1 libio-pty-perl libipc-run-perl libmbedcrypto3 libmbedtls12 libmbedx509-0
  lshw-gtk moreutils startpar sysv-rc
Use 'sudo apt autoremove' to remove them.
The following packages will be REMOVED:
  cargo
0 upgraded, 0 newly installed, 1 to remove and 527 not upgraded.
After this operation, 10.6 MB disk space will be freed.
Do you want to continue? [Y/n] Y
(Reading database ... 434684 files and directories currently installed.)
Removing cargo (0.47.0-3+b1) ...
Processing triggers for man-db (2.9.4-2) ...
Scanning application launchers
Removing duplicate launchers or broken launchers
Launchers are updated
root@cyberghazi-vmwarevirtualplatform:/# apt autoremove
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages will be REMOVED:
  figlet insserv libgit2-1.1 libio-pty-perl libipc-run-perl libmbedcrypto3 libmbedtls12 libmbedx509-0
  lshw-gtk moreutils startpar sysv-rc
0 upgraded, 0 newly installed, 12 to remove and 526 not upgraded.
After this operation, 5,555 kB disk space will be freed.
Do you want to continue? [Y/n] Y
(Reading database ... 434636 files and directories currently installed.)
Removing figlet (2.2.5-3+b1) ...
Removing sysv-rc (2.96-7) ...
Removing insserv (1.21.0-1.1) ...
Removing libgit2-1.1:amd64 (1.1.0+dfsg.1-4) ...
Removing moreutils (0.65-1) ...
Removing libipc-run-perl (20200505.0-1) ...
Removing libio-pty-perl (1:1.15-2) ...
Removing libmbedtls12:amd64 (2.16.9-0.1) ...
Removing libmbedx509-0:amd64 (2.16.9-0.1) ...
Removing libmbedcrypto3:amd64 (2.16.9-0.1) ...
Removing lshw-gtk (02.18.85-0.7) ...
Removing startpar (0.64-3) ...
Processing triggers for desktop-file-utils (0.26-1) ...
Processing triggers for gnome-menus (3.36.0-1) ...
Processing triggers for libc-bin (2.31-13+deb11u2) ...
Processing triggers for man-db (2.9.4-2) ...
Processing triggers for menu (2.1.48) ...
Processing triggers for mailcap (3.69) ...
Processing triggers for bamfdaemon (0.5.4-2) ...
Rebuilding /usr/share/applications/bamf-2.index...
Scanning application launchers
Removing duplicate launchers or broken launchers
Launchers are updated
root@cyberghazi-vmwarevirtualplatform:/# apt update
Hit:1 http://mirrors.mit.edu/parrot parrot InRelease
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
471 packages can be upgraded. Run 'apt list --upgradable' to see them.
root@cyberghazi-vmwarevirtualplatform:/# apt-get update
Hit:1 http://mirrors.mit.edu/parrot parrot InRelease
Reading package lists... Done
root@cyberghazi-vmwarevirtualplatform:/# apt install build-essential
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
build-essential is already the newest version (12.9).
0 upgraded, 0 newly installed, 0 to remove and 526 not upgraded.
root@cyberghazi-vmwarevirtualplatform:/# apt install cargo
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  libgit2-1.1 libmbedcrypto3 libmbedtls12 libmbedx509-0
Suggested packages:
  cargo-doc
The following NEW packages will be installed:
  cargo libgit2-1.1 libmbedcrypto3 libmbedtls12 libmbedx509-0
0 upgraded, 5 newly installed, 0 to remove and 526 not upgraded.
Need to get 911 kB/3,781 kB of archives.
After this operation, 12.8 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://mirrors.mit.edu/parrot parrot/main amd64 libmbedcrypto3 amd64 2.16.9-0.1 [219 kB]
Get:2 http://mirrors.mit.edu/parrot parrot/main amd64 libmbedx509-0 amd64 2.16.9-0.1 [109 kB]
Get:3 http://mirrors.mit.edu/parrot parrot/main amd64 libmbedtls12 amd64 2.16.9-0.1 [139 kB]
Get:4 http://mirrors.mit.edu/parrot parrot/main amd64 libgit2-1.1 amd64 1.1.0+dfsg.1-4 [444 kB]
Fetched 911 kB in 3s (316 kB/s)      
Selecting previously unselected package libmbedcrypto3:amd64.
(Reading database ... 434358 files and directories currently installed.)
Preparing to unpack .../libmbedcrypto3_2.16.9-0.1_amd64.deb ...
Unpacking libmbedcrypto3:amd64 (2.16.9-0.1) ...
Selecting previously unselected package libmbedx509-0:amd64.
Preparing to unpack .../libmbedx509-0_2.16.9-0.1_amd64.deb ...
Unpacking libmbedx509-0:amd64 (2.16.9-0.1) ...
Selecting previously unselected package libmbedtls12:amd64.
Preparing to unpack .../libmbedtls12_2.16.9-0.1_amd64.deb ...
Unpacking libmbedtls12:amd64 (2.16.9-0.1) ...
Selecting previously unselected package libgit2-1.1:amd64.
Preparing to unpack .../libgit2-1.1_1.1.0+dfsg.1-4_amd64.deb ...
Unpacking libgit2-1.1:amd64 (1.1.0+dfsg.1-4) ...
Selecting previously unselected package cargo.
Preparing to unpack .../cargo_0.47.0-3+b1_amd64.deb ...
Unpacking cargo (0.47.0-3+b1) ...
Setting up libmbedcrypto3:amd64 (2.16.9-0.1) ...
Setting up libmbedx509-0:amd64 (2.16.9-0.1) ...
Setting up libmbedtls12:amd64 (2.16.9-0.1) ...
Setting up libgit2-1.1:amd64 (1.1.0+dfsg.1-4) ...
Setting up cargo (0.47.0-3+b1) ...
Processing triggers for man-db (2.9.4-2) ...
Processing triggers for libc-bin (2.31-13+deb11u2) ...
Scanning processes...                                                                                         
Scanning linux images...                                                                                      

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.
Scanning application launchers
Removing duplicate launchers or broken launchers
Launchers are updated
root@cyberghazi-vmwarevirtualplatform:/# rustc --version
rustc 1.48.0
root@cyberghazi-vmwarevirtualplatform:/# apt install rustc
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
rustc is already the newest version (1.48.0+dfsg1-2).
0 upgraded, 0 newly installed, 0 to remove and 526 not upgraded.
root@cyberghazi-vmwarevirtualplatform:/# apt remove cargo
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  libgit2-1.1 libmbedcrypto3 libmbedtls12 libmbedx509-0
Use 'sudo apt autoremove' to remove them.
The following packages will be REMOVED:
  cargo
0 upgraded, 0 newly installed, 1 to remove and 526 not upgraded.
After this operation, 10.6 MB disk space will be freed.
Do you want to continue? [Y/n] Y
(Reading database ... 434430 files and directories currently installed.)
Removing cargo (0.47.0-3+b1) ...
Processing triggers for man-db (2.9.4-2) ...
Scanning application launchers
Removing duplicate launchers or broken launchers
Launchers are updated
root@cyberghazi-vmwarevirtualplatform:/# apt autoremove
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages will be REMOVED:
  libgit2-1.1 libmbedcrypto3 libmbedtls12 libmbedx509-0
0 upgraded, 0 newly installed, 4 to remove and 526 not upgraded.
After this operation, 2,149 kB disk space will be freed.
Do you want to continue? [Y/n] Y
(Reading database ... 434382 files and directories currently installed.)
Removing libgit2-1.1:amd64 (1.1.0+dfsg.1-4) ...
Removing libmbedtls12:amd64 (2.16.9-0.1) ...
Removing libmbedx509-0:amd64 (2.16.9-0.1) ...
Removing libmbedcrypto3:amd64 (2.16.9-0.1) ...
Processing triggers for libc-bin (2.31-13+deb11u2) ...
Scanning application launchers
Removing duplicate launchers or broken launchers
Launchers are updated
root@cyberghazi-vmwarevirtualplatform:/# rustc --version
rustc 1.48.0
root@cyberghazi-vmwarevirtualplatform:/# apt remove rustc
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  libstd-rust-1.48 libstd-rust-dev rust-gdb
Use 'sudo apt autoremove' to remove them.
The following packages will be REMOVED:
  rustc
0 upgraded, 0 newly installed, 1 to remove and 526 not upgraded.
After this operation, 5,857 kB disk space will be freed.
Do you want to continue? [Y/n] Y
(Reading database ... 434358 files and directories currently installed.)
Removing rustc (1.48.0+dfsg1-2) ...
Processing triggers for man-db (2.9.4-2) ...
Scanning application launchers
Removing duplicate launchers or broken launchers
Launchers are updated
root@cyberghazi-vmwarevirtualplatform:/# rustc --version
bash: /usr/bin/rustc: No such file or directory
root@cyberghazi-vmwarevirtualplatform:/# curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
info: downloading installer

Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /root/.rustup

This can be modified with the RUSTUP_HOME environment variable.

The Cargo home directory is located at:

  /root/.cargo

This can be modified with the CARGO_HOME environment variable.

The cargo, rustc, rustup and other commands will be added to
Cargo's bin directory, located at:

  /root/.cargo/bin

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /root/.profile
  /root/.bash_profile
  /root/.zshenv

You can uninstall at any time with rustup self uninstall and
these changes will be reverted.

Current installation options:


   default host triple: x86_64-unknown-linux-gnu
     default toolchain: stable (default)
               profile: default
  modify PATH variable: yes

1) Proceed with installation (default)
2) Customize installation
3) Cancel installation
>1

info: profile set to 'default'
info: default host triple is x86_64-unknown-linux-gnu
warning: Updating existing toolchain, profile choice will be ignored
info: syncing channel updates for 'stable-x86_64-unknown-linux-gnu'
info: default toolchain set to 'stable-x86_64-unknown-linux-gnu'

  stable-x86_64-unknown-linux-gnu unchanged - rustc 1.65.0 (897e37553 2022-11-02)


Rust is installed now. Great!

To get started you may need to restart your current shell.
This would reload your PATH environment variable to include
Cargo's bin directory ($HOME/.cargo/bin).

To configure your current shell, run:
source "$HOME/.cargo/env"
root@cyberghazi-vmwarevirtualplatform:/# source "$HOME/.cargo/env"
root@cyberghazi-vmwarevirtualplatform:/# rustc --version
rustc 1.65.0 (897e37553 2022-11-02)
root@cyberghazi-vmwarevirtualplatform:/# which bashrc
root@cyberghazi-vmwarevirtualplatform:/# locate bashrc
/etc/bash.bashrc
/etc/bashrc
/etc/skel/.bashrc
/home/cyberghazi/.bashrc
/usr/lib/parrot-skel/etc/skel/.bashrc
/usr/lib/python3/dist-packages/pexpect/bashrc.sh
/usr/share/base-files/dot.bashrc
/usr/share/doc/adduser/examples/adduser.local.conf.examples/bash.bashrc
/usr/share/doc/adduser/examples/adduser.local.conf.examples/skel/dot.bashrc
root@cyberghazi-vmwarevirtualplatform:/# source $HOME/.bashrc
bash: /root/.bashrc: No such file or directory
root@cyberghazi-vmwarevirtualplatform:/# source $/home/cyberghazi/.bashrc
bash: $/home/cyberghazi/.bashrc: No such file or directory
root@cyberghazi-vmwarevirtualplatform:/# source $HOME/.bashrc
bash: /root/.bashrc: No such file or directory
root@cyberghazi-vmwarevirtualplatform:/# source $HOME/.profile
root@cyberghazi-vmwarevirtualplatform:/# rustc --version
rustc 1.65.0 (897e37553 2022-11-02)
root@cyberghazi-vmwarevirtualplatform:/# cargo install ripgen
    Updating crates.io index
     Ignored package `ripgen v0.1.3` is already installed, use --force to override
root@cyberghazi-vmwarevirtualplatform:/# cargo install ripgen --force
    Updating crates.io index
  Installing ripgen v0.1.3
  Downloaded psl v2.1.3
  Downloaded libc v0.2.138
  Downloaded syn v1.0.105
  Downloaded 3 crates (1034.5 KB) in 0.92s
   Compiling proc-macro2 v1.0.47
   Compiling unicode-ident v1.0.5
   Compiling quote v1.0.21
   Compiling version_check v0.9.4
   Compiling syn v1.0.105
   Compiling memchr v2.5.0
   Compiling libc v0.2.138
   Compiling autocfg v1.1.0
   Compiling thiserror v1.0.37
   Compiling psl-types v2.0.11
   Compiling byteorder v1.4.3
   Compiling heck v0.4.0
   Compiling anyhow v1.0.66
   Compiling regex-syntax v0.6.28
   Compiling os_str_bytes v6.4.1
   Compiling hashbrown v0.12.3
   Compiling psl v2.1.3
   Compiling fxhash v0.2.1
   Compiling clap_lex v0.2.4
   Compiling once_cell v1.16.0
   Compiling indexmap v1.9.2
   Compiling bitflags v1.3.2
   Compiling proc-macro-error-attr v1.0.4
   Compiling proc-macro-error v1.0.4
   Compiling strsim v0.10.0
   Compiling termcolor v1.1.3
   Compiling lazy_static v1.4.0
   Compiling textwrap v0.16.0
   Compiling aho-corasick v0.7.20
   Compiling atty v0.2.14
   Compiling regex v1.7.0
   Compiling addr v0.15.6
   Compiling thiserror-impl v1.0.37
   Compiling clap_derive v3.2.18
   Compiling ripgen_lib v0.1.4
   Compiling clap v3.2.23
   Compiling ripgen v0.1.3
    Finished release [optimized] target(s) in 38.22s
   Replacing /root/.cargo/bin/ripgen
    Replaced package `ripgen v0.1.3` with `ripgen v0.1.3` (executable `ripgen`)
root@cyberghazi-vmwarevirtualplatform:/# ripgen
