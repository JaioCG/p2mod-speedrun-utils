**Designed for Danger:**
```sar_speedrun_cc_start "Designed for Danger"
sar_speedrun_cc_rule "Start" load action=start map=dfd_1_intro 
sar_speedrun_cc_rule "Finish" entity action=stop map=dfd_8_adventure2 targetname=end_fade inputname=Fade
sar_speedrun_cc_finish
sar_speedrun_category "Designed for Danger"
```

**Welcome Back:**
```sar_speedrun_cc_start "Welcome Back"
sar_speedrun_cc_rule "Start" load action=start map=sp_intro 
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_bts2 targetname=@changelevel inputname=Changelevel
sar_speedrun_cc_finish
sar_speedrun_category "Welcome Back"
```

**Aperture Ireland:**
```sar_speedrun_cc_start "Aperture Ireland"
sar_speedrun_cc_rule "Start" load action=start map=ep1_testchmb_00
sar_speedrun_cc_rule "Finish" entity action=stop map=ep2_finale targetname=anti_cmb_thrown_down inputname=Cancel
sar_speedrun_cc_finish
sar_speedrun_category "Aperture Ireland"
```

**Mind Escape:**
```sar_speedrun_cc_start "Mind Escape"
sar_speedrun_cc_rule "Start" load action=start map=sp_a260201_room_1alpha
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_a260202_room_5beta targetname=mind_escape inputname=Trigger
sar_speedrun_cc_finish
sar_speedrun_category "Mind Escape"
```

**Portal: Unity Reboot**
```sar_speedrun_cc_start "Portal Unity Reboot"
sar_speedrun_cc_rule "Start" entity action=start map=testchmb00 targetname=blackout_cam inputname=Disable
sar_speedrun_cc_rule "Finish" entity action=stop map=escape00 targetname=a00-a01_elevator_stop inputname=PlaySound
sar_speedrun_cc_finish
sar_speedrun_category "Portal Unity Reboot"
```

**P1 Done P2 (Splits on Chambers):**
```sar_speedrun_cc_start "P1 Done P2 Chambers RTA" action=split
sar_speedrun_cc_rule "Start" entity action=force_start targetname=trigger_knockout_teleport inputname=Disable map=testchmb_a_00
sar_speedrun_cc_rule "01 Start" entity targetname=elevator_body_middle inputname=Stop map=testchmb_a_00
sar_speedrun_cc_rule "03 Start" entity targetname=a01-middleelevator_body inputname=Stop map=testchmb_a_01
sar_speedrun_cc_rule "05 Start" entity targetname=a02-middle_elevator_body inputname=Stop map=testchmb_a_02
sar_speedrun_cc_rule "07 Start" entity targetname=a03-middle_elevator_body inputname=Stop map=testchmb_a_03
sar_speedrun_cc_rule "12 Start Inbounds" entity targetname=07a_07b_elevator_body inputname=Stop map=testchmb_a_07
sar_speedrun_cc_rule "Finish" entity action=stop targetname=glados_destruction inputname=Start map=escape_02
sar_speedrun_cc_finish
sar_speedrun_category "P1 Done P2 Chambers RTA"
```

**P1 Done P2 (Splits on Maps):**
```sar_speedrun_cc_start "P1 Done P2"
sar_speedrun_cc_rule "Start" entity action=start map=testchmb_a_00 targetname=trigger_knockout_teleport inputname=Disable
sar_speedrun_cc_rule "Finish" entity action=stop map=escape_02 targetname=glados_destruction inputname=Start
sar_speedrun_cc_finish
sar_speedrun_category "P1 Done P2"
```