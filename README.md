

<VirtualHost *:80>
    ServerName vlms.dev
    ServerAlias *.vlms.dev


    DocumentRoot
/home/vohung/vietEd_Work/vlms/public/ 
    <Directory />
         Options            Indexes 
FollowSymLinks
      AllowOverride None
      AllowOverride      All
      Require all granted
      RewriteEngine On
    </Directory>


<Directory
"/home/vohung/vietEd_Work/vlms/public/">
     Options            Indexes  FollowSymLinks
      AllowOverride None
      AllowOverride      All
      Require all granted
      RewriteEngine On
</Directory>
AccessFileName     .htaccess


    SetEnv CODENAME edx
    SetEnv NO_PERMISSION 1
    SetEnv APPLICATION_ENV development.vlms
    SetEnv LANGUAGE en
    SetEnv k c65ff8694e5bad1c1a805f5aac721bdf
php_value session.cookie_domain edx.dev
Header set Access-Control-Allow-Origin "*"
</VirtualHost>




<VirtualHost *:80>
    ServerName system.vlms.dev
    ServerAlias *.vlms.dev


    DocumentRoot
/home/vohung/vietEd_Work/vlms/public/
    <Directory />
         Options            Indexes 
FollowSymLinks
      AllowOverride None
      AllowOverride      All
      Require all granted
      RewriteEngine On
    </Directory>


<Directory
"/home/vohung/vietEd_Work/vlms/public/">
     Options            Indexes  FollowSymLinks
      AllowOverride None
      AllowOverride      All
      Require all granted
      RewriteEngine On
</Directory>
AccessFileName     .htaccess


    SetEnv CODENAME edx
    SetEnv NO_PERMISSION 1
    SetEnv APPLICATION_ENV development.vlms
    SetEnv LANGUAGE en
    SetEnv k c65ff8694e5bad1c1a805f5aac721bdf
php_value session.cookie_domain edx.dev
Header set Access-Control-Allow-Origin "*"
</VirtualHost>




<VirtualHost *:80>
    ServerName mongodb.dev
    DocumentRoot
/home/vohung/vietEd_Work/mongodb
    <Directory />
          Options            Indexes 
FollowSymLinks
      AllowOverride None
      AllowOverride      All
      Require all granted
      RewriteEngine On
    </Directory>


<Directory
"/home/vohung/vietEd_Work/mongodb">
     Options            Indexes  FollowSymLinks
      AllowOverride None
      AllowOverride      All
      Require all granted
      RewriteEngine On
</Directory>
</VirtualHost>
