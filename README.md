# tdh-lib
A collection of abstractions for Pure Data<br>
<br>
Here you will find a collection of abstractions I have developed for my own projects or for instruction/educational purposes.<br><br>

## General Conventions<br>
All objects follow the naming syntax "tdh.[category].[abstractionName]". <br>

### Categories<br>
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

All abstractions that end with a tilde ('~') can be assumed to accept and/or output data at audio rate.

Many abstractions have help files ([abstractionName]-help.pd) but many do not. Abstractions with help files should be considered much more stable/robust than abstractions without.

An attempt has been made to comment the abstractions as much as possible, so that new users to Pd could potentially learn from the code, however, I can't guarantee that every abstraction has been thoroughly documented. Additionally, an attempt at a coding style/synthax has been attempted, but this style has developed over the years of building this library, and as such, consistency may be lacking at times.

Every attempt will be made to keep all updates to abstractions backwards compatible, so any new features added will not break previously made patches. If this becomes an issue, there will be a note.

It is assumed that you are using the newest version of Pd when working with these abstractions.
