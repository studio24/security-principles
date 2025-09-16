# Supported versions

Our policy is to only use supported and up-to-date software. If any website or web application cannot be upgraded to a supported version then it is considered legacy software and we'll make recommendations on how to resolve this.

We aim to update this page on a semi-regular basis.

### Current supported versions

| Software                                                            | Description  | Active support | Security support | Major version policy             |
|---------------------------------------------------------------------|--------------|----------------|------------------|----------------------------------|
| [PHP](https://www.php.net/supported-versions)                       | Programming language | 8.3, 8.4 | 8.1, 8,2       | Point releases (e.g. 8.4 to 8.5) |
| [Laravel](https://laravel.com/docs/releases#support-policy)         | Web framework (PHP)  | 11, 12 |                  | Major releases (e.g. 12 to 13)   |
| [Symfony](https://symfony.com/releases)                             | Web framework (PHP)  | 6, 7   | 5                | Major releases (e.g. 7 to 8)     |
| [WordPress](https://wordpress.org/download/releases/)               | CMS (PHP)    | 6.8 [^1]       |                  | Point releases (e.g. 6.8 to 6.9) |
| [Craft CMS](https://craftcms.com/knowledge-base/supported-versions) | CMS (PHP)    | 5              | 4                | Major releases (e.g. 5 to 6)     |
| [NodeJS](https://nodejs.org/en/about/previous-releases)             | JavaScript runtime | 22 [^2]  | 20               | Major releases (e.g. 22 to 23)   |
| [MySQL](https://dev.mysql.com/doc/refman/9.4/en/mysql-releases.html) | Database    | 8.4, 9.4       | 8.0              | Point releases (e.g. 8.3 to 8.4) |
| [MariaDB](https://mariadb.com/docs/release-notes/community-server/about/release-model) | Database | 10.11, 11.4, 11.8 |  | Point releases (e.g. 11.3 to 11.4) |
| [PostgreSQL](https://www.postgresql.org/support/versioning/)        | Database     | 15, 16         |                  | Major releases (e.g. 15 to 16)   |
| [SQLite](https://sqlite.org/lts.html)                               | Database     | 3 [^3]         |                  | Major releases (e.g. 3 to 4)     |

A useful website for end of life information is [endoflife.date](https://endoflife.date/)

[^1]: Officially, WordPress only maintains the current major version. Previous major releases before this may or may not get security updates as serious exploits are discovered.
[^2]: We only use long-term support (LTS) releases of NodeJs, which typically guarantees that critical bugs will be fixed for a total of 30 months.
[^3]: SQLite 3 has long-term support until 2050!
