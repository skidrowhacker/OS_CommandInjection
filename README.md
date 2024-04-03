What is OS Command Injection ? ماهي ثغرة حقن اوامر نظام التشغيل 
it's also known as shell Injection / معروفة ايضا باسم حقن الشيل 
it allows an attacker to execute OS Commands such as Whoami,id,ver,uname-a.. etc تسمح للمهاجم بتنفيذ اوامر انظمة تشغيل مثل 
where this Vunrability can be found ? اين توجد هذه الثغرة 
occur when web applications call operating system commands with user-supplied input provided as arguments \ عندما تطبيق ويب يستدعي دوال انظمة تشغيل عن طريق مدخلات يتحكم فيها المستخدم 
such as ; مثل
exec,passthru,shell_exec,system
how to Exploit this ? \ كيف يتم الاستغلال ؟ 
?file=1.jpg
?id=2
using characters استخدام اختصارات مثل
&
&&
|
||
;

prevent OS command injection \ كيف يتم منع هذه الثغرة او اصلاحها ؟  
(1 ) تعطيل استخدام هذه الدوال / Disable functions باستخدام php.ini \ using 
disable_functions=exec,passthru,shell_exec,system

(2) input sanitization  \مراجعة مدخلات المستخدم والتاكد منها

(3) Using BlackList\Wafs\ escapeshellcmd

مراجع للثغرة / Refrance 
https://book.hacktricks.xyz/pentesting-web/command-injection
https://portswigger.net/web-security/os-command-injection

twitter.com/@firfox20

./GoodLuck
