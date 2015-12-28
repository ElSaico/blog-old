.. title: Automation Track Builder
.. date: 2014-08-06 14:40:46
.. author: Bruno Marques
.. category: Projects
.. tags: web, angular.js
.. slug: 2014-08-06-automation-track-builder

Time to talk about the first (and so far only) open-source project that I created
and maintain consistently (yes, Kiwi Krossing is on hiatus - shame on me!) - the
[Automation Track Builder](http://github.com/ElSaico/automation-track-builder).

## What
This is an auxiliary web application for [Automation](http://www.automationgame.com),
a “car company tycoon” game under development where you design cars and engines from scratch.<br/>
Currently, there are Multiplayer, Scenario and Sandbox modes available, and the finished version
will present a Campaign mode *a la* Detroit.

One of the car designer’s features is the possiblity of choosing a track and
setting a lap on it. There are two available from the start, and more can be created
and downloaded.<br/>
The process of track creation used to be somewhat cumbersome, involving manual
editing of Lua files and a lot of trial and error. This application was designed
to facilitate it - you can start from scratch (or import an existing track) and
edit everything visually.

You can access it [here](http://uberwald-dev.net/automation-track-builder). Fellow
forumite 07CobaltGirl made a [tutorial](http://automationgame.com/phpBB3/viewtopic.php?f=36&t=4179)
that helps learning its functionality.

## How
This app was made possible thanks to several JavaScript libraries. In particular:

* [AngularJS](http://angularjs.org), the main framework
* [Fabric.js](http://fabricjs.com), for drawing the track preview
* [luaparse](http://oxyc.github.io/luaparse), a JS parser for Lua source files - used to import existing track files
* [mustache.js](https://github.com/janl/mustache.js), a template system used to export the tracks to the Automation format

Not to mention libraries such as [Grunt](http://gruntjs.com/) and [Bower](http://bower.io/),
which automate a significant chunk of the development process and make working with
JavaScript much easier.<br/>
With their aid, web applications are very viable choices for portable development
and smooth deployment.
