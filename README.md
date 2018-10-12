# hello

To use your new extension, you will have to execute the following steps:

1.  

        $ cd hello

2.  

        $ vi config.m4

3.  

        $ phpize

4.  

        $ ./configure --[with|enable]-hello

5.  

        $ make

6.  
        $ php -d extension=.libs/hello.so -f hello.php
        Functions available in the test extension:
        confirm_hello_compiled

        Congratulations! You have successfully modified ext/hello/config.m4. Module hello is now compiled into PHP.

    or

        $ php -d extension=.libs/hello.so -m | grep -i hel
        hello

7.  

        $ vi ext/hello/hello.c

8.  
        $ make

Repeat steps 3-6 until you are satisfied with ext/hello/config.m4 and
step 6 confirms that your module is compiled into PHP. Then, start writing
code and repeat the last two steps as often as necessary.
