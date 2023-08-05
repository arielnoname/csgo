```
echo "##############################################"
echo "##################NONAMESIYO##################"
echo "##############################################"

unbindall
sensitivity 1.8

bind 1 "slot1"
bind 2 "slot2"
bind 3 "slot3"
bind 4 "slot4"
bind 5 "slot5"

bind e "+forward;r_cleardecals" 
bind d "+back" 
bind s "+moveleft" 
bind f "+moveright" 
bind a "+speed" 
bind w "lastinv" 
bind r "+reload" 
bind g "+use" 
bind t "drop"
bind shift "+duck" 
bind space "+jump" 

bind "z" "+lookatweapon"

bind b "buymenu"
bind MWHEELUP "+jump" 
bind MWHEELDOWN "invnext" 
bind MOUSE1 "+attack" 
bind MOUSE2 "+attack2" 
bind MOUSE3 "+spray_menu"
bind MOUSE4 "+voicerecord" 
bind MOUSE5 "clutch_mode_toggle"
bind MOUSE6 "player_ping" 

bind F1 player_ping
bind F2 negative
bind F4 cheer
bind F12 jpeg

bind "KP_END" ""
bind "KP_PGDN" ""
bind "KP_HOME" ""
bind "KP_PGUP" ""
bind "KP_DEL" "use weapon_knife; use weapon_c4; drop; say_team SUELTO LA BOMBA LOCO RECOGELA RECOGELA BOMBA BOMBA"

bind "q" "buy flashbang; use weapon_flashbang"
bind "x" "buy smokegrenade; use weapon_smokegrenade"
bind "c" "buy hegrenade; use weapon_hegrenade"
bind "v" "buy incgrenade; buy molotov; use weapon_molotov; use weapon_incgrenade"

bind o "messagemode" 
bind p "messagemode2"

alias "+jumpthrow" "+jump;-attack" 
alias "-jumpthrow" "-jump" 
bind alt "+jumpthrow"


// TWINSEN'S DISPLAY DAMAGE INFO SCRIPT
developer 1
con_filter_enable 2
con_filter_text_out "Player:"
con_filter_text "damage Given"

// MISC
fps_max "0"
cl_radar_always_centered "0" // Keeps the radar centered
cl_autowepswitch "0" // no cambia al arma recogida
cl_autohelp "0" // Enable/disable on screen hints (enemy, trade weapon, etc.)
cl_showhelp "0" // Show the hints on screen
cl_righthand "0" // 0 for left hand 1 for right hand or use bindtoggle <key> cl_righthand to 

// INTERNET
rate "128000" // This is your client rate, you may need to lower it if your net speed cannot keep up
cl_cmdrate "128" // 128 tick servers require this rate (64 will default to 64 for you, no need to edit)
cl_updaterate "128" // 128 tick servesr require this rate (64 will default to 64 for you, no need to edit)
cl_interp_ratio 1 // Common interp setting for MM/League
cl_interp 0 // Common interp setting for MM/League
mm_dedicated_search_maxping "50" // no entra a servers con mas de ese ping 

// MOUSE HARDWARE
m_rawinput "1" 
m_mouseaccel1 "0" 
m_mouseaccel2 "0"


// Audio
volume "0.05"
voice_enable "1"
voice_scale "0.2"
snd_mixahead "0.05"
snd_tensecondwarning_volume "0.2"
snd_menumusic_volume "0"
snd_roundend_volume "0"
snd_roundstart_volume "0"
snd_deathcamera_volume "0"
snd_mapobjective_volume "0"
snd_mute_losefocus "0"

snd_front_headphone_position "90.0"
snd_rear_headphone_position "90.0"
snd_headphone_pan_radial_weight "1.0"
snd_headphone_pan_exponent "1.2"
dsp_enhance_stereo "0"

snd_pitchquality "1"

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

cl_crosshairstyle "4" 
cl_crosshairusealpha "1"
cl_crosshairalpha "255" // full opacity
cl_crosshaircolor "0" // Will give you a red crosshair
cl_crosshairdot "1" 
cl_crosshairsize "0.6" // justo antes de ser cruz
cl_crosshairthickness "0.7" // un punto mas
cl_crosshair_drawoutline "0" // no shadow
cl_crosshair_outlinethickness 0 // no se usa
cl_crosshairgap "-3.2" // min pa que quede bien con el punto
// sgte es para que no se mueva
cl_crosshair_dynamic_maxdist_splitratio "0.0" 
cl_crosshair_dynamic_splitalpha_innermod "1" 
cl_crosshair_dynamic_splitalpha_outermod "0.300000" 
cl_crosshair_dynamic_splitdist "5" 
// MISC
cl_crosshair_friendly_warning "0" 
cl_crosshair_sniper_show_normal_inaccuracy "0" 
cl_crosshair_sniper_width "1"
cl_crosshair_t "0" 
cl_crosshairgap_useweaponvalue "0" 


// RADAR 
cl_radar_always_centered "0" 
cl_radar_scale "0.28" 
cl_radar_icon_scale_min "2" // puntitos del radar gigantes
cl_hud_radar_scale "1.15"

// lo que se mueve la mano (cre)oa
cl_bob_lower_amt "5" // cuanto desaparece la mano al correr. 5 min. no desaparece.
cl_bobamt_lat "0.1" // cuanto se mueve la mano horizontalmente
cl_bobamt_vert "0.1" // idem vertical
cl_bobcycle "0.98" // no cache bien

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
alias "+scorenet" "+showscores; net_graphheight 0" 
alias "-scorenet" "-showscores; net_graphheight 9999" 


// OBSCURE SHIt
r_dynamic "0" // Turns off dynamic lighting, which some players find distracting.
r_drawparticles "0" //  Turns off engine particles.
r_drawtracers_firstperson "1"
cl_disablehtmlmotd "1"// (Disables The Servers Message of The Day.)
cl_forcepreload "1" //(Preloads The Whole Map & Sounds.)
mat_queue_mode "2" //(Forcing Your CPU To Use Multi-Threaded Mode.)
r_drawtracers_firstperson "0" //(First-person Tracers OFF.)
r_eyegloss "0"// (No Makeup.)
r_eyemove "0" //(No Eye Movement.)
r_eyeshift_x "0" //(No Eye Movement X-Angel.)
r_eyeshift_y "0"// (No Eye Movement Y-Angel.)
r_eyeshift_z "0"// (No Eye Movement Z-Angel.)
r_eyesize "0" //(Smaller Eyes.)

host_writeconfig 

echo "##############################################"
echo "##################NONAMESIYO##################"
echo "##############################################"

