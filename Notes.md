## About

This repository is forked from ONLYOFFICE/Docker-CommunityServer, we have the following modifications are provided

* replace README.md
* add README-zh.md, CHANGELOG.md, Note.md, License.md, docker-compose-production.yml, .github folder

## FAQ

#### Drupal 容器的用户是什么？

www-data

#### mount 挂载 modules, profiles 之后没有权限怎么办？

```
chown -R www-data:www-data volumes/drupal
```

#### Drupal 容器启动后是否已经连接数据库？

没有，需要在安装向导完成数据库配置

#### Drupal 安装向导数据库总是连接不成功？

确保主机名称正确  

![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/drupal/drupal-install-db-docker-websoft9.png)
