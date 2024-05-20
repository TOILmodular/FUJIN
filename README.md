# FUJIN
This Eurorack module provides a kind of wind or noise machine with four different selectable noise types, blue, white, pink, and a grainy white noise (meaning that the noise signal is peaking only occasionally with the frequency of peaks being controllable).

The module contains a state-variable filter with selectable modes, lowpass, bandpass, and highpass.

The output signal is send to two separate VCAs and two separate output channels.

There is CV control for the filter cutoff, which is following the 1volt/oct standard for the filter self-resonance, as well as CV control for the filter resonance.

<img height="500" src="https://github.com/TOILmodular/CONTINUUM/assets/97026614/9aa25208-d464-4d61-b3e9-2e5df699201f">
<img height="500" src="https://github.com/TOILmodular/CONTINUUM/assets/97026614/58ca1409-5d84-451c-b231-6b8a6a3aa704">

A demo of the module is available in this YouTube video:

<img width="500" src="https://github.com/TOILmodular/FUJIN/assets/97026614/6e20f427-5a2c-4069-b416-353bc8a022fa">

## Module Build and PCBs
I added two different versions for the control board in the folder GerberFiles, an "original", and a "Thonk" version.
Reason is that for my own module, I am using specific potentiometers - 16K4 series from Supertech Electronics - and 3.5mm jack sockets - MJ-355 from Marushin - available at my local electronics shop.

<img width="300" alt="CtrlPCB_Orig" src="https://github.com/TOILmodular/FUJIN/assets/97026614/8f17df41-11c8-4d36-8c2c-b37f129190d1">

However, since most DIY projects for Eurorack modules out there are using potentiometers from ALPHA and so-called THONKICONN jacks, as they are provided by Thonk in the UK, I also created another control board PCB for the "Thonk" version with footprints for those components.

<img width="300" alt="CtrlPCB_Thonk" src="https://github.com/TOILmodular/FUJIN/assets/97026614/ce6a1bbc-a053-4b08-a7f0-3a410ccd49d4">

The main PCB is the same for both versions.

<img width="300" alt="MainPCB" src="https://github.com/TOILmodular/FUJIN/assets/97026614/dc94dd6e-d988-4a71-9a45-64ae2f939674">

I created the Gerber files with the online tool EasyEDA and ordered the PCBs at JLCPCB.

## Additional Information about specific Components
The module build is mainly THT, including all ICs.
However, there are a number SMD capacitors with the package size 1608 (imperial 0603) and a few MMBT3904/MMBT3906 transistors, package size SOT-23-3.

For the "Original" version three of the IC sockets on the control board need to be soldered in a specific way, as described in the next section. For the "Thonk" version, all sockets are to be soldered the usual way.

Concerning the resistor size, I am usually using small-size resistors, about half the length of the usual size, so they need less space on the PCB. If you want to use my Gerber files, you have to consider that fact. You might still use normal size resistors and put them in a standing position on the boards. Should also work fine.

## Soldering IC Sockets on Control Board (only valid for the "Original" PCB version!)
The following information is not relevant, if you are using the "Thonk" version PCB.

There are three IC sockets to be soldered on the control board in a special way, although the ICs themselves are THT.
Due to space reasons, there are no holes for the IC sockets.
The socket legs need to be soldered to the PCB surface, like SMD components.

In order to do that, you need to use the type of sockets, where the legs can be bent, NOT the ones with stiff round legs!

<img width="500" src="https://github.com/TOILmodular/GARGLER/assets/97026614/440ea4bd-f64a-49aa-b3e9-e93ae8265c44">

All socket legs need to be bent to the outside, so they can be put flat onto the PCB. Soldering the socket to the board is very easy, since the legs and the space inbetween are big compared to real SMD components.

<img width="500" src="https://github.com/TOILmodular/GARGLER/assets/97026614/437a25b2-b9cc-4be9-bf65-0ad2c10efac4">
<img width="500" src="https://github.com/TOILmodular/GARGLER/assets/97026614/31184858-4c74-43f4-b11a-abf582f29de1">

All other sockets on the control board and the ones on the main board are to be soldered the usual THT way.
