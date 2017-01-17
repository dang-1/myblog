# myblog
system: centos 7.3  
python: 2.7.10

    yum install -y mariadb mariadb-server mariadb-devel
    yum install -y python pip
    systemctl start mariadb.service
    pip install django==1.8
    pip install MySQL-python
    pip install Pillow


    python manage.py syncdb #第一次
    python manage.py migrate
    create database blogdb charset=utf8;
