```
sensivity 3

bind e "+forward" 
bind d "+back" 
bind s "+moveleft" 
bind f "+moveright" 
bind a "+speed" 
bind w "lastinv" 
bind r "+reload;r_cleardecals" 
bind g "+use" 
bind t "drop"
bind shift "+duck" 
bind space "+jump" 

bind MWHEELUP "+jump" 
bind MWHEELDOWN "invnext" 
bind MOUSE1 "+attack" 
bind MOUSE2 "+attack2" 
bind MOUSE4 "+voicerecord" 
bind MOUSE5 "clutch_mode_toggle"

bind z "use weapon_flashbang" 
bind x "use weapon_smokegrenade" 
bind c "use weapon_hegrenade" 
bind v "use weapon_molotov;use weapon_incgrenade"

bind o "messagemode" 
bind p "messagemode2"

alias "+jumpthrow" "+jump;-attack" 
alias "-jumpthrow" "-jump" 
bind alt "+jumpthrow"

// PRACTICE BINDS
bind "h" "give weapon_hegrenade;give weapon_flashbang;give weapon_smokegrenade;give weapon_incgrenade;give weapon_molotov;give weapon_decoy" 
bind "j" "cast_ray"
bind ctrl "noclip"

cl_autowepswitch "0" // no cambia al arma recogida

// MOUSE HARDWARE
m_rawinput "1" 
m_mouseaccel1 "0" 
m_mouseaccel2 "0"

// HUD
cl_hud_healthammo_style "0" // 3 balitas marcadas pa la glock
hud_showtargetid "1" // nombres de enemigos
cl_hud_playercount_pos "0" // score arriba
cl_hud_radar_scale "1.15" // radar mas grande
cl_hud_playercount_showcount "1" // cuenta de players vivos
cl_hud_color "9" // teal 
cl_hud_background_alpha "0" // sin fondo pa los numeritos etc
cl_hud_bomb_under_radar "1" // c4 debajo del radar

// CROSSHAIR. Este es un punto rojo y no se mueve. // Para setear con un mapa, ir a: // 1. https://steamcommunity.com/sharedfiles/filedetails/?id=308490450 
cl_crosshair_drawoutline "0" 
cl_crosshair_dynamic_maxdist_splitratio "0.0" 
cl_crosshair_dynamic_splitalpha_innermod "1" 
cl_crosshair_dynamic_splitalpha_outermod "0.300000" 
cl_crosshair_dynamic_splitdist "5" 
cl_crosshair_friendly_warning "1" 
cl_crosshair_outlinethickness "0.5" 
cl_crosshair_sniper_show_normal_inaccuracy "0" 
cl_crosshair_sniper_width "1" cl_crosshair_t "0" 
cl_crosshairalpha "255" cl_crosshaircolor "5" 
cl_crosshaircolor_b "0" cl_crosshaircolor_g "0" 
cl_crosshaircolor_r "255" cl_crosshairdot "1" 
cl_crosshairgap "-4.000000" 
cl_crosshairgap_useweaponvalue "0" 
cl_crosshairsize "0.500000" 
cl_crosshairstyle "4"
cl_crosshairthickness "0"
cl_crosshairusealpha "1"

// RADAR 
cl_radar_always_centered "0" 
cl_radar_scale "0.28" 
cl_radar_icon_scale_min "2" // puntitos del radar gigantes
cl_hud_radar_scale "1.15"

// lo que se mueve la mano (cre)oa
cl_bob_lower_amt "5" 
cl_bobamt_lat "0.1" 
cl_bobamt_vert "0.1" 
cl_bobcycle "0.98"

// Como se ven las manos
viewmodel_fov "0" // 0 se ve menos arma, 68 se ve mas. en realidad creo que 54 es el minimo 
viewmodel_offset_x "2.5" maximo, -2 minimo. menos es mas al centro 
viewmodel_offset_y "2" // 2 maximo, -2 minimo. 
viewmodel_offset_z "-2" // -2 minimo. 2 maximo. mas es mas arriba.
cl_viewmodel_shift_left_amt "0" // este par de hueas no hacen nada pero estaban en el tut 
cl_viewmodel_shift_right_amt "0"
viewmodel_recoil "0" // idem

net_graph "1" net_graphheight "9999" 
bind "TAB" "+scorenet" 
alias "+scorenet" "+showscores; 
net_graphheight 0" 
alias "-scorenet" "-showscores;
net_graphheight 9999" 
host_writeconfig 
echo "nonamesitos cfg"
```
