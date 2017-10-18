+++
title = "root"
description = "*root* simply specifies the root of where CoreDNS finds (e.g.) zone files."
weight = 24
tags = [ "plugin", "root" ]
categories = [ "plugin" ]
date = "2017-09-15T21:22:42.285957"
+++

The default root is the current working directory of CoreDNS. A relative root path is relative to
the current working directory.

## Syntax

~~~ txt
root PATH
~~~

**PATH** is the directory to set as CoreDNS' root.

## Examples

Serve zone data (when the *file* plugin is used) from `/etc/coredns/zones`:

~~~ corefile
. {
    root /etc/coredns/zones
}
~~~