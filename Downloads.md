# ![picture logo](https://github.com/syncgw/gui-bundle/blob/master/assets/syncgw.png "sync•gw") #
 
![](https://img.shields.io/packagist/v/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/l/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/dt/syncgw/doc-bundle.svg)
 
**sync•gw** is the one and only fully portable server software available providing synchronization service between nearly any mobile device and your web server.


# Downloads #

## [System check](downloads/Check/check.php) ##
You may use this small PHP program to perform a check of the system requirements for **sync•gw**. Please download file to your web server root directory and call script by opening `http://[your domain]/check.php` in your favorite browser. Alternatively you may check system requirements [manually](https://github.com/toteph42/syncgw/blob/master/downloads/PreReqs.md).

## [Fast-CGI configuration](downloads/Fast-CGI/.htaccess) ##
If you recognize during synchronization your web server is always asking for credentials even if
you have specified during configuration of synchronization, is may be the reason your domain is
running in FastCGI mode. To fix this problem, please copy `.htaccess` to the root 
directory of your web server.  

## [WebDAV configuration](downloads/WebDAV/.htaccess) ##
If you want to use the **WebDAV** protocoll for synchronization between your client device and **sync•gw** server 
and you don't want to force your user to add to the server name `/sync.php` during configuration of 
synchronization (they need to specify `[your-domain]/sync.php` instead of only `[your-domain]`), then you have 
two choices:

If you have access to the apache configuration files, your may add the following alias definitions 
to your Web server configuration:

```	
Alias /.well-known/carddav    [Path to]/sync.php
Alias /.well-known/caldav     [Path to]/sync.php
```

Alternatively you may copy `.htaccess` file to the root directory of your domain.
 
If you receive warning message **19001**, then you've enabled both **Calendar** and **Task list** synchronization 
on **sync•gw** server and you want to use the **WebDAV** protocoll for synchronization. Unfortunatly 
**WebDaV** does not differentiate between **Calendar** and **Task lists** during initial synchronization requests
ending up **sync•gw** does not know which synchronization is wanted. To avoid confusion **sync•gw** automatically disabled the **Task list** synchronization.

There are two option available to handle this situation:

1. If you've installed your **sync•gw** server on domain `[your-domain]` , then please  define an additional 
domain (e.g. `task.[your-domain]`) and edit file `config.ini.php` in **sync•gw** directory and change parameter
`ForceDav = ""` to `ForceDav = "task"`. If you want to use a different sub domain name, then specify this name in configuration file `config.ini.php`.

   Finally define your synchronization profile for **Calendar** on client device using domain `[your-domain]` and for **Task list** use domain `task.[your-domain]`.

2. Create a second **sync•gw** installation on same domain with a second configuration  file e.g. in a sub-directory `[your-domain]/task`. Then edit `config.ini.php` file in this sub directory and change parameter `ForceDav = ""`
to `ForceDav = "FORCE"`.

   Finnaly you should advise your users to specify the host name `[your-domain]/task` during configuration 
of the `Task list` synchronization.
	  
## [Exchange ActiveSync (EAS) configuration](downloads/ActiveSync/.htaccess) ##
If you want to use the **Exchange ActiveSync (EAS)** synchronization between your client device and 
**sync•gw** server and you don't want to force your user to add to the server name `/sync.php` during 
configuration of synchronization (they need to specify `[your-domain]/sync.php` instead of only
`[your-domain]`), then you should copy `.htaccess file` to the root directory of your domain.

## [EXPERIMENTAL: MAPI over HTTP](downloads/MAPI/.htaccess) ##
If you want to use MAPI over HTTP then you should copy `.htaccess` file to the root directory of your domain. 

## [Browser Interface (GUI)](downloads/GUI/BrowserInterface.pdf) ##
Description of **sync•gw** browser interface also available as [.docx file](downloads/GUI/BrowserInterface.docx).

## [Developer Guide](downloads/DeveloperGuide/DeveloperGuide.pdf) ##
Application back end developers guide (also available as [.docx file](downloads/DeveloperGuide/DeveloperGuide.docx)). This gives you information about the [myApp](../myapp-bundle/) skeleton interface handler.

[[Go back](README.md)]
[[System requirements](PreReqs.md)] 
[[Available bundles](Bundles.md)] 
[[List of all changes](Changes.md)] 
[[Additional Downloads](Downloads.md)] 
[[Frequently asked questions](FAQ.md)] 
[[Supported feature](Features.md)]
