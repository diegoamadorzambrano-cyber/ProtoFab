# ProtoFab  
A machine built for tinkerers and engineers who want more control.  

# Bringing PCB Manufacturing to Your Desk  
This whole thing started because making PCBs at home just felt harder than it needed to be. Sending boards out for fabrication kills momentum. Waiting days for a simple prototype? Yuck. It ruins the fun. And let’s be honest, most desktop CNCs are either too noisy, too messy, or clearly made for woodworkers, not electronics folks. I wanted something that made PCB prototyping feel as instant as opening a CAD file. Something you actually want sitting on your desk, not hiding out in the garage. Instead of just buying a closed-off CNC and twisting my process around it, I built a machine that works with me. Every change in this project happened because I ran into a real roadblock, figured out why, and then redesigned to fix it. So, ProtoFab isn’t just a finished gadget—it’s a living platform that keeps getting better.  

## Project Goals
* Make PCB milling a true desktop thing
* Keep noise, dust, and size friendly for any room
* Focus on rigidity and accuracy, not just movement
* Stay modular so tools and features can keep evolving
* Clean Software
* Iterate endlessly

## Why Build Instead of Buy?
Buying a CNC is definitely faster. But you’re stuck with someone else’s decisions. Most off-the-shelf machines have fixed frames, barely any upgrade paths, and workflows that fight you if you want to do things differently. You end up paying for stuff you don’t care about and missing the pieces you actually need.

With ProtoFab, I traded convenience for control and real understanding. Every joint, every rail, and every bit of software exists because something earlier just wasn’t strong, accurate, or flexible enough. My goal isn’t to beat commercial machines on paper—it’s to build something that nails my needs better than a generic solution ever could.


## PCB First, Everything Else Second  
Most hobby CNCs are built around wood first, PCB milling second. ProtoFab flips that. Z-axis consistency, probing accuracy, and flatness aren’t upgrades—they’re the whole point. Conductive probing is baked right in, so leveling a PCB is routine, not a weird workaround.



## Development Stages

### V1 – Proof of Concept
* Mostly PETG structure
* Linear rods, lead screws
* Small, desktop-sized frame
* Prioritized motion and geometry over stiffness

V1 taught me something fast: moving parts don’t mean a stiff machine. Sure, it worked, but the flex in the structure became obvious the moment I tried to push for real accuracy. PETG bends. Gantry connections matter way more than I thought. V1 wasn’t enough.

### V2 – Structural Rethink
* Swapped linear rods for MGN rails
* Moved lead screw behind the gantry
* Redesigned sides with 2020 aluminum extrusions
* PETG only for non-critical parts now
* Multiple brackets to beef up the frame

Here’s where things got serious. I had to push my design skills. The result? A machine that’s strong, rigid, and actually looks like something you’d want on your desk. PETG is still in the mix, but only where it makes sense for quick tweaks or electrical isolation. Now, parts feel designed, not improvised.

### V3 – Planned Refinement (Work in Progress)
* Replace the last critical PETG with aluminum
* Fully support and stiffen up the bed
* Lighten up the Z-axis
* Add an enclosure
* Refine spindle and laser mounts
* Add vacuum and filter to the CNC
* ATC... maybe?

V3 isn’t about patching up flaws—it’s about smoothing out what works. At this point, ProtoFab should feel solid and reliable, not something you have to babysit. I’m also adding some quality-of-life features and a bit of custom software.

## Software  
The brains: MKS DLC32 MAX, running GRBL on an ESP32. Instead of just slapping on a generic interface, I’m tweaking the firmware to fit real CNC workflows. That means ditching pointless 3D printer features and adding tools for probing, leveling, and tool changes the way this machine actually needs. Software gets the same treatment as hardware: keep it simple, clear, and easy to adapt.

## What This Project Is Really About  
Honestly, ProtoFab isn’t just about building a CNC. It’s about understanding how and why machines are built the way they are. It’s about learning what real stiffness feels like, and getting comfortable with constant iteration. Every version exists because the last one taught me something I couldn’t ignore.

The goal? Make PCB manufacturing feel like a natural part of your workspace—so that the machine evolves along with your ideas.
