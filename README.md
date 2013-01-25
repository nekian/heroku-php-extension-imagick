heroku-php-extension-imagick
================

Compiled a few library for Heroku's PHP extension - __imagick.so__

And Setting for local development environment. - __php_imagick.dll__



Instruction for 'imagick.so': 
----------------------------
for Heroku

1.  create folder __ext__ in project folder

2.  put __imagick.so__ in __ext__ folder

3.  create file __php.ini__ in main folder of project

4.  Add this line to __php.ini__ 
<PRE>
extension=/app/www/ext/imagick.so
</PRE>
  
5.  $ __git add php.ini ext/imagick.so__

6.  $ __git commit -m "PHP's imagemagick library"__

7.  $ __git push heroku master__



Instruction for 'php_imagick.dll':
----------------------------
for Local development

1.  open file __php.ini__ in local php folder

2.  Add this line to __php.ini__
<PRE>
extension=php_imagick.dll
</PRE>

3.  put __php_imagick.dll__ in local PHP's __ext__ folder

4.  restart local apache server