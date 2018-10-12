# hello

To use your new extension, you will have to execute the following steps:

1.  $ cd ..
2.  $ vi ext/hello/config.m4
3.  $ ./buildconf
4.  $ ./configure --[with|enable]-hello
5.  $ make
6.  $ ./sapi/cli/php -f ext/hello/hello.php
7.  $ vi ext/hello/hello.c
8.  $ make

Repeat steps 3-6 until you are satisfied with ext/hello/config.m4 and
step 6 confirms that your module is compiled into PHP. Then, start writing
code and repeat the last two steps as often as necessary.
