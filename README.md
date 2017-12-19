# MySQL パフォーマンス最適化勉強用

## Wordpress

- Docker for Mac

### Init

http://mysql.local

**/etc/hosts**

```sh
127.0.0.1    mysql.local
```

```sh
$ bin/c dc build
$ bin/c dc start
$ docker exec mysql_mysql mysql -u mysql_study -p3030 mysql_study < develop.sql
```

### Start

```sh
$ bin/c dc start
```

### Stop

```sh
$ bin/c dc stop
```

### Dump

```sh
$ bin/c dc ssh mysql_mysql
$ mysqldump -u mysql_study -p mysql_study > develop.sql #PW: 3030
```

### Admin

http://mysql.local/wp/wp-admin

- ID: dev / PW: `NXn*49pyjW9$lfNKBc`

---

## c

`~/.bash_profile`などに、`export PATH="./bin:$PATH"`を追加しておくとPATHが通るので楽です。

### c docker build / c dc build

```sh
$ bin/c dc build
```

### c docker start / c dc start

```sh
$ bin/c dc start
```

### c docker stop / c dc stop

```sh
$ bin/c dc stop
```

### c docker ssh / c dc ssh

```sh
$ bin/c dc ssh
```