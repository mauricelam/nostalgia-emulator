An Emulator Configured to Run Nostalgia-Inducing Games in a Browser
=====

a.k.a. Little Fighter 2 in a browser

## Usage

1. Navigate to https://mauricelam.github.io/nostalgia-emulator/
2. Enjoy

## How it works

We are almost in the year 2025, so it's about time for this to happen: [![image](https://github.com/user-attachments/assets/364ea962-390e-424a-9609-1817c81ef0cd)](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript)

Little Figher 2 is a closed-source Windows game, so to run it, we have to emulate the underlying environment.

So we run Windows 95, which is also closed-source, by emulating _its_ environment.

Windows 95 is compiled to work with x86, so we use an [x86 emulator](https://github.com/copy/v86) compiled to webassembly.

The Webassembly is then run by the Webassembly runtime in your browser, like V8 or SpiderMonkey.

It's not as many layers as the GIMP example in the talk, but hey, it's not quite 2025 yet.
