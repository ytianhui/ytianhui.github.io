[TOC]

## Ad unit ID
The unique identifier for an ad unit.
To find the ad unit ID, click the Monetize tab. Select an app from the list of apps in the sidebar. The ad unit ID is listed below the ad unit name.

## App ID
The unique ID assigned to your app.
You'll need to integrate the app ID into your app's source code to use certain features in AdMob.
To find the ID of an app, go to Settings > App management. The IDs of all of your apps will be listed in the App ID column of the table.

## V8
V8是一个由美国Google开发的开源JavaScript引擎，用于Google Chrome中。

## NPM
Node包管理器（Node Package Manager）。它是一个以javascript编写的软件包管理系统，默认环境为Node.js，从Node.js0.6.3版本开始，npm被自动附带在安装包中。

## Node JS
Node.js 是一个基于 Chrome V8 引擎的 JavaScript 运行环境。
Node.js 使用了一个事件驱动、非阻塞式 I/O 的模型，使其轻量又高效。Node.js 的包管理器 npm，是全球最大的开源库生态系统。

## OAuth
OAuth（开放授权）是一个开放标准，允许用户让第三方应用访问该用户在某一网站上存储的私密的资源（如照片，视频，联系人列表），而无需将用户名和密码提供给第三方应用。
OAuth允许用户提供一个令牌，而不是用户名和密码来访问他们存放在特定服务提供者的数据。每一个令牌授权一个特定的网站（例如，视频编辑网站)在特定的时段（例如，接下来的2小时内）内访问特定的资源（例如仅仅是某一相册中的视频）。这样，OAuth让用户可以授权第三方网站访问他们存储在另外服务提供者的某些特定信息，而非所有内容。

## Off-the-Record Messaging
Off-the-Record Messaging（缩写为 OTR），一种安全协议，为即时通讯提供加密保护。OTR使用128bit长度的高级加密标准（AES）对称密钥加密保护，1536bits的迪菲－赫尔曼密钥交换（D-H）与SHA-1函数。在加密与验证机制之外，OTR同时提供前向保密（Forward secrecy）功能。

## CDN
A content delivery network, or CDN, offers an efficient, cost-effective way of reducing both network I/O costs and content delivery latency for regularly accessed website assets. A CDN can be understood as group of geographically-distributed caches, with each cache located in one of several global points of presence (POPs). The CDN service pulls assets from an origin server at regular intervals and distributes them to these caches. When a client requests an asset, the asset is served from the nearest cache.

## SafetyNet
SafetyNet provides services for analyzing the configuration of a particular device to **verify that it passes the Android compatibility test**.

## gsutil
gsutil is a Python application that lets you access Cloud Storage from the command line. 
You can use gsutil to do a wide range of bucket and object management tasks

## alt in html
The alt attribute provides alternative information for an image if a user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

## GCM onTokenRefresh ()
Called when the system determines that the tokens need to be refreshed. The application should call getToken() and send the tokens to all application servers.
This will not be called very frequently, it is needed for key rotation and to handle special cases.
The system will throttle the refresh event across all devices to avoid overloading application servers with token updates.

## FCM onTokenRefresh ()
Firebase Instance ID provides a unique identifier for each app instance and a mechanism to authenticate and authorize actions (example: sending FCM messages).
Instance ID is stable except when:
App deletes Instance ID
App is restored on a new device
User uninstalls/reinstall the app
User clears app data

## Canonical IDs
On the server side, as long as the application is behaving well, everything should work normally. However, if a bug in the application triggers multiple registrations for the same device, it can be hard to reconcile state and you might end up with duplicate messages.

GCM provides a facility called "canonical registration IDs" to easily recover from these situations. A canonical registration ID is defined to be the ID of the last registration requested by your application. This is the ID that the server should use when sending messages to the device.

If later on you try to send a message using a different registration ID, GCM will process the request as usual, but it will include the canonical registration ID in the registration_id field of the response. Make sure to replace the registration ID stored in your server with this canonical ID, as eventually the ID you're using will stop working.

## CRUD
In computing, CRUD is an acronym for create, retrieve, update, and delete. It is used to refer to the basic functions of a database or persistence layer in a software system.

## JavaScript是一行一行执行的，Java是按照入口之行的

## FCM background
display-messages: These messages trigger the onMessageReceived() callback only when your app is in foreground
data-messages: Theses messages trigger the onMessageReceived() callback even if your app is in background

## FCM message types
Notification messages, sometimes thought of as "display messages."
Data messages, which are handled by the client app.

## Big query 
可以链接Firebase Analytics，然后可以导入全部数据到Bigquery，

## curl
time curl 测量的是全部时间，所以长达1秒的可能，实际应用中，是只发送，后确认，所以可以很快。

## FCM Device to Device
According to the docs you must implement a server for handling push notifications in device to device communication.

## Rest API
as per the charesteristics of REST, it is independent of the client and is stateless, so the results as per latency is concerned can vary
http://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm

## .gitignore用法
在使用 Git 进行版本控制的时候，有些文件是无需纳入 Git 管理的，通常都是些自动生成的文件，
像日志或者编译过程中创建的文件。我们可以创建一个名为 .gitignore 的文件，列出要忽略的文件来解决这个问题。

## http中的payload怎么理解？
payload英语单词意思是有效载荷，在http中，应该是post请求时，所携带的有效数据的意思，比如你post请求上传文件，用谷歌浏览器抓包可以看到payload相关信息，它分成了多组数据描述信息，用类似于“------WebKitFormBoundaryaL7XJASi3bOcnKjn”这样的字符串分割，Content-Disposition: form-data; name="localUrl"这个是描述上传的文件的本地路径，Content-Disposition: form-data; name="imgFile"; filename="1.png" Content-Type: image/png这个是描述上传的图片的mime类型
