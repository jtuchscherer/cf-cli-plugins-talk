<!-- .slide: class="titlePage" -->

## Intro to Cloud Foundry

#### A guide to the Clouds

Note:
Welcome and Introduction

---

## What is Cloud Foundry

Let's take a look <!-- .element: class="fragment" data-fragment-index="1" -->
<br/>
![Thanks](./images/CloudFoundry.jpg) <!-- .element: class="fragment" data-fragment-index="1" -->

Note:
Josh showed this very nicely

---

## What is Cloud Foundry
<br/>
Just some additions
<br/><br/><br/>
Note:
There are only a few additional things to mention

---

## Cloud Foundry is a PaaS
<br/>

SaaS - Features <!-- .element: class="boxes" -->

Platform - Applications <!-- .element: class="boxes" -->

Infrastructure - VMs <!-- .element: class="boxes" -->

Bare Metal - Server<!-- .element: class="boxes" -->

Note:

---

## How does it work

---

![Detour](./images/detour.png)
<br/>
### What is a Linux container

--

### Linux container

![Docker Docker Docker](./images/dockerdocker.png) <!-- .element: class="fragment" data-fragment-index="1" -->

--

### Linux container

* Tools in the Linux Kernel to isolate processes
* Lightweight virtualization
* Linux filesystem + metadata

--

![Containers](./images/containers.png)

<small class="quote-source">
Credit: [Boden Russel, VMware](http://www.slideshare.net/BodenRussell/realizing-linux-containerslxc)
</small>

--

### chroot

![chroot man page](./images/chroot.png)

* Added to Unix Kernel in 1979 <!-- .element: class="fragment" data-fragment-index="1" -->
* Launch process under in a self-contained directory <!-- .element: class="fragment" data-fragment-index="1" -->



--

### cgroups

![cgroups man page](./images/cgroups.png)

* Donated by Google in 2007 <!-- .element: class="fragment" data-fragment-index="1" -->
* Isolate resource (CPU, memory, network...) for processes <!-- .element: class="fragment" data-fragment-index="1" -->

--

### namespace isolation

![namespace man page](./images/namespaces.png)

* Been around for a long long time <!-- .element: class="fragment" data-fragment-index="1" -->
* Isolate PIDs, users, mount points from processes <!-- .element: class="fragment" data-fragment-index="1" -->

--

### Timeline

<div style="float: left; text-align: left; padding-right: 60px; margin-right: 20px; border-right: 1px solid white;">
1979 chroot <br/>
2000 BSD jails <br/>
2004 Solaris Zones <br/>
2007 cgroups in Linux <br/>
2008 LXC <br/>
</div>

<div style="text-align: left;">
2011 CF Warden <br/>
2013 Docker <br/>
2014 Rocket <br/>
2015 OCI <br/>
</div>

---

### Back to CF

More history

---

## 2009 - The beginnings

Simple Deployment Experience

Note:
- Dual start with Spring Source and VM Ware
- Simple push experience
- Demo:
  Scaling
  Health Monitor

--

## Pushing an app

![Staging](./images/staging.png)

--

## Running an app

![Running](./images/running.png)

--

## App Health Management

![Running App](./images/restarting_1.png)

--

## App Health Management

![Crashing App](./images/restarting_2.png)

--

## App Health Management

![Recovering App](./images/restarting_3.png)

---

## 2011 Warden

Multi-tenancy

Note:  
- Talk about Warden and Isolation before Warden

---

## 2012 Bosh

Ease of deployment and operations

Note:  
- CPIs and Bosh awesomeness

--

![BOSH](./images/bosh.png)

--

![Bosh VMS](./images/bosh-vms.png)

---

## 2013 Service Brokers

Connecting Apps and Services

Note:  
- all the buildpacks

--

## Binding a service

![Service Binding](./images/service.png)


---

## 2013 Buildpacks

Multi-language

Note:  
- all the buildpacks

---

## 2014 Logging and Metrics

Keep your apps running

Note:  
- show logs and metrics

--

## Log aggregation

![Loggregator](./images/logging.png)

---

## 2015 Diego

Run Docker container and Windows apps

Note:  
- Talk about Diego's impact

---

## 2015 Foundation

Cloud Foundry Foundation

Note:  
- OSS community

--


### Foundation

![Cloud Foundry Foundation - Part1](./images/foundation1.png)

Note:
- Docker
- Anynines


--

### Foundation

![Cloud Foundry Foundation - Part2](./images/foundation2.png)


Note:
- SAP
- IBM (co-opetition)
- MimaCom
- bunch of other big names


---

## 2016 Azure and Google Cloud

Cloud Foundry everywhere

Note:  
- they did the integration

---

## How can I try it

* Pivotal Web Services
* BlueMix
* Anynines
* [...]

* Locally: Bosh-Lite, PCF Dev, CF Local

---

## When not to use CF

<span class="fragment fade-in">
	<span class="fragment fade-out">Local File System</span>
</span>

<span class="fragment fade-in">
	<span class="fragment fade-out">More than one port per app</span>
</span>  

<span class="fragment fade-in">
  <span class="fragment fade-out">Incoming traffic other than HTTP</span>
</span>      

<span class="fragment fade-in">
  <span class="fragment fade-out">Lots of app-to-app traffic</span>
</span>

<span class="fragment fade-in">Huge memory requirement</span>


---

## Thank you

May the Clouds be with you

jtuchscherer@pivotal.io
