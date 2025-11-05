# Fork
Thanks to Chineko-Koizumi for the great work!
I updated as follows:
Made FILAMENT_LOAD as well as FILAMENT_UNLOAD makro. 
For this it is necessary to have a vetry exact measurement of your bowden tube length including lenght inside feeder and about 20mm inside toolhead.
I uncoupled the bowden tube from toolhead an loaded filament through the feeder with force moves, e.g. <FORCE_MOVE STEPPER="extruder_stepper support_extra_stepper" DISTANCE=100 VELOCITY=40 ACCEL=500>. If the filament is at the end of the bowden tube add 20mm and you have your length. You can use FORCE_MOVE as well with negative values. My bowden tube is 1856mm (it is longer because of different routing).
To avoid very hot buffer stepper motor you can try to change run current. My one is running weith 
run_current: 0.8
hold_current: 0.8
Still enough power and a little cooler. I don`t need the cooling case for it. It is running at a max of 60°C.


# ORIGINAL DESCRIPTION
https://github.com/Chineko-Koizumi/SV08MAXCustomFeeder
