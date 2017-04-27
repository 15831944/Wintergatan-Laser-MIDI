# Wintergatan Laser MIDI #
![alt text](https://lh3.googleusercontent.com/vT2hciPWMBsPH0dvx-Le0jP9HVhAqWLTJgCErLT-SgyeTtuMMui5nKkZ19TMOimvvXCOPfDBKiEWvT52WHTIVizrnRkbJywZ4FTlYWsA7at_YDL8Lztnifjy-9ISj6qMUlnw-r9VIQU3CchvKhZeG04qAfOOud7QXz3XXtHZZBr_pXYYCruv1l5Xmgr5gT0Da8wzYV6TLtvFK6EpfJ7ksv82wkL3pkTRKtS5AcDnP0nx2MnC5FTosahdTsQ48ZlH73_Jlu4GyQk4B9XM8jTRKCB0tg-jjcwoRixDPsJ0_Olp9X-r71sWnd_eie-iKjWlN0PdC0vTu-YRyeagTDFwZvBTUVbTDIAZYkzFQaY7PxmvuD41dAOjEMmlCLvRXcCwQ1X6zEpxYbg_O-7ULTwNLLloHE1n0yNfDRE2OtYjbBwyEQOmHStdvNh3hJKbDut9cJxALeorr-avh4ZZPT9DAElOZgi8I864jQCLoWR5Gi8tLeNYs8X9_UR4mVK1lVPlsuwVyFWVsrsxeZwqwDiQrPF7ZQ7ukFDrZnW8kFfR1s4VSc1yGPBViAdoxrJG5vyynygGu-1QhbTCmPDFF5jq8kr9juNNE53cqPx08N6gbskxAq5YcBv-EdBUOt5pi-SyetokkhTWLZGqBnuwny-a5_t634XQ-dhc6xZiW9EbFg=w1283-h975-no "Sample generation")

### Description ###
Wintergatan Laser MIDI generates a .scr for AutoCAD from a MIDI file. You can use AutoCAD to control pretty much anything you want in terms of "machining", be it a CNC router, a laser cutter, a 3D printer, an automatic hole puncher... The sky is the limit.

You could also take the cad in .dxf format and convert it into .svg using Inkscape for other machines that can't take raw AutoCAD formats.

### Synopsis ###
`WintergatanLaserMIDI <filename.mid> [(optional) Tone Distance (mm)] [(optional) Beat Distance (mm)]`

#### Arguments ####
filename.mid = MIDI file for which to generate code.

Tone Distance = Defines the distance between every note-pitch. (optional)

Beat Distance = Defines how far away the beats are from each other. (optional)

### Usage ###
    1. Open a new command line window where the executable is located.
    2. Execute the program with the command found above. Keep in mind that Y=0 corresponds to C4!
    3. In AutoCAD, make a new block called PUNCHHOLE. Make sure said block has the dimensions you wish to use for your punch holes (I recommend making a circle shape, but it is not mandatory)
    4. Drag and drop the .scr file generated by the program into the AutoCAD window.

### Latest Version ###
1.0.1

### Latest Changes ### 
#### [1.0.1] - 26-04-2017
- #### Fixed
  - Half-time notes not outputting correctly.

### To do:

 - Watch out for bugs and squash them asap

### Credits ###
[Stephen Toub (stephentoub)](https://github.com/stephentoub) - Making the MIDI C# Library
 
[Ian Ram�rez (ianespana)](https://github.com/ianespana) - Making this program