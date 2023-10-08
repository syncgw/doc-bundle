# ![picture logo](https://github.com/syncgw/gui-bundle/blob/master/assets/syncgw.png "sync•gw") #
 
![](https://img.shields.io/packagist/v/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/l/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/dt/syncgw/doc-bundle.svg)
 
**sync•gw** is the one and only fully portable server software available providing synchronization service between nearly any mobile device and your web server.

This file contains the list of all available bundles.

## [sync•gw core-bundle](../core-bundle/README.md) ##
* Written in PHP - no binary CPU depended code.
* Support of **[XML](https://en.wikipedia.org/wiki/XML)** and 
**[WBXML](http://en.wikipedia.org/wiki/WBXML)** protocol.
* Support of **[WebDAV](https://en.wikipedia.org/wiki/WebDAV)** (**CalDAV** and **CardDAV**) protocol.
* Support of **[MicroSoft Exchange ActiveSync (EAS)](http://en.wikipedia.org/wiki/Exchange_ActiveSync)** protocol (2.5, 12.0, 12.1, 14.0, 14.1, 16.0, 16.1).
* Only a web server with PHP is required to run **sync•gw** (no additional software or tools required).
* Full internationalization support.
* Multi byte support (support for e.g. Japanese language).
* Support for time zones..
* Multiple level of logging supported
* Intelligent field assignment - calculated based on mix of configuration file and probability calculation.
* Programming documentation available (see **Developers Guide** in the [Downloads](../doc-bundle/Downloads.md).
* Support for encrypted message exchange using SSL web server setting.
* Administrator browser interface with password protection.
* Contact synchronization support.
* Calendar and task synchronization support.
* Notes synchronization support.
* Experimental: Mail synchronization support.

**sync•gw** setup is very easy. Install this software bundle, check for other bundles [Bundles](../doc-bundle/Bundles.md), define a administrator password, connect a data base handler and **sync•gw** is ready for your first synchronization.

A detailed description of available configuration option is available in our browser interface documentation available in the [download section](../doc-bundle/Downloads.md)).

## [sync•gw file-bundle](../file-bundle/README.md) ##
**sync•gw** requires an interface bundle to store and handle data during synchronization. 
This data base handler is useful when your installation does not provide any MySQL data base handler.

## [sync•gw mysql-bundle](../mysql-bundle/README.md) ##
**sync•gw** requires an interface bundle to store and handle data during synchronization. 
This data base handler is useful when you want to synchronize data between devices and you does not have any server application running.

## [sync•gw RoundCube bundle](../roundcube-bundle/README.md) ##
**sync•gw** requires an interface bundle to store and handle data during synchronization. 
This data base handler includes the MySQL data base handler mentioned above. Additionally this interface handler synchronizes data (e.g. **contact** records) from RoundCube with **sync•gw** internal records. Your application users can always access most current data.

## [sync•gw myapp bundle](.../myapp-bundle/README.md) ###
**sync•gw** requires an interface bundle to store and handle data during synchronization. 
If you require any another interface bundle for which you're need a handler not listed here, you may either develop your own (for more information, please read our **Developer Guide** in our [download section](Downloads.md).

## [EXPERIMENTAL: sync•gw mail-bundle](../mail-bundle/README.md) ###
**sync•gw** requires an interface bundle to store and handle data during synchronization. 
The purpose of this interface handler is to communicate to an **IMAP** and a **SMTP** handler. It is an "on top" interface to all other data base handler. Currently this interface handler is in development and I hope to offer it as soon as possible. Please aware, this interface handler does not turn **sync•gw** into a full blown **Exchange server**. It does not support only **MicroSoft Exchange** protocol. But it is able to synchronize mails from your mail server to client devices. It is included in **Developer Edition** only.

## [sync•gw webdav-bundle](../webdav-bundle/README.md) ##
Protocoll bundle were used to handle the comunication with your device. 
The included files enables support for [CalDav](http://en.wikipedia.org/wiki/CalDAV) and [CardDav](http://en.wikipedia.org/wiki/CardDAV) protocol. 

## [sync•gw activesync-bundle](../activesync-bundle/README.md) ##
Protocoll bundle were used to handle the comunication with your device. 
The included files enables support for [MicroSoft ActiveSync](http://en.wikipedia.org/wiki/Exchange_ActiveSync). 

## [EXPERIMENTAL: sync•gw mapi-bundle](../mapi-bundle/README.md) ##
If you want to connect your **[Outlook](https://en.wikipedia.org/wiki/Outlook)** installation to **sync•gw**,
then you need **Messaging Application Programming Interface (MAPI) over HTTP ** protol.

The included files enables support for [MAPI](https://en.wikipedia.org/wiki/MAPI). Technically the
communication between **Outlook** and your **sync•gw** installation works fine, bute unfortunately 
currently the results were poor. Due to the very poor documentation provided by **MicroSoft**, I was not able
to find out the meaning of many fields. 

## [EXPERIMENTAL: ROPS bundle for sync•gw](../rops-bundle/README.md) ##
If you want to connect your **[Outlook](https://en.wikipedia.org/wiki/Outlook)** installation to **sync•gw**,
then you need **Remote Operations (ROP) List and Encoding** protocol.

## [EXPERIMENTAL: RPC bundle for sync•gw](../rpc-bundle/README.md) ##
If you want to connect your **[Outlook](https://en.wikipedia.org/wiki/Outlook)** installation to **sync•gw**,
then you need **Wire Format Protocol handler** protocol.

## [EXPERIMENTAL: ICS bundle for sync•gw](../ics-bundle/README.md) ##
If you want to connect your **[Outlook](https://en.wikipedia.org/wiki/Outlook)** installation to **sync•gw**,
then you need **Bulk Data Transfer Protocolr** protocol.

[[Go back](README.md)]
[[System requirements](PreReqs.md)] 
[[Available bundles](Bundles.md)] 
[[List of all changes](Changes.md)] 
[[Additional Downloads](Downloads.md)] 
[[Frequently asked questions](FAQ.md)] 
[[Supported feature](Features.md)]

