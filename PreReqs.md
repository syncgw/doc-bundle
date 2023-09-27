# ![picture logo](../gui-bundle/assets/syncgw.png "sync•gw") #
 
![](https://img.shields.io/packagist/v/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/l/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/dt/syncgw/doc-bundle.svg)
 
**sync•gw** is the one and only fully portable server software available providing synchronization service between nearly any mobile device and your web server.

# System requirements #

**sync•gw** is fully written in PHP. Your web server should provide the following PHP configuration:

* At minimum PHP version **[7.1.1](http://www.php.net/downloads.php#v7)**.
* At minimum **[8 MB](http://www.php.net/manual/en/ini.core.php#ini.memory-limit)** memory.
* PHP extension **[DOM_XML](https://www.php.net/manual/de/dom.setup.php)** need to be disabled.
* PHP extension **[GD](http://www.php.net/manual/en/image.setup.php)** must be enabled.
* If you want to down or upload data from "Administrator Interface", PHP extension **[ZIP](http://www.php.net/manual/en/zip.setup.php)** need to be enabled.
* If you want to synchronize multi-byte language date, you need to enable PHP extension **[Multi byte extension](http://www.php.net/manual/en/mbstring.installation.php)**.
* If you want to use a MySQL server database, you need to enable **[MySQLi](http://www.php.net/manual/en/mysqli.installation.php)** extension.

You may download a small PHP script to check the system requirements from the avaibale [downloads](Downloads.md).

[Go back](./README.md/)
