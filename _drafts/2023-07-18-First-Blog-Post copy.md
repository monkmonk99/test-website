---
layout: post
title:  "Trying out NixOS"
info: "Create About/Portfolio theme"
tech : "none"
type: Meta
---

I've been a happy user of the Linux operating system for everything I do in my personal time on a computer for the last 2 years. Throughout that time I have gone through a few distributions, primarily distributions following the normal pipeline for a newer linux user. You know, Ubuntu -> Linux Mint -> Debian -> Fedora. I tried PopOS! for a while after my Nvidia drivers gave out on my lovingly configured Fedora install, as after trying to fix that I had a new found fear of driver updates and found comfort in "It just works" distros.

I've known about NixOS and been interested for a while, but the rockbottom feeling of using PopOS! after Fedora breaking was enough to drive me to it.

# What is NixOS

NixOS is a distribution of Linux which is considered *immutable*, i.e. you can't change what's installed or how things are configured real-time. Now, you can still mutate most of the OS freely, creating files and configuring things through `~/.config` but, as I understand it, there is a section of your OS essentially locked off to you from changing which includes all the packages you install via nixpkgs and quite a bit of the configuration of these packages and other parts of your OS. When you want to change what packages you have installed or the configuration for these packages, you can edit a `configuration.nix` file and run a command to rebuild Nix. Essentially, you are writing a set of build steps to **reproduce** your setup from any other computer.

There's a lot more to NixOS too, such as the ability to roll back to a previous build, including to a build before you updated to a broken package. So if I were using this instead of Fedora when my Nvidia drivers carked it, I likely would have been able to roll back to a previous version of the drivers and continue using my computer, waiting for a working version of those drivers.