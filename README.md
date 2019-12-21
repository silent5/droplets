# Droplets

![Droplets Image](Droplets.jpg)

A counter based note sequencer inspired by the excellent Meadowphysics patch/eurorack 
module from monome. Droplets is my attempt at repurposing a few of the ideas presented 
in Meadowphysics for use without a grid, while still trying to maintain an interface 
that invites experimentation and interaction.

Droplets is made up of four note events. A note event is dropped from a certain
height, and when it reaches the ground that note event is triggered. Each note event 
is composed of a base pitch, velocity, duration and probability. A note event drops
at its own clock rate, and features an interval offset list processing section that
enables each note event to create a melody centered on the base pitch. Droplets can
output four independent melodic sequences simultaneously. 

A note event's height can be subject to one of four rules when that note event is
triggered (increment, decrement, positive random offset, negative random offset).


The Droplets interface is made up of three panes:

![Droplets Image](left.jpg)
- The leftmost pane contains 4 color coded sliders. Each of these represent one note event,
and are used to set the height from which a note event will be dropped.

![Droplets Image](middle.jpg)
- The middle pane is used to set the parameters for each of the four note events. It will
change its contents (and color) based on which of the four note events is currently selected.

![Droplets Image](right.jpg)
- The rightmost pane is the global area. It is used for preset management, setting the trigger
rules for each note event, and for setting the global pitch quantization.
