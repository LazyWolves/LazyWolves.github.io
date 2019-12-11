---
layout: default
---

This page contains the projects which are under actice development. All these projects
are under very early or intermediate stages of development, with basic to intermediate
features implemented. Any contribution in form of code, documentation or artwork will
be highly appreciated.

# SaberX

Saberx is a trigger based monitoring, alerting and action execution system which can be used for self healing.

SaberX is a trigger based monitoring, alerting and action execution system which can be used for self healing. SaberX watches for specific events in your system and fires its trigger when any such event happens. In reply to the firing of any such trigger, you can execute an action, like sending alert to you alert management system or any command to heal your system.

A very simple example would be waching your apache server and making sure its accessable at port 80. If its not, then you can configure saberx to fire a trigger for this. When such a trigger gets fired, you may send a curl request call to your alert manager to raise a alert and at the same time restart your apache server.

SaberX provides many more such triggers like filetrigger (watching over files), Process trigger (watching over processes), CPUTrigger (watching over CPU), memory trigger (watching over memory) and the already described TCP trigger (watching over ports).

**Currently SaberX only supports Linux**.

[Read documentation](https://saberx.readthedocs.io/en/latest/)

# ElasticPyProxy

A controller for dynamic scaling of Haproxy backend servers 

ElasticPyProxy (EP2) is a controller written completely in python for dynamically scaling HAProxy backend servers. Using this controller, it is possible to integrate HAProxy with a server orchestrator which spwans servers dynamically and scales out and in very frequently. As of now it provides support for only for AWS however handler for any orchestrator which exposes an API for getting live backends can be added easily.

So, going ahead with aws, it is possible, using EP2 to integrate HAProxy with a AWS Autoscaling Group. Once integrated, the HAProxy backend servers will scale out and in with the ASG of interest. Thus, whenever the ASG spawns a new instance, that instance will get added to haproxy's concerned backend/listener and when the ASG removes a backend, that particular server will also be removed from HAProxy's concerned backend/listener.

[Read documentation](https://elasticpyproxy.readthedocs.io/en/latest/)

# Vision

A lightwieght tool purely written in golang to view remote files

Vision is a light weight tool written purely in golang for viewing remote resources over HTTP. Vision allows you to view config files, log files and other such files over HTTP via your browser or on your terminal.

It allows you to set ACLs via which you can block view on certain resources and alow view on certain resources. It allows you to configure aliases so that you do not have to type the entire path of the resource on server, view a file from top, or bottom, apply regex for filtering contents and specify number of lines to be read form desired files.

[Read documentation](https://github.com/LazyWolves/vision/blob/dev/README.md)
