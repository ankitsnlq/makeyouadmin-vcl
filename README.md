makeyouadmin-vcl
================
It is copy of TheNextWeb Varnish VCL with some customization which i am using for My site [MakeYouAdmin](www.makeyouadmin.com) Following is features of my Varnish VCL.

1.Don't Cache Wp-admin.

2.Forward User IP to Backend Apache server so Wordpress can get Origin IP of User not Varnish server IP address.


3.Remove Cookies from Static Pages so that Varnish can Cache Pages Properly.

4.Auto Purge (Remove Cached Content) Varnish Cache when somone comments or you Publish new Post.


5.Don't Cache Wordpress Post Preview page, to keep that feature working.


6.Don't Cache Sitemap Page of your site , else when you Purge your cache search engine bots again read your site whole sitemap.(This i come to Know From Google Webmaster Tools, when i use to cache Makeyouadmin Sitemap page, Every time I purge Varnish Cache Google Webmaster Tools shows URLs submitted and URLs indexed 0 in Sitemap section. Once Google bots visit my site again every thing become normal.).

7.Don't Cache search Results , so that User see fresh Content when they search Something from your site.

