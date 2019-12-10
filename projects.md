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
