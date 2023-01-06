---
title: Magento 2 install part 1 - Install on unbutu or windows
---

1. Install magento 2.4 on Windows 10 :
I use [Laragon](https://laragon.org/download/index.html) to setup LEMP on windows 10 :

2. Install magento 2.4 ubuntu 22.04 :

3. Create docker container:

4. Use docker:
> Base on [mgt-ecomerece](https://www.mgt-commerce.com/docs/mgt-development-environment/installation)

{% highlight bash lineos %}
docker run -d --net=bridge -v /var/lib/mysql -v /home/cloudpanel --restart=always --privileged -h mgt-dev --name mgt-dev -it -p 80:80 -p 443:443 -p 8443:8443 -p 22:22 -p 3306:3306 -p 9200:9200 -p 15672:15672 mgtcommerce/mgt-dev:v3
{% endhighlight %}
