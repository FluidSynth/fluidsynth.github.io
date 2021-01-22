---
title: Bug in SDL2_Mixer will crash fluidsynth
author: Tom Moebert
layout: post
---

A bug in SDL2_Mixer <= 2.0.4 will crash fluidsynth >= 2.1.6 because the objects are destroyed in an illegal order. Until there is an official bug fix release for SDL2_Mixer, packagers are encouraged to add the following upstream patch to their distribution package:

https://hg.libsdl.org/SDL_mixer/rev/b0afe341a91d
