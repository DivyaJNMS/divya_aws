# divya_aws
Online/offline
#Steps to launch developer html templates on AWS server


steps to deploy the zip directory in EC2 instance (Linux OS)=>

1) mkdir temp
2) ls -lrt
3) cd temp/
4) (Now select any free css template file and copy the doawload link)
5) wget https://www.free-css.com/assets/files/free-css-templates/download/page292/picstudio.zip
6) ls -lrt
7) unzip picstudio.zip            (unzip the folder)
8) ls -lrt
9) mv * /var/www/html/        (Move the Css tempalte file to html folder)
10) systemctl enable httpd
11) systectl start httpd

(Note : if we have note seletected teh Http and https option while creating the server. kindly go to the Security option in instance then inbound rule  then select the option of HTTP and HTTPs and save the rules)


13) cd /var/www/html/    .........(cpy directory name and html file name from here. Create link like IP address/directoryname/html_fil_ename)
14) http://3.110.173.74/picstudio-html/index.html
