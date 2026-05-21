VAG / VW reverse-engineering notes
===================================

This is a dump of some notes I took while reverse engineering the CAN/BAP
communication on a VW Golf Mk 6.

The notes are incomplete, and may contain misinterpretations of observed
communication. Since they are quite old and I don't have the time to work
on them anymore, I'd rather have them out in the open than lost to time.


Sources
--------

The vendor specific MDI protocol has been reverse engineered entirely
from wire traces between an RCD 310 head unit and a MDI device.

A few other traces of simpler CAN messages have been observed on the
infotainment CAN bus of a Golf Mk 6.


Acknowledgements
-----------------

Special thanks go out to tmbinc who laid out the simplicity of BAP in
his talk on hacking his handsfree unit in his Golf Mk 6:

  https://media.ccc.de/v/30C3_-_5360_-_en_-_saal_2_-_201312281600_-_script_your_car_-_felix_tmbinc_domke
  https://github.com/tmbinc/car
  https://github.com/tmbinc/kisim/


Acknowledgements
-----------------

Special thanks go out to tmbinc who inspired me to do this, and
laid out the simplicity of BAP in his talk on hacking his handsfree
unit in his Golf Mk 6:

  https://media.ccc.de/v/30C3_-_5360_-_en_-_saal_2_-_201312281600_-_script_your_car_-_felix_tmbinc_domke
  https://github.com/tmbinc/car
  https://github.com/tmbinc/kisim/


Disclaimer
-----------

The author(s) take NO responsibility whatsoever for any damage, safety
issues, or anything else, be it in a lab setup or in an actual car.


Licence
--------

GNU GPL v2 only.

Please see the file COPYING for details.
