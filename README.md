heroku-php-extension-imagick
================

Compiled a few library for Heroku's PHP extension - imagick.so

And Setting for local development environment.

----------------------------
# for Heroku
Instruction for 'imagick.so':
----------------------------

1.  create folder "ext" in project folder

2.  put "imagick.so" in "ext" folder

3.  create file "php.ini" in main folder of project

4.  Add this line to "php.ini" 
	extension=/app/www/ext/imagick.so
  
5.  $ git add php.ini ext/imagick.so

6.  $ git commit -m "PHP's imagemagick library"

7.  $ git push heroku master


----------------------------
# for Local development
Instruction for 'php_imagick.dll':
----------------------------

1.  open file "php.ini" in local php folder

2.  Add this line to "php.ini"
	extension=php_imagick.dll

3.  put "php_imagick.dll" in local PHP's "ext" folder

4.  restart local apache server