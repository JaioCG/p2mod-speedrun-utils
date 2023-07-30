**Aperture Ireland:**
```
sar_speedrun_cc_start "Aperture Ireland"
sar_speedrun_cc_rule "Start" entity action=start map=ep1_testchmb_00 targetname=blackout_cam inputname=Disable
// If you're using Vault Save, set sar_speedrun_offset to 3600
sar_speedrun_cc_rule "Vault Start" entity action=start map=ep1_testchmb_00 targetname=green_portal inputname=SetActivatedState
sar_speedrun_cc_rule "Finish" entity action=stop map=ep2_finale targetname=anti_cmb_thrown_down inputname=Cancel
sar_speedrun_cc_finish

sar_speedrun_category "Aperture Ireland"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map ep1_testchmb_00"
```

**Cosmonogy:**
```
sar_speedrun_cc_start "Cosmogony"
sar_speedrun_cc_rule "Start" entity action=start map=cosmogony_release1 targetname=wakeup_camera inputname=Disable
sar_speedrun_cc_rule "Finish" entity action=stop map=cosmogony6_release1 targetname=begin_ending_rl inputname=Trigger
sar_speedrun_cc_finish

sar_speedrun_category "Cosmogony"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map cosmogony_release1"
```

**Designed for Danger:**
```
sar_speedrun_cc_start "Designed for Danger"
sar_speedrun_cc_rule "Start" entity action=start map=dfd_1_intro targetname=blackout_teleport_player_to_surprise inputname=Teleport
sar_speedrun_cc_rule "Finish" entity action=stop map=dfd_8_adventure2 targetname=end_fade inputname=Fade
sar_speedrun_cc_finish

sar_speedrun_category "Designed for Danger"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map dfd_1_intro"
```

**Dilapidation:**
```
sar_speedrun_cc_start "Dilapidation"
sar_speedrun_cc_rule "Start" entity action=start map=sp_dilapidation_p0 targetname=camera inputname=Disable
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_dilapidation_p6 targetname=end_fade inputname=Fade
sar_speedrun_cc_finish

sar_speedrun_category "Dilapidation"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map sp_dilapidation_p0"
```

**Eidolon:**
```
sar_speedrun_cc_start "Eidolon"
sar_speedrun_cc_rule "Start" entity action=start map=sp_a1_beginning targetname=title_fade inputname=Fade
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_a5_eidolon3 targetname=end_titles inputname=Display
sar_speedrun_cc_finish

sar_speedrun_category "Eidolon"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map sp_a1_beginning"
```

**Memories:**
```
sar_speedrun_cc_start "Memories"
sar_speedrun_cc_rule "Start" entity action=start map=Memories_Chapter_I targetname=wake_up inputname=Display
sar_speedrun_cc_rule "Finish" entity action=stop map=Memories_chapter_5_map_4 targetname=outro_fade inputname=Fade
sar_speedrun_cc_finish

sar_speedrun_category "Memories"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map Memories_Chapter_I"
```

**Mind Escape (Splits on Chambers):**
```
sar_speedrun_cc_start "Mind Escape Chambers" action=split
sar_speedrun_cc_rule "Start" entity action=start map=sp_a260201_room_1alpha targetname=cam inputname=Disable
// If you're using Vault Save, set sar_speedrun_offset to 2730
sar_speedrun_cc_rule "Vault Start" entity action=start map=sp_a260201_room_1alpha targetname=p0 inputname=SetActivatedState
sar_speedrun_cc_rule "00" entity map=sp_a260201_room_1alpha targetname=1l--start_elev inputname=StopSound
sar_speedrun_cc_rule "01" entity map=sp_a260201_room_1alpha targetname=2l--start_elev inputname=StopSound
sar_speedrun_cc_rule "03" entity map=sp_a260201_room_2alpha targetname=AutoInstance1-start_elev inputname=StopSound
sar_speedrun_cc_rule "04" entity map=sp_a260201_room_2alpha targetname=2l--stop_elev inputname=PlaySound
sar_speedrun_cc_rule "06" entity map=sp_a260201_room_3alpha targetname=3l--stop_elev inputname=PlaySound
sar_speedrun_cc_rule "08" entity map=sp_a260201_room_4alpha targetname=AutoInstance3-stop_elev inputname=PlaySound
sar_speedrun_cc_rule "10" entity map=sp_a260201_room_5beta targetname=2l--stop_elev inputname=PlaySound
sar_speedrun_cc_rule "15" entity map=sp_a260201_room_8alpha targetname=2l--stop_elev inputname=PlaySound
sar_speedrun_cc_rule "Felix" entity map=sp_a260202_room_2beta targetname=InstanceAuto9-railsystem_1 inputname=Toggle
sar_speedrun_cc_rule "Toxins" entity map=sp_a260203_room_1alpha targetname=prop_portal_n0 inputname=SetActivatedState
sar_speedrun_cc_rule "Airport" entity map=sp_a260203_room_4alpha targetname=airport_tp inputname=Teleport
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_a260202_room_5beta targetname=mind_escape inputname=Trigger
sar_speedrun_cc_finish

sar_speedrun_category "Mind Escape Chambers"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map sp_a260201_room_1alpha"
```

**Mind Escape (Splits on Maps):**
```
sar_speedrun_cc_start "Mind Escape"
sar_speedrun_cc_rule "Start" entity action=start map=sp_a260201_room_1alpha targetname=cam inputname=Disable
// If you're using Vault Save, set sar_speedrun_offset to 2730
sar_speedrun_cc_rule "Vault Start" entity action=start map=sp_a260201_room_1alpha targetname=p0 inputname=SetActivatedState
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_a260202_room_5beta targetname=mind_escape inputname=Trigger
sar_speedrun_cc_finish

sar_speedrun_category "Mind Escape"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map sp_a260201_room_1alpha"
```

**P1 Done P2 (Splits on Chambers):**
```
sar_speedrun_cc_start "P1 Done P2 Chambers" action=split
sar_speedrun_cc_rule "Start" entity action=start map=testchmb_a_00 targetname=trigger_knockout_teleport inputname=Disable
// If you're using Vault Save, set sar_speedrun_offset to 3412
sar_speedrun_cc_rule "Vault Start" entity action=start map=testchmb_a_00 targetname=portal_blue_0 inputname=SetActivatedState
sar_speedrun_cc_rule "01" entity map=testchmb_a_00 targetname=elevator_body_middle inputname=Stop
sar_speedrun_cc_rule "03" entity map=testchmb_a_01 targetname=a01-middleelevator_body inputname=Stop
sar_speedrun_cc_rule "05" entity map=testchmb_a_02 targetname=a02-middle_elevator_body inputname=Stop
sar_speedrun_cc_rule "07" entity map=testchmb_a_03 targetname=a03-middle_elevator_body inputname=Stop
sar_speedrun_cc_rule "12" entity map=testchmb_a_07 targetname=07a_07b_elevator_body inputname=Stop
sar_speedrun_cc_rule "Finish" entity action=stop map=escape_02 targetname=glados_destruction inputname=Start
sar_speedrun_cc_finish

sar_speedrun_category "P1 Done P2 Chambers"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map testchmb_a_00"
```

**P1 Done P2 (Splits on Maps):**
```
sar_speedrun_cc_start "P1 Done P2"
sar_speedrun_cc_rule "Start" entity action=start map=testchmb_a_00 targetname=trigger_knockout_teleport inputname=Disable
// If you're using Vault Save, set sar_speedrun_offset to 3412
sar_speedrun_cc_rule "Vault Start" entity action=start map=testchmb_a_00 targetname=portal_blue_0 inputname=SetActivatedState
sar_speedrun_cc_rule "Finish" entity action=stop map=escape_02 targetname=glados_destruction inputname=Start
sar_speedrun_cc_finish

sar_speedrun_category "P1 Done P2"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map testchmb_a_00"
```

**Portal: Unity Reboot:**
```
sar_speedrun_cc_start "Portal Unity Reboot"
sar_speedrun_cc_rule "Start" entity action=start map=testchmb00 targetname=blackout_cam inputname=Disable
sar_speedrun_cc_rule "Finish" entity action=stop map=escape00 targetname=a00-a01_elevator_stop inputname=PlaySound
sar_speedrun_cc_finish

sar_speedrun_category "Portal Unity Reboot"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map testchmb00"
```

**Wake Up:**
```
sar_speedrun_cc_start "Wake Up"
sar_speedrun_cc_rule "Start" entity action=start map=map1 targetname=FILM inputname=PlayMovie
sar_speedrun_cc_rule "Finish" entity action=stop map=mapcake targetname=credits inputname=PlayMovie
sar_speedrun_cc_finish

sar_speedrun_category "Wake Up"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map map1"
```

**Welcome Back:**
```
sar_speedrun_cc_start "Welcome Back"
sar_speedrun_cc_rule "Start" entity action=start map=sp_intro targetname=start_fade inputname=Fade
// If you're using Vault Save, set sar_speedrun_offset to 1180
sar_speedrun_cc_rule "Vault Start" entity action=start map=sp_intro targetname=elevator_1_body inputname=SetAnimation
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_bts2 targetname=@changelevel inputname=Changelevel
sar_speedrun_cc_finish

sar_speedrun_category "Welcome Back"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map sp_intro"
```

**Wibi!Data:**
```
sar_speedrun_cc_start "Wibi!Data"
sar_speedrun_cc_rule "Start" entity action=start map=sp_lobby_1 targetname=Arrival_Elevator inputname=Open
sar_speedrun_cc_rule "Finish" entity action=stop map=sp_lobby_final targetname=End_UI inputname=Activate
sar_speedrun_cc_finish

sar_speedrun_category "Wibi!Data"
sar_alias do_reset "sar_speedrun_reset; stop; sv_allow_mobile_portals 0; map sp_lobby_1"
```