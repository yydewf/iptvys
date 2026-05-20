# IPTV影视 - iptvys

定制影视TV播放器。支持rtp2httpd代理的RTSP源。解决RTSP节目在通过RTSP to HTTP代理播放时不能获取时长信息，不能拖动进度条、快进快退等问题。

RTSP是国内IPTV使用的主流协议，但许多播放器对RTSP源的支持不好。把RTSP转发成HTTP是一种解决方案。rtp2httpd就是一款非常优秀多媒体流转发服务器，支持将组播 RTP/UDP 流、RTSP 流转换为 HTTP 单播流。但rtp2httpd代理的RTSP点播资源（电影/剧集等），由于使用的 RTSP MPEG-TS 封装，在转成 HTTP 后，无法提供播放时间显示、快进快退能力。播放器在播放时，没有点播节目时长信息，只能从头播放，不能拖动进度、快进快退等。这显然非常不方便。

IPTV影视是基于影视TV/蜂蜜影视的适配，支持通过rtp2httpd代理RTSP源播放。支持RTSP点播节目的时长信息获取，进度条拖动，快进快退等。IPTV影视保持蜂蜜影视的全部功能，在播放设置中增加了RTSP代理的选项。想通过rtp2httpd代理播放RTSP源，只需开启RTSP代理，并在RTSP代理地址中输入rtp2httpd服务的地址即可。开启RTSP代理后，IPTV影视在播放RTSP节目时，自动会通过rtp2httpd代理后播放。


使用方法：<br>
在播放设置中，开启RTSP代理，并设置RTSP代理地址 ( rtp2httpd地址，e.g. <code>http://192.168.1.4:4022</code> )。


###  基于蜂蜜影视版：
TV版：leanback-arm64_v8a.apk leanback-armeabi_v7a.apk<br>
手机版：mobile-arm64_v8a.apk mobile-armeabi_v7a.apk

