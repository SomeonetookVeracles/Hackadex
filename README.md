# Hackadex
A zero 2w powered pentesting tool designed to look like a retro game console

I love the idea and feel of the flipper zero, but I feel like it's missing in a lot of areas when it comes to functionality -- specifically when it comes to wifi. I'm studying to get my CEH (certified ethical hacker) certification currently, and I believe that making a project like this will help me cement the core ideas and principles more than routine studying. I plan on adding the following stuff currently
- A TFT touchscreen with indicator lights
- 2 USB C Ports for data and maybe power
- A decently sized battery for portability (I'm thinking 10000 MaH currently but it depends on price)
- ESP-32 chip for extra wifi functionality
- A U.FL connector on the outside for increased signal strength
- And a 3 stage switch to alternate between on, a low power mode, and off.
- programmable neopixel indicators
- BadUSB compatibility
- a battery controller for maximum efficiency.

There's a lot here, and I'm not sure I'll be able to get everything on it, but I want to at least document everything I'm working towards on this.

## September 9th
I started off by getting a general idea of how much space I'd have to work with. Because I'm lazy, I'll just be stealing the dimensions of the gameboy PCB (which is about 100mm by 100mm), but I'll change this depending on my needs

Now, I started by booting up EasyEDA, and immediately realizing I have **zero** clue what I'm doing, I know Kicad well, but this is my first time using Easy. This is just a warning for the future, in case I do anything stupid.










The first view!
<img width="1920" height="1050" alt="image" src="https://github.com/user-attachments/assets/b3357242-cad2-41e6-9843-f2ca17a354b4" />


First off, we need to establish design rules, fortunately, the manufacturer of this, JLPCB, has documentation that's surprisingly robust, so we can just pop over there and establish everything we need:


The layer stackup

<img width="1920" height="1050" alt="image" src="https://github.com/user-attachments/assets/3a94149c-3cba-4fbe-b0ff-4c85ee125181" />

Now, this is where I realize, JLPCB doesn't sell the Zero 2W, so I'm a little screwed on that front, so I'll be looking for a new solution.
