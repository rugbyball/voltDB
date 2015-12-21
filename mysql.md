config authentication
===
mysql -p <br />
use mysql <br />
select host, user, authentication_string from user; <br />
update user set host = '%'; <br />
