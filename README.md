# php-compile-script
Updated PHP compile script for PocketMine. Open a issue in the issue tracker if you have issues with this compile script!

Use this script to build the custom PHP binary for PocketMine. Make sure you have ``make autoconf automake libtool m4 wget getconf gzip bzip2 bison g++``.

| Flag   | Description                                                  |
| ------ | ------------------------------------------------------------ |
| -t     | Set target                                                   |
| -j     | Set make threads to #                                        |
| -c     | Will force compile cURL                                      |
| -l     | Will compile with LevelDB support (not supported with PHP7)  |
| -f     | Enabling abusive optimizations...                            |

### Example:

| Target  | Arguments |
| ------- | --------- |
| linux64 | ``-t linux64 -j 2 -c -f x86_64`` |
| mac64   | ``-t mac64 -l -j -c -f``            |
  
If you are compiling with Linux, I reconmend ``./compile.sh -t linux64 -c -f x86_64``.
