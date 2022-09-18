# SBC Case Builder


## Introduction

This project is about autonomous SBC case creation. It utilizes the SBC Model Framework project 
to automatically generate cases based on the data for any given SBC contained within the framework.
It uses the Customizer for a graphical user interface for all case attributes.  Cases can be created, 
saved, recalled and edited using the graphical interface after enabling the customizer in the 
OpenSCAD menu->view.  It also supports variable height sbc standoffs to accommodate hats and other add-on 
PCB. Multi-associative parametric positioning of accessories is supported.

License: GPLv3.

![Image](SBC_Case_Builder_Cases.gif)

### Install
```
  git clone https://github.com/hominoids/SBC_Case_Builder.git
  cd SBC_Case_Builder
  git submodule init
  git submodule update

```
### Notes
  
  More information can be found at this [Hard Kernel forum thread](https://forum.odroid.com/viewtopic.php?f=53&t=43948)

### Case Designs and Styles
The case naming convention for standard cases in the configuration file follow the basic form of “sbc”_”design”_”style” e.g. c4_shell or c4_tray_vu5.

#### Current Case Count 368

##### Hardkernel

**Odorid-C1+ cases** - 16 : c1+_shell,c1+_panel,c1+_panel_lcd3.5,c1+_desktop_lcd3.5,c1+_stacked,c1+_tray,c1+_tray_sides,c1+_tray_vu5,
c1+_tray_vu7,c1+_shell_boombox,c1+_panel_boombox,c1+_tray_boombox,c1+_round,c1+_hex,c1+_snap,c1+_fitted

**Odorid-C2 cases** - 17 : c2_shell,c2_panel,c2_panel_lcd3.5,c2_desktop_lcd3.5,c2_stacked,c2_tray,c2_tray_sides,c2_tray_vu5,
c2_tray_vu7,c2_shell_boombox,c2_panel_boombox,c2_deskboom_lcd3.5,c2_tray_boombox,c2_round,c2_hex,c2_snap,c2_fitted

**Odorid-C4 cases** - 17 : c4_shell,c4_panel,c4_panel_lcd3.5,c4_desktop_lcd3.5,c4_stacked,c4_tray,c4_tray_sides,c4_tray_vu5,
c4_tray_vu7,c4_shell_boombox,c4_panel_boombox,c4_deskboom_lcd3.5,c4_tray_boombox,c4_round,c4_hex,c4_snap,c4_fitted

**Odorid-HC4 cases** - 15 : hc4_shell,hc4_shell_drivebox2.5,hc4_shell_drivebox2.5v,hc4_shell_drivebox3.5,hc4_panel,hc4_stacked
,hc4_tray,hc4_tray_sides,hc4_tray_vu5,hc4_tray_vu7,hc4_tray_drivebox2.5,hc4_round,hc4_hex,hc4_snap,hc4_fitted

**Odorid-N1 cases** - 11 : n1_shell,n1_panel,n1_stacked,n1_tray,n1_tray_sides,n1_tray_vu5,n1_tray_vu7,n1_round,n1_hex,n1_snap,n1_fitted

**Odorid-N2 cases** - 9 : n2_panel,n2_tray,n2_tray_sides,n2_tray_vu5,n2_tray_vu7,n2_round,n2_hex,n2_snap,n2_fitted

**Odorid-N2+ cases** - 9 :n2+_panel,n2+_tray,n2+_tray_sides,n2+_tray_vu5,n2+_tray_vu7,n2+_round,n2+_hex,n2+_snap,n2+_fitted

**Odorid-XU4 cases** - 11 : xu4_shell,xu4_panel,xu4_stacked,xu4_tray,xu4_tray_sides,xu4_tray_vu5,xu4_tray_vu7,xu4_round,xu4_hex,xu4_snap,xu4_fitted

**Odorid-XU4Q cases** - 11 : xu4q_shell,xu4q_panel,xu4q_stacked,xu4q_tray,xu4q_tray_sides,xu4q_tray_vu5,xu4q_tray_vu7,xu4q_round,xu4q_hex,xu4q_snap,xu4q_fitted

**Odroid-H2 cases** - 17 : h2_shell,h2_lowboy,h2_lowboy_router,h2_shell_router,h2_shell_routerssd,h2_panel,h2_stacked,h2_tray,h2_tray_sides,
h2_tray_vu5,h2_tray_vu7,h2_tray_router,h2_router_station,h2_round,h2_hex,h2_snap,h2_fitted

**Odroid-Show2** cases - 1 : show2_shell


##### Pine64

**Rock64** - 9 : rockp64_shell,rock64_panel,rock64_stacked,rock64_tray,rock64_tray_sides,rock64_round,rock64_hex,rock64_snap,rock64_fitted

**RockPro64** - 9 : rockpro64_shell,rockpro64_panel,rockpro64_stacked,rockpro64_tray,rockpro64_tray_sides,rockpro64_round,rockpro64_hex,rockpro64_snap,rockpro64_fitted


##### Raspberry PI

**RPIzero** - 9 : rpizero_shell,rpizero_panel,rpizero_stacked,rpizero_tray,rpizero_tray_sides,rpizero_round,rpizero_hex,rpizero_snap,rpizero_fitted

**RPIzero2w+** - 9 : rpizero2w_shell,rpizero2w_panel,rpizero2w_stacked,rpizero2w_tray,rpizero2w_tray_sides,rpizero2w_round,rpizero2w_hex,rpizero2w_snap,rpizero2w_fitted

**RPI1a+** - 9 : rpi1a+_shell,rpi1a+_panel,rpi1a+_stacked,rpi1a+_tray,rpi1a+_tray_sides,rpi1a+_round,rpi1a+_hex,rpi1a+_snap,rpi1a+_fitted

**RPI1b+** - 9 : rpi1b+_shell,rpi1b+_panel,rpi1b+_stacked,rpi1b+_tray,rpi1b+_tray_sides,rpi1b+_round,rpi1b+_hex,rpi1b+_snap,rpi1b+_fitted

**RPI3a+** - 9 : rpi3a+_shell,rpi3a+_panel,rpi3a+_stacked,rpi3a+_tray,rpi3a+_tray_sides,rpi3a+_round,rpi3a+_hex,rpi3a+_snap,rpi3a+_fitted

**RPI3b** - 9 : rpi3b_shell,rpi3b_panel,rpi3b_stacked,rpi3b_tray,rpi3b_tray_sides,rpi3b_round,rpi3b_hex,rpi3b_snap,rpi3b_fitted

**RPI3b+** - 9 : rpi3b+_shell,rpi3b+_panel,rpi3b+_stacked,rpi3b+_tray,rpi3b+_tray_sides,rpi3b+_round,rpi3b+_hex,rpi3b+_snap,rpi3b+_fitted

**RPI4b** - 9 : rpi4b_shell,rpi4b_panel,rpi4b_stacked,rpi4b_tray,rpi4b_tray_sides,rpi4b_round,rpi4b_hex,rpi4b_snap,rpi4b_fitted


##### Nivida

**Jetson Nano** - 9 : jetsonnano_shell,jetsonnano_panel,jetsonnano_stacked,jetsonnano_tray,jetsonnano_tray_sides,jetsonnano_round,jetsonnano_hex,jetsonnano_snap,jetsonnano_fitted


##### Radxa

**ROCKPi 4b+** - 9 : rockpi4b+_shell,rockpi4b+_panel,rockpi4b+_stacked,rockpi4b+_tray,rockpi4b+_tray_sides,rockpi4b+_round,rockpi4b+_hex,rockpi4b+_snap,rockpi4b+_fitted
**ROCKPi 4c** - 9 : rockpi4c_shell,rockpi4c_panel,rockpi4c_stacked,rockpi4c_tray,rockpi4c_tray_sides,rockpi4c_round,rockpi4c_hex,rockpi4c_snap,rockpi4c_fitted
**ROCKPi 4c+** - 9 : rockpi4c+_shell,rockpi4c+_panel,rockpi4c+_stacked,rockpi4c+_tray,rockpi4c+_tray_sides,rockpi4c+_round,rockpi4c+_hex,rockpi4c+_snap,rockpi4c+_fitted


##### Khadas

**Vim1** - 9 : vim1_shell,vim1_panel,vim1_stacked,vim1_tray,vim1_tray_sides,vim1_round,vim1_hex,vim1_snap,vim1_fitted
**Vim2** - 9 : vim2_shell,vim2_panel,vim2_stacked,vim2_tray,vim2_tray_sides,vim2_round,vim2_hex,vim2_snap,vim2_fitted
**Vim3** - 9 : vim3_shell,vim3_panel,vim3_stacked,vim3_tray,vim3_tray_sides,vim3_round,vim3_hex,vim3_snap,vim3_fitted
**Vim3l** - 9 : vim3l_shell,vim3l_panel,vim3l_stacked,vim3l_tray,vim3l_tray_sides,vim3l_round,vim3l_hex,vim3l_snap,vim3l_fitted
**Vim4** - 9 : vim4_shell,vim4_panel,vim4_stacked,vim4_tray,vim4_tray_sides,vim4_round,vim4_hex,vim4_snap,vim4_fitted


##### Asus

**Tinkerboard** - 9 : tinkerboard_shell,tinkerboard_panel,tinkerboard_stacked,tinkerboard_tray,tinkerboard_tray_sides,tinkerboard_round,tinkerboard_hex,tinkerboard_snap,tinkerboard_fitted

**Tinkerboard S** - 9 : tinkerboard-s_shell,tinkerboard_panel,tinkerboard-s_stacked,tinkerboard-s_tray,tinkerboard-s_tray_sides,tinkerboard-s_round,tinkerboard-s_hex,tinkerboard-s_snap,tinkerboard-s_fitted

**Tinkerboard 2/2S** - 9 : tinkerboard-2_shell,tinkerboard-2_panel,tinkerboard-2_stacked,tinkerboard-2_tray,tinkerboard-2_tray_sides,tinkerboard-2_round,tinkerboard-2_hex,tinkerboard-2_snap,tinkerboard-2_fitted

**Tinkerboard R2/R2S** - 9 : tinkerboard-r2_shell,tinkerboard-r2_panel,tinkerboard-r2_stacked,tinkerboard-r2_tray,tinkerboard-r2_tray_sides,tinkerboard-r2_round,tinkerboard-r2_hex,tinkerboard-r2_snap,tinkerboard-r2_fitted


##### Orange PI

**OPI Zero/ZeroPlus** - 9 : opizero_shell,opizero_panel,opizero_stacked,opizero_tray,opizero_tray_sides,opizero_round,opizero_hex,opizero_snap,opizero_fitted

**OPI Zero2** - 9 : opizero2_shell,opizero2_panel,opizero2_stacked,opizero2_tray,opizero2_tray_sides,opizero2_round,opizero2_hex,opizero2_snap,opizero2_fitted

**OPI R1PlusLTS** - 9 : opir1plus_lts_shell,opir1plus_lts_panel,opir1plus_lts_stacked,opir1plus_lts_tray,opir1plus_lts_tray_sides,opir1plus_lts_round,opir1plus_lts_hex,opir1plus_lts_snap,opir1plus_lts_fitted


### Case and Accessory Schema
The schema for case configuration and accessories is documented in the beginning of the file sbc_case_builder.cfg. It has not been finalized and may be subject to changes in the near future as development in these areas is ongoing. Here is a review of the current schema which will be updated as needed for each release. The schema is divided into two areas, case and accessories. There are 30 fixed entries that describe any given case followed by an unlimited number of accessory entries each containing 14 entries.

schema:

    "case_name","sbc_model","case_design","case_style",
    pcb_loc_x,pcb_loc_y,pcb_loc_z,case_offset_x,case_offset_y,case_offset_tz,case_offset_bz,
    wallthick,floorthick,sidethick,gap,fillet,
    indents,sidewall_support,sbc_top_standoffs,sbc_bottom_standoffs,case_ext_standoffs,mode
    sata_punchout,"gpio_opening","cooling","exhaust_vents",
    top_standoff[    6.75,     // diameter
                       18,     // height (top_height)
                      2.5,     // holesize
                       10,     // supportsize
                        4,     // supportheight
                        4,     // 0=none, 1=countersink, 2=recessed hole, 3=nut holder, 4=blind hole
                        0,     // standoff style 0=hex, 1=cylinder
                        1,     // enable reverse standoff
                        0,     // enable insert at top of standoff
                      4.5,     // insert hole dia. mm
                      5.1],    // insert depth mm
    bottom_standoff[ 6.75,     // diameter
                        5,     // height (bottom_height-pcb_z)
                      3.6,     // holesize
                       10,     // supportsize
                        4,     // supportheight
                        1,     // 0=none, 1=countersink, 2=recessed hole, 3=nut holder, 4=blind hole
                        0,     // standoff style 0=hex, 1=cylinder
                        0,     // enable reverse standoff
                        0,     // enable insert at top of standoff
                      4.5,     // insert hole dia. mm
                      5.1],    // insert depth mm
    top_ext_standoff[    6.75, // diameter
                       18,     // height (top_height)
                      2.5,     // holesize
                       10,     // supportsize
                        4,     // supportheight
                        4,     // 0=none, 1=countersink, 2=recessed hole, 3=nut holder, 4=blind hole
                        0,     // standoff style 0=hex, 1=cylinder
                        1,     // enable reverse standoff
                        0,     // enable insert at top of standoff
                      4.5,     // insert hole dia. mm
                      5.1],    // insert depth mm
    bottom_ext_standoff[ 6.75, // diameter
                        5,     // height (bottom_height-pcb_z)
                      3.6,     // holesize
                       10,     // supportsize
                        4,     // supportheight
                        1,     // 0=none, 1=countersink, 2=recessed hole, 3=nut holder, 4=blind hole
                        0,     // standoff style 0=hex, 1=cylinder
                        0,     // enable reverse standoff
                        0,     // enable insert at top of standoff
                      4.5,     // insert hole dia. mm
                      5.1],    // insert depth mm

"class","type",loc_x,loc_y,loc_z,face,rotation[x,y,z],parametrics[association,x,y,z],size_x,size_y,size_z,data_1,data_2,"data_3",data_4[]

Fixed Schema Entries
The 30 fixed schema entries are self-evident based on their name.

    case_name = “case_name”
    sbc_model = any sbc from sbc model framework: "c1+","c2","c4"...
    case_design = "shell", "panel", "stacked", "tray"
    case_style = “style” of case_design (tray: none, vu5, vu7)
    pcb_loc_x = sbc location x axis
    pcb_loc_y = sbc location y axis
    pcb_loc_z = sbc location z axis
    case_offset_x = additional case x axis size
    case_offset_y = additional case y axis size
    case_offset_tz = additional case top z axis size
    case_offset_bz = additional case bottom z axis size
    wallthick = case wall thickness
    floorthick = case floor thickness
    sidethick = case side thickness
    gap = distance between pcb and case
    fillet = edge fillets
    indents = enable indentations around io openings (true or false)
    sidewall_support = enable wall support for standoffs (true or false)
    sbc_top_standoffs = enable sbc top standoffs (true or false)
    sbc_bottom_standoffs = enable sbc bottom standoffs (true or false)
    case_ext_standoffs = enable case extended standoffs (true or false)
    sata_punchout = enable sata punchout (true or false)
    gpio_opening = gpio openings "none","vent","open","punchout"
    cooling = "none", "vents", "fan", "custom" using ./dxf/customfan.dxf
    exhaust_vents = exhaust vents "none","vent"
    top_standoff[] = top pcb standoffs
    bottom_standoff[] = bottom pcb standoffs
    top_ext_standoff[] = top extended standoffs
    bottom_ext_standoff[] = bottom extended standoffs
    mode = special mode "net_card"

### Accessories Configuration Entries
The accessories entries need more explanation because of their input variability. For accessories there are 6 classes, “add1”,“sub”,”suball”,”add2”,”model”,”platter” and all use the same command format for various “type”.

  `"class","type",loc_x,loc_y,loc_z,size_x,size_y,size_z,"face",rotation[],parametrics[],data_1,data_2,"data_3",data_4[]`

e.g.

  `"sub","rectangle",3,78,-.1,8,8,5,"bottom",[0,0,0,],["sbc",true,true,true],0,0,"",[1,1,1,1]`

Every type, regardless of it’s class, uses a basic set of variables(loc_x,loc_y,loc_z,”face”,rotation[],parametrics[]) but each type doesn’t necessarily use all available data fields(size_x,size_y,size_z,data_1,data_2,”data_3”,data_4[]). “add1” and “add2” are used to add geometry to the case. The difference is when the addition occurs. “add1” happens at the beginning when the core case geometry is created and add2 happens after all subtractions have occurred. “suball” is used to affect all faces of a case, not just “face”. The “face” is the case piece that will be effected by the addition or subtraction. The "model" type is for placing supporting accessories in the model view. e.g. hard drives, fans. The "platter" type is for adding supporting accessories to the print platter.

The parametric array specifies the axis to enable for associated parametric positoning. An accessory can be associated with the sbc position("sbc"), case offset("case"),multi-associated which use sbc xy postion and case z offset(sbc-case_z) or uses absolute values if all axises are false

#### classes: add1, sub, suball, add2, model, platter

**additive type:**
circle, rectangle, slot, text, art, standoff, batt_holder, uart_holder, hd_holder, hd_holes, hd_vertright_holes, hc4_oled_holder, access_port, button, pcb_holder, boom_grill, boom_speaker_holder

**subtractive type:**
circle, rectangle, slot, text, art, punchout, vent, fan, hd_holes, hd_vertleft_holes, hd_vertright_holes, microusb, sphere

**model type:**
uart_strap, fan_cover, hd25, hd35, hc4_oled, feet, access_cover, net_card, hk35_lcd, hk_boom, boom_speaker, boom_vring, hk_uart

**platter type:**
uart_strap, fan_cover, access_cover, button_top, boom_vring


#### Shared add and sub “type” commands
**circle**
description: circlular geometry.
*uses:* size_x=dia, size_z=height

**rectangle**
*description:* rectangular geometry with individual defined corner fillets. Radius1 is lower left corner then moves clockwise.
*uses:* size_x, size_y, size_z, data_4=[radius1, radius2, radius3, radius4]

**slot**
*description:* slot geometry.
*uses:* size_x=diameter, size_y=length, size_z=height

**text**
*description:* raised or sunk text
*uses:* data_1=size, data_3="text"

**art**
*description:* art work in dxf or svg format
*uses:* data_1=scale, data_2=height, data_3=file


#### Add class only “types”
**uart_holder**
*description:* console uart holder
*uses:* none

**batt_holder**
*description:* rtc battery holder
*uses:* none

**standoff**
*description:* user defined standoff
*uses:* data_4=
    [ 6.75, // radius
    5, // height
    3.6, // holesize
    10, // supportsize
    4, // supportheight
    1, // 0=none, 1=countersink, 2=recessed hole, 3=nut holder, 4=blind hole
    0, // standoff style 0=hex, 1=cylinder
    0, // enable reverse standoff
    0, // enable insert at top of standoff
    4.5, // insert hole dia. mm
    5.1] // insert depth mm


**hd_holder**
*description:* double stacked holder for 2.5 and 3.5 drives
*uses:* data_1=2.5 or 3.5, data_3=”portrait” or “landscape”

**hd_vertleft_holder**
*description:* vertical left side holder for 2.5 and 3.5 drives
*uses:* data_1=2.5 or 3.5, data_3=”portrait” or “landscape”

**hd_vertright_holder**
*description:* vertical right side holder for 2.5 and 3.5 drives
*uses:* data_1=2.5 or 3.5, data_3=”portrait” or “landscape”

**hc4_oled_holder**
*description:* hc4 oled holder
*uses:* size_z=floorthick

**access_port**
*description:* bottom access for sd and emmc
*uses:* size_z=floorthick, data_3=”portrait” or “landscape”

**button**
*description:* button top and plunger
*uses:* size_x=diameter,size_z=height, data_3=”reccess”

**pcb_holder**
*description:* pcb bottom edge holder
*uses:* size_x=pcb_x,size_y=pcb_y,size_z=pcb_z, data_1=wall_thick

**boom_grill**
*description:* hk boom bonnet grill covers
*uses:* data_3="flat", "dome", "frame"

**boom_speaker_holder**
*description:* hk boom bonnet speaker friction holder
*uses:* data_1=tolorence


#### Sub class only “types”
**punchout**
*description:* punchout in rectangle, round or slot shape
*uses:* size_x=width, size_y=depth, data_1=gap, size_z=thick, data_2=fillet, data_3="rectangle","round" or "slot"

**vent**
*description:* horizontal or vertical vent openings
*uses:* size_x=open_width, size_y=open_length, size_z=thick, data_4=gap, data_1=rows, data_3=columns, data_3=orientation("vertical","horizontal")

**fan**
*description:* fan opening
*uses:* size_x=size, size_z=thick, date_1=style(1=open,2=fan)

**hd_holes**
*description:* bottom hole pattern for 2.5 or 3.5 drives
*uses:* data_1=2.5 or 3.5, data_2=thick, data_3=”portrait” or “landscape”

**hd_vertleft_holes**
*description:* bottom hole pattern for 2.5 or 3.5 drives
*uses:* data_1=2.5 or 3.5, data_2=thick, data_3=”portrait” or “landscape”

**hd_vertright_holes**
*description:* bottom hole pattern for 2.5 or 3.5 drives
*uses:* data_1=2.5 or 3.5, data_2=thick, data_3=”portrait” or “landscape”-component mask(incomplete)

**microusb**
*description:* micro usb opening
*uses:* none

**sphere**
*description:* sphere subtraction
*uses:* size_x=diameter

#### Model class “types”
**uart_strap**
*description:* console uart holder strap
*uses:* none

**fan_cover**
*description:* cover for fan hole opening
*uses:* size_x=40 or 80, size_z=thick

**hd25**
*description:* 2.5 hard drive
*uses:* data_1=height

**hd35**
*description:* 3.5 hard drive
*uses:* none

**hc4_oled**
*description:* hc4_oled model
*uses:* none

**feet**
*description:* case feet
*uses:* size_x=diameter, size_z=height

**access_cover**
*description:* bottom access cover for sd and emmc
*uses:* size_z=floorthick, data_3=”portrait” or “landscape”

**button_top**
*description:* button top and plunger
*uses:* size_x=diameter,size_z=height, data_3=”reccess”

**h2_netcard**
*description:* h2 network card model
*uses:* none

**hk_lcd35**
*description:* hk 3.5 inch lcd model
*uses:* none

**hk_boom**
*description:* hk stereo boom bonnet model
*uses:* data_1=speakers(true or false), data_3=”front” or "rear"

**boom_speaker**
*description:* hk stereo boom bonnet speaker
*uses:* data_1=pcb(true or false), data_3=”left” or "right"

**hk_speaker**
*description:* hk speaker model
*uses:* none

**boom_vring**
*description:* hk stereo boom bonnet volume wheel extention
*uses:* data_1=tolerence

**hk_uart**
*description:* hk console uart model
*uses:* none


#### Platter class “types”
**uart_strap**
*description:* console uart holder strap
*uses:* none

**fan_cover**
*description:* cover for fan hole opening
*uses:* size_x=40 or 80, size_z=thick

**access_cover**
*description:*bottom access cover for sd and emmc
*uses:* size_z=floorthick, data_3=”portrait” or “landscape”

**button_top**
*description:* button top and plunger
*uses:* size_x=diameter,size_z=height, data_3=”reccess”

**boom_vring**
*description:* hk stereo boom bonnet volume wheel extention
*uses:* data_1=tolerence 
