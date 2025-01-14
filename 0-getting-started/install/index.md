---
layout: documentation
title: Installing RethinkDB
docs_active: install
permalink: docs/install/
alias: install/
---
<section class="supported-platforms">
    <section class="platform-category">
        <h2>Official packages</h2>
        <ul class="platform-buttons">
            <li>
                <a href="ubuntu/">
                    <img src="/assets/images/docs/install-platforms/ubuntu.png" />
                    <p class="name">Ubuntu</p>
                </a>
            </li>
            <li>
                <a href="centos/">
                    <img src="/assets/images/docs/install-platforms/centos.png" />
                    <p class="name">CentOS/AlmaLinux/RockyLinux</p>
                </a>
            </li>
            <li>
                <a href="debian/">
                    <img src="/assets/images/docs/install-platforms/debian.png" />
                    <p class="name">Debian</p>
                </a>
            </li>
            <li>
                <a href="https://marketplace.digitalocean.com/apps/rethinkdb-fantasia/?action=deploy&refcode=438afa41d795" target="_blank">
                    <img src="/assets/images/docs/install-platforms/digitalocean.png" />
                    <p class="name">DigitalOcean</p>
                </a>
            </li>
            <li>
                <a href="osx/">
                    <img src="/assets/images/docs/install-platforms/osx.png" />
                    <p class="name">OS X</p>
                </a>
            </li>

            <!--
            <li>
                <a href="windows/">
                    <img src="/assets/images/docs/install-platforms/windows.png" />
                    <p class="name">Windows</p>
                </a>
            </li>
            -->
        </ul>
    </section>
    <section class="platform-category">
        <h2>Community supported packages</h2>
        <ul class="platform-buttons">
            <li>
                <a href="arch/">
                    <img src="/assets/images/docs/install-platforms/arch.png" />
                    <p class="name">Arch Linux</p>
                </a>
            </li>
            <li>
                <a href="opensuse/">
                    <img src="/assets/images/docs/install-platforms/opensuse.png" />
                    <p class="name">openSUSE</p>
                </a>
            </li>
            <li>
                <a href="fedora/">
                    <img src="/assets/images/docs/install-platforms/fedora.png" />
                    <p class="name">Fedora</p>
                </a>
            </li>
            <li>
                <a href="mint/">
                    <img src="/assets/images/docs/install-platforms/mint.png"/>
                    <p class="name">Linux Mint</p>
                </a>
            </li>
            <li>
                <a href="raspbian/">
                    <img src="/assets/images/docs/install-platforms/raspbian.png"/>
                    <p class="name">Raspbian</p>
                </a>
            </li>
            <li>
                <a href="gentoo/">
                    <img src="/assets/images/docs/install-platforms/gentoo.png"/>
                    <p class="name">Gentoo</p>
                </a>
            </li>
        </ul>
    </section>
</section>

{% infobox info %}
<strong>Ready to install the client drivers?</strong> Take a look at [the drivers install page](/docs/install-drivers/).
{% endinfobox %}

- - -

# Docker #

Docker provides an [official RethinkDB repository][docker] on the Docker Hub. To deploy RethinkDB on Docker, run the following command:

    $ docker run -d -P --name rethink1 rethinkdb

You can find unofficial community-supported Docker images on our [Frameworks and Libraries][fnl] list under "Docker images."

[docker]: https://registry.hub.docker.com/_/rethinkdb/
[fnl]: /docs/frameworks-and-libraries/

# Installing on other platforms #

<img class="install-illustration" src="/assets/images/docs/api_illustrations/install.png"/>

## Building from source ##

If your platform isn't listed here, you may still be able to build
from source. You should be able to build RethinkDB on most Linux-based
systems&mdash;check out the generic <a href="/docs/build">build
instructions</a>. If you get RethinkDB running on your platform,
please <a href="/community">contribute</a> a package!

<!--
## FreeBSD ##
Thanks to the efforts of [@hungte] (https://github.com/hungte), RethinkDB has
[experimental FreeBSD
support](https://github.com/rethinkdb/rethinkdb/pull/688). Please help improve
RethinkDB on FreeBSD by testing the build!
-->

## Other architectures ##

Currently the RethinkDB server only supports x86 and x86\_64 architectures on
Unix-based platforms, and has experimental ARM support (thanks to the effort of
[@davidthomas426](http://github.com/davidthomas426)).

Our long-term goal is to port RethinkDB to every widely-used platform. [Get
involved](/community/) in the development effort and help port RethinkDB to
more platforms.

# Older versions #

Binaries for previous versions of RethinkDB are available in the [download archive](https://download.rethinkdb.com).
