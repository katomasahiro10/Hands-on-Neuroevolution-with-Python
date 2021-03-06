# Instructions

This module provides C++/TensorFlow interfaces that operated similarly to OpenAI's gym library. Since it was built to remove python from the critical portion of the code (simulations) it provides a significant speed up when operating in a multithreading environment.
We currently provide 2 environments utilizing the interface, Atari and Hard Maze. 

## Building Module with Atari Environment

 Our Atari support is licensed under GPLv2 and instructions on how to use it can be found under the `./atari` folder.

 Please follow these instruction to build Atari environment first and after that build this module by running `make`

## Building Module without Atari Environment 

 To compile this module simply open the `Makefile` to adjust settings (USE_GPU, USE_ALE, etc), once configured run `make` to build from source.

 To disable Atari support set in the `Makefile` parameter `USE_ALE` to have value zero as follows:
 
 `USE_ALE := 0`