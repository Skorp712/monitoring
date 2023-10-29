Задание 1

Команды

# wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-5+debian12_all.deb
# dpkg -i zabbix-release_6.0-5+debian12_all.deb
# apt update
# apt install zabbix-server-pgsql zabbix-frontend-php php8.2-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent
# sudo -u postgres createuser --pwprompt zabbix
# sudo -u postgres createdb -O zabbix zabbix
# zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix
# nano /etc/zabbix/zabbix_server.conf (DBPassword=password)
# systemctl restart zabbix-server zabbix-agent apache2
# systemctl enable zabbix-server zabbix-agent apache2

![alt text](https://github.com/Skorp712/monitoring/blob/main/1.png)

Задание 2

# wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-5+debian12_all.deb
# dpkg -i zabbix-release_6.0-5+debian12_all.deb
# apt update
# apt install zabbix-agent2 zabbix-agent2-plugin-*
# systemctl restart zabbix-agent2
# systemctl enable zabbix-agent2

![alt text](https://github.com/Skorp712/monitoring/blob/main/11.png)
![alt text](https://github.com/Skorp712/monitoring/blob/main/13.png)
![alt text](https://github.com/Skorp712/monitoring/blob/main/23.png)
![alt text](https://github.com/Skorp712/monitoring/blob/main/3.png)
![alt text](https://github.com/Skorp712/monitoring/blob/main/33.png)
