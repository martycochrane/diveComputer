# MPC Dive Computer Toolkit

## Motivation

As I "dive" more into the world of recreational and technical scuba diving I've struggled to find one place to log all of my dives across various different dive computers. There are some nice mobile apps and also some tool kits like [MultiDeco](https://www.hhssoftware.com/multideco/) for understanding different gasses and decompression stops however not really one place to store all of my information and plan future dives.

I want to understand more about different decompression algorithms and generally it's not overly transparent how each of these work on different dive computers. I find it easiest to learn these things by either teaching or writing my own solutions to do the calculations which is one of the reasons I've decided to start to create this toolkit

[Subsurface](https://github.com/subsurface/subsurface) is the best toolkit I've found so far but it's very complicated for a newbie to understand how to plan a dive etc. It's also missing some key functionality I want so I've decided to start building my own but as I learn while building my own I'd like to try and create PR's to subsurface with any additional functionality I can add to their solution

### Language Choice

Originally I was going to build this using go and [fyne](https://github.com/fyne-io/fyne) as I find that combination really clean as a development environment and also nicely cross platform to allow a nice user experience with installation and useability.

I ended up choosing python and QT as the python community is better for mathematical libraries and also because I wanted to build my own skills with using QT which is something I've not used too much in the past.

## Goals / Features

Ability to import dives from popular dive computers or apps like
 - Oceanic+
 - SSI App
 - Mares Computers
 - Garmin Computers

 Store all of your dives in one location. (probably to a common cloud storage solution like dropbox)

 Nicely view all of your dives and as much nice information as possible about each dive

 Understand and plan what dives can look like with different dive gases and different accent rates

 Compare different decompression algorithms

 Add your Padi or SSI certs so you can show digitally to dive centres etc. Also helps with planning dives. Eg if you're Padi Advanced then software should automatically know you should not go beyond 30m depth

 Make same available on iphone & android devices

 Maybe see if there is a way to make a PR to [Subsurface](https://github.com/subsurface/subsurface) to add any additional functionality I build here to their repo.

## Todo List

- [ ] Import uddf Dives
- [ ] Create simple QT desktop application and test across different platforms
- [ ] Test on iPhone
- [ ] Display simple values from imported uddf dives
- [ ] Create cloud storage solution to sync across devices (probably google dive or dropbox)
