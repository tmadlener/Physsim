# v00-04-02

* 2021-08-16 Valentin Volkl ([PR#1](https://github.com/iLCSoft/Physsim/pull/1))
  - Add explicit include for TString.h to avoid build failure with ROOT v6.24

# v00-04-01

# v00-04

# v00-03
- original version by Junping & Keisuke...

- F.Gaede
  - made compatible w/ c++11	
  - remove -Wall -ansi


# v00-01
- original version by Junping & Keisuke...

1.) Physsim -- a matrix element package, consists of mainly two libraries, HELLib which is essentially C++ version of HELAS (HELicity Amplitude Subroutines, cf original manual by H.Murayama, etc.), and LCME which provides Matrix Element calculation for various e+e- processes. (note: there exists another independent generator which is also called Physsim, since core part of the Physsim here in ilcsoft is quite similar and developped mainly by Keisuke, we would like to keep the same name.)

2.) Pros of this package are mainly defined by HELAS, such as any tree level Feynman diagram can be calculated with sufficient precision up to 100 TeV? in a very compact and fast way. One of obvious Cons is that Feynman diagrams for given final states need to be treated by hand, which however is not expected to be a real problem, because analysts will eleminate most of the background processes and focus on several signal (or one) and dominant background processes where matrix elment method is supposed to help.

3.) This first versin provides major Higgs production processes, LCMEZH, LCMENNH, LCMEEEH, LCMEZHH, LCMENNHH, for obvious reason. There is plan to implement all useful e+e- processes in future. You are welcome to join the effort.

4.) It is expected to be used in Marlin Processors, cf examples in "example_stdhep" subdirectory which give you some hints how matrix element can be calculated for each event in your analysis processors (actually very straightforward, all you need provide are four momentum of final state particles).

5.) Some introduction can be found in the talk by JT @ AWLC14.
https://agenda.linearcollider.org/getFile.py/access?contribId=167&sessionId=14&resId=0&materialId=slides&confId=6301
