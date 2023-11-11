# NEC PC Engine Duo PCB Reproductions

This repository contains a recreation of the main board PCB for NEC's PC
Engine Duo console. The recreation is based on the available schematics for the
TurboGrafx-16 and additional reverse engineering using scanned images of an
original board's copper layers, so should be a reasonably accurate reproduction.

**NOTE**: In order to use these PCBs successfully you will need to be proficient in:

* Soldering-fine pitched surface mount components.
* In most cases, desoldering said components to obtain these from a donor board.
* Troubleshooting any issues that may arise.

The authors are not obliged to provide support, nor shall they be held responsible
for botched attempts at using these boards.

Should you however find a legitimate flaw in the board's design or have suggestions
for improvements, please feel free to submit an issue. Please note that the current
scope of the project is to provide a working replica; we are not at this moment
entertaining feature requests for significant modifications.


## PCB Production

Minimum track widths, clearances and via sizes are within the standard
offering of modern PCB fabricators. Gerber files are generated with the relevant
options for both [JLCPCB](https://jlcpcb.com/) and [PCBWay](https://www.pcbway.com/).
Placeholders for the order number are provided so remember to select
the "Specify location" option for this when ordering. If using another service
you may wish to remove or replace this placeholder.

The design is verified to work as a 2-layer PCB with 1 oz copper. A leaded HASL
finish is perfectly adequate and ensures compatibility with the original solder
that will ineveitably be left behind on salvaged parts.


## Bill of Materials

Most parts are marked on the board and it is expected that these will be reused
from a donor board. It is completely possible that your particular board uses
different (but compatible) parts so it's advisable to take photos before starting.
For a complete BOM, consult the generated [Interactive BOM][IBOM] or the KiCad
project itself.

Some parts may be different, extra or not present on revisions other than the
particular board this reproduction is based upon. It is probably not feasible to
list the differences between all possible revisions but should you work out a
solution for a particular donor board, please let us know so we can include it in
this documentation.

Capacitor voltages may exceed those given, within reason. E.g. you may
substitute 16V for a 10V part. Do not, however, use a lower voltage than
specified. No voltage is specified for the ceramic capacitors; any 0805 part is
expected to exceed the required voltage anyway.


## Thanks

  * Simon "Aergan" Lock ([@Aergan](https://github.com/Aergan)) for providing
    the donor hardware and testing support.

  * Leo Oliveira, Zaxour, Chrissy ([@chris-jh](https://github.com/chris-jh))
    and Dennis (@PointerFunction) for their insights and support when
    testing the prototype board.

  * Rob Taylor ([@PeepoUK](https://github.com/PeepoUK)) for the groundwork
    on the original [PC Engine reproduction](https://github.com/Board-Folk/PC-Engine)
    project which served as a base for this one.

  * The rest of the Board Folk for their support and general coolness.


## Legal

As the product of this project is a replica of a proprietary product, the
the author makes no claim of copyright to the schematics nor PCB layouts and
releases these into the public domain, solely for the purposes of study and
historical preservation.

You are free to produce PCBs based on this project's designs at your own risk
and without limitation, for your own use or for sale and/or repair at a
reasonable price. Attribution is appreciated. The authors are not obliged to
provide support of any kind.

Under no circumstances will the authors be held responsible or liable in any
way for losses, damages or costs resulting from the use of the information
and/or resources of this project.

The resources are provided "as-is" without warranty of any kind, either
expressed or implied, including, but not limited to, the implied warranties
of merchantability and fitness for a particular purpose.

[IBOM]: http://htmlpreview.github.io/?https://raw.githubusercontent.com/Board-Folk/PC-Engine-Duo/master/bom/ibom.html
