# tdh.lib
A collection of abstractions for Pure Data<br>
<br>
Here you will find a collection of abstractions I have developed for my own projects or for instruction/educational purposes.<br><br>
Some abstractions are integral building blocks for my code (and can be for your code!), some are modules with user interfaces for higher-level programming. Some of these user-interface (.ui) modules are graphic front-ends for other programmer's excellent objects (such as UI versions of ELSE objects), some are graphic front-ends for core Pd functionality that are then ported over to my collection of modules for sonic exploration for those new to Pd, the SOUND ART TOOL KIT (<https://github.com/thouldcroft/tdh.satk/>), so you may be scratching your head wondering why a certain object exists - its likely then an object that is intended for the SATK to give a specific limited set of modules to the user.<br><br>
<b>This library requires the ELSE (<https://github.com/porres/pd-else/>) and CYCLONE (<https://github.com/porres/pd-cyclone/>) libraries to run.</b> While I have strived to keep tdh.lib as vanilla as possible, there have been times when I just didn't have the programming skills to do so. Both libraries are availble via Deken, and are preinstalled in PlugData.<br><br>
This library is very much a work in progress and may not be backwards compatible from version to version, but I will strive to make minimal changes. If a patch using my library breaks, check inlets, likely they were just changed (this is the most common change to existing objects).

## General Conventions<br>
All objects follow the naming syntax "tdh.[category].[abstractionName]". <br>

### Categories<br>
#### Algorithmic Composition (ac.---)
Abstractions for the algorithmic generation of sonic composition, musical or otherwise.
#### Control
These are mostly abstractions that serve as UI controllers mainly to be ported over to the SOUND ART TOOL KIT.
#### Math (math.---)
Abstractions for calculation, some simple, some complex.
#### Sequence (seq.---)
Abstractions for sequencing events.
#### Signal Processors (sigproc.---)
Signal processors that operate on signal rate data.
#### Synthesis Modules (synth.---)
Abstractions for synthetic sound generation. Many draw on modular synthesis design foundations.
#### Utilities
More or less, everything else. This includes:
  - Routing matrixes
  - Panning and mixing tools
  - Envelope/ramp tools
  - Audio-file playback
  - Audio I/O
  - Audio recording
  - GUI tools
  - Audio graphic displays
  - Patching tools
  - Clock tools
  - Graphic front ends for arrays/data tables
  - Graphic front ends for general patching mechanics, mostly intended for the SOUND ART TOOL KIT
  - Remote send modules, intended for the SOUND ART TOOL KIT

All abstractions that end with a tilde ('~') can be assumed to accept and/or output data at audio rate.

Many abstractions have help files ([abstractionName]-help.pd) but many do not. Abstractions with help files should be considered much more stable/robust than abstractions without.

An attempt has been made to comment the abstractions as much as possible, so that new users to Pd could potentially learn from the code, however, I can't guarantee that every abstraction has been thoroughly documented. Additionally, an attempt at a coding style/syntax has been attempted, but this style has developed over the years of building this library, and as such, consistency may be lacking at times.

It is assumed that you are using the newest version of Pd when working with these abstractions.
<br>
## License
Copyright (C) 2024  Travis Houldcroft<br>
thouldcroft@gmail.com<br>
<https://www.travishouldcroft.com/> 

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.<br>

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.