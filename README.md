Vewngyu
=======

A system for tracking habits and behaviors, and visualizing the trends over the time.

Install and Run
---------------

Currently ensure that you have python-virtualenv and then run the following command:
`virtualenv . && . bin/activate && pip install django`

You should make a config file by running `make ~/.vewngyu` and then adding a config file
in ~/.vewngyu/config.ini which contains at the minimum:
```
[vewngyu]
salt = YourSecretSaltHere
```

A Full config is
```
[vewngyu]
salt = YourSecretSaltHere
debug = true

[database]
engine = mysql
host = database.example.com
port = 3306
name = TableName
```
_Database default's to sqlite database named 'saomum.db'_

Other database engines are:

| Engine              | Database     |
| --------------------|--------------|
| postgresql_psycopg2 | PostgreSQL   |
| mysql               | MySQL        |
| sqlite3             | SQLite       |
| oracle              | Oracle DB    |


Bugs
----

Please report any bugs you find on [the Github](https://github.com/Aeva/vewngyu/issues)

Licence
-------

Vewngyu is under the AGPL version 3

[<img alt="AGPL v3" src="https://www.gnu.org/graphics/agplv3-155x51.png">](https://www.gnu.org/licenses/agpl-3.0.html)
