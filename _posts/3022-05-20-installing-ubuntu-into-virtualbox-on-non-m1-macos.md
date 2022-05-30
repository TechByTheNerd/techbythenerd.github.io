---
title: Installing Ubuntu into VirtualBox on (non-M1) macOS
date: "3022-05-30 12:44"
categories: [Infrastructure, Homelab]
tags: [homelab, virtualbox, ubuntu, macos, infrastructure, virtualization]
published: false
---
## Overview

Suppose you want to play around with Linux and maybe you've heard people talking about [Ubuntu](https://www.ubuntu.com). But you don't have an extra computer laying around to try it, and you certainly don't want to replace your main computer with this experimental idea. What should you do?

Enter "virtualization". In modern day, pretty much any computer can host a [hypervisor](https://www.vmware.com/topics/glossary/content/hypervisor.html). That is, a piece of software that can host a virtual computer, inside of your actual computer. Meaning, you could create a "virtual machine" on your main computer, and try out Ubuntu on that virtual machine, or VM. When you are done, you can delete it, install other operating systems, etc.

## What You'll Need

There's really two things you need here, a hypervisor of some sort, and some installation media for the operating system that you want to install.

### PART 1: A Hypervisor

On macOS, you have a couple of choices, but for a few reasons, we'll cover how to set up VirtualBox. First, navigate to:

- **[www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)**

From here, there are two things to download:

- **Platform Package** - click on "OS X hosts" to download a `.dmg` file. This is the main hypervisor software and user interface.
- **Extension Pack** - click on "All supported platforms" to download a `.vbox-extpack` file. This has some extended functionality that is useful.

They upgrade VirtualBox all of the time, but here is a snapshot of what this looks like on the day of this writing, and what to click on:

![What to download](/assets/img/virtualbox-what-to-download.png)

Next, in your Downloads folder double-click the `.dmg` file to mount the installation image.

![Downloads folder](/assets/img/virtualbox-downloads.png)

That brings up the installer:

![VirtualBox Install Launcher](/assets/img/virtualbox-installer.png)

### PART 2: Installation Media