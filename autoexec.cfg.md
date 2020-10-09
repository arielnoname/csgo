```
echo "##############################################"
echo "##################NONAMESIYO##################"
echo "##############################################"

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

//bind "f" "buy flashbang; use weapon_knife; use weapon_flashbang"
//bind "t" "buy smokegrenade; use weapon_knife; use weapon_smokegrenade"
//bind "q" "buy hegrenade; use weapon_knife; use weapon_hegrenade"
//bind "r" "buy incgrenade; buy molotov; use weapon_knife; use weapon_molotov; use weapon_incgrenade"
//bind "c" "buy decoy; use weapon_knife; use weapon_decoy"

bind o "messagemode" 
bind p "messagemode2"

alias "+jumpthrow" "+jump;-attack" 
alias "-jumpthrow" "-jump" 
bind alt "+jumpthrow"

// PRACTICE BINDS
bind "h" "give weapon_hegrenade;give weapon_flashbang;give weapon_smokegrenade;give weapon_incgrenade;give weapon_molotov;give weapon_decoy" 
bind "j" "cast_ray"
bind ctrl "noclip"

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
tickrate 128 // If you launch a local server it will run at 128 tick (can also be done with -tickrate 128 put as launch option)
mm_dedicated_search_maxping "50" // no entra a servers con mas de ese ping 

// MOUSE HARDWARE
m_rawinput "1" 
m_mouseaccel1 "0" 
m_mouseaccel2 "0"

// Audio

volume "1"
voice_enable "1"
voice_scale "1"
windows_speaker_config "1"
snd_musicvolume "0.04"
snd_mixahead "0.05"
snd_tensecondwarning_volume "1"
snd_menumusic_volume "0"
snd_roundend_volume "0"
snd_roundstart_volume "0"
snd_deathcamera_volume "0"
snd_mapobjective_volume "0"
snd_headphone_pan_exponent "2"

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


// CROSSHAIR ALTERNO
//cl_crosshairalpha "150" // Changes opacity/alpha of the crosshair color
//cl_crosshaircolor "5" // Will give you a pink crosshair
//cl_crosshaircolor_b "255" // Edits crosshair color manually
//cl_crosshaircolor_g "0" // Edits crosshair color manually
//cl_crosshaircolor_r "255" // Edits crosshair color manually
//cl_crosshairdot "0" // Dot in the center of the crosshair
//cl_crosshairscale "0" // Edits scale/size of crosshair
//cl_crosshairsize "3" // Edits the size of the crosshair
//cl_crosshairthickness ".75" // Changes thickness of the crosshair itself
//cl_crosshairusealpha "0" // Forces use of alpha changes made here
//cl_crosshairstyle "4" // 0 for new CSGO, 1 for static, 2 for old CS:S style (static), and 3 for old CS:S (dynamic)
//cl_crosshair_drawoutline "1" // outlines the crosshair
//cl_crosshair_outlinethickness ".5" // thickness of the outline



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
alias "+scorenet" "+showscores; net_graphheight 0" 
alias "-scorenet" "-showscores; net_graphheight 9999" 


// OBSCURE SHIt
r_dynamic “0” // Turns off dynamic lighting, which some players find distracting.
r_drawparticles "0" //  Turns off engine particles.
r_drawtracers_firstperson “1”
cl_disablehtmlmotd “1” (Disables The Servers Message of The Day.)
cl_forcepreload “1” (Preloads The Whole Map & Sounds.)
mat_queue_mode “2” (Forcing Your CPU To Use Multi-Threaded Mode.)
r_drawtracers_firstperson “0” (First-person Tracers OFF.)
r_eyegloss “0” (No Makeup.)
r_eyemove “0” (No Eye Movement.)
r_eyeshift_x “0” (No Eye Movement X-Angel.)
r_eyeshift_y “0” (No Eye Movement Y-Angel.)
r_eyeshift_z “0” (No Eye Movement Z-Angel.)
r_eyesize “0” (Smaller Eyes.)

host_writeconfig 
echo "##############################################"
echo "##################NONAMESIYO##################"
echo "##############################################"
```
