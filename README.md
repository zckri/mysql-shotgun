# mysql-shotgun
MySQL master-slave replication inside docker containers

[docker](http://www.docker.com) and [fig](http://www.fig.sh) are required for this to work.

**Installation and run.**
```
$ git clone https://github.com/zckri/mysql-shotgun.git
$ cd mysql-shotgun
$ fig up
```

**Accessing db**

- master: root@localhost:3306
- slave: root@localhost:3307
- creditentials: root/masterpass12

*see [this](https://github.com/zckri/mysql-shotgun/blob/master/dbmaster/run) and [also this](https://github.com/zckri/mysql-shotgun/blob/master/dbslave/run) to change your creditentials*
