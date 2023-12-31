# ![picture logo](https://github.com/syncgw/gui-bundle/blob/master/assets/syncgw.png "sync•gw") #
 
![](https://img.shields.io/packagist/v/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/l/syncgw/doc-bundle.svg)
![](https://img.shields.io/packagist/dt/syncgw/doc-bundle.svg)
 
**sync•gw** is the one and only fully portable server software available providing synchronization service between nearly any mobile device and your web server.

# Client device #
<details> 
<summary><strong>Why does my phone number does not arrive on client device?</strong></summary>
<p>Some information may not be synchronized due to internal device limitations not covered by back end handler. In some back ends you may enter "abc" as telephone number. If you try to synchronize this piece of information to cell phone, telephone number will not be synchronized, because numbers strings are only allowed to contain the digits 0 to 9 and the special characters "+ ()#".</p>
</details>

<details>
<summary><strong>I've attached a picture to my contact on server. Why does it not synchronize to client device?</strong></summary>
<p>All images are stored in common PNG graphic format in <strong>sync•gw</strong>. As soon as you connect your client device to <strong>sync•gw</strong> and this device is capable of receiving or sending images, the image is converted to the supported graphic format (the information about the supported graphics formats are exchanged during synchronization initialization).<br>
During exchange of device information, some client devices raises the "Supporting pictures" flag, 
but does include which graphic formats is supported. <strong>sync•gw</strong> assumes as default the <strong>JPEG</strong> graphic format. If that format is not supported by client device, picture may not been shown.</p>
</details>

<details>
<summary><strong>My server do not accept my credentials. What can I do?</strong></summary>
<p>If your server is configured to run as <strong>FAST-CGI</strong> then Apache do not provide your credentials automatically to PHP. Please goto to <a href="Downloads.md">downloads</a> and install the file <code>.htaccess</code> in root directory of your internet server.</p>
</details>

# Client configuration #

<details>
<summary><strong>CardDAV: How do I have to configure my <em>Android device</em> for synchronizing?</strong></summary>
<p>Please use the following Android CardDav description as starting point. This documentation should help you figuring out how to configure your device.<br>
<ul><li>Select <a href="assets/webdav-1.png" target="_blank">CardDav-Sync</a></li>
<li>Enter <a href="assets/carddav-1.png" target="_blank">URL, user id and password</a>. For more information about which URL to use, please check out our data store definitions</li>
<li>Select <a href="assets/carddav-2.png" target="_blank">address book</a> to sync</li>
<li>Check <strong>Account Name</strong> and click on <a href="assets/carddav-3.png" target="_blank">address bookFinish</a>. For synchronization in both directions please don't forget to un-check check box</li>
</ul></p>
</details>

<details>
<summary><strong>CardDAV: How do I have to configure my iPhone device for synchronizing?</strong></summary>
<p>Please use the following <em>iPhone CardDav</em> description as starting point. This documentation should help you figuring out how to configure your device.<br>
<ul>
<li>In <strong>Settings</strong> open <a href="assets/ip01.png" target="_blank">Accounts &amp; Passwords</a></li>
<li>Select <a href="assets/ip02.png" target="_blank">Add Account</a></li>
<li>Select <a href="assets/ip03.png" target="_blank">Other</a></li>
<li>Select <a href="assets/ip04.png" target="_blank">Add CardDAV Account</a></li>
<li>Insert server name (e.g. <code>[your-domain]</code>), your user name (e.g. <strong>test@xx.com</strong>), your password and a description. Then click on <a href="assets/ip05.png" target="_blank">Next</a>. Please note, it might happen your iPhone claims the server certificate does not match. This might happen if you use <strong>Let's Encrypt</strong> certificates. In this case, please accept certificate shown.</li>
</ul>
</p>
</details>

<details>
<summary><strong>ActiveSync: How can I configure my device for synchroniziation?</strong></summary>
<p>Please use the this description for an <em>Android device</em> as starting point. This documentation should help you figuring out how to configure your device.<br>
<ul>
<li>Select <strong>Settings</strong> and scroll down to <a href="assets/pic01.png" target="_blank">Accounts</a></li>
<li>Select <a href="assets/pic02.png" target="_blank">Microsoft Exchange ActiveSync</a></li>
<li>Enter <a href="assets/pic03.png" target="_blank">E-Mail address and Password</a> and click on <strong>Manual Setup</strong></li>
<li>Change in field <strong>Domain\username</strong> your user name to your e-Mail address. Add to <strong>Exchange server</strong> the <code>/sync.php</code> script name. If your server does not have an valid SSL certificate available, de-select <strong>Use secure connection</strong> and click on <a href="assets/pic04.png" target="_blank">Sign in</a></li>
</ul></p>
</details>

[[Go back](README.md)]
[[System requirements](PreReqs.md)] 
[[Available bundles](Bundles.md)] 
[[List of all changes](Changes.md)] 
[[Additional Downloads](Downloads.md)] 
[[Frequently asked questions](FAQ.md)] 
[[Supported feature](Features.md)]

