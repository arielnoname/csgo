Varias cosas robadas de: https://steamcommunity.com/sharedfiles/filedetails/?l=norwegian&id=257041519

1. Es recomendable poner opciones de lanzamiento para el counter. Eso se hace de la siguiente manera:
    
    Browse to your Steam Library
    Right click on Counter Strike: Global Offensive
    Click: Properties
    Click: Set Launch Options
    Paste the following: +exec autoexec.cfg
    For the common CS:GO launch options (disable video, open console, 128tick local server, force monitor refresh rate etc.) use:
    
    -console -novid -high -threads 4 +exec autoexec.cfg -tickrate 128 -refresh 144
    
    Imagen: https://steamuserimages-a.akamaihd.net/ugc/598161395753900450/A7C5AB002CA002B767E9DFB6690CEC8DAD69901C/

# csgo
// autoexec.cgf 



sensitivity 2.6

// OJO ACA
bind e "+forward"
bind d "+back"
bind s "+moveleft"
bind f "+moveright"
bind a "+speed"
bind shift "+duck"
bind space "+jump"
bind MWHEELUP "+jump"
bind MWHEELDOWN "invnext"
bind MOUSE1 "+attack"
bind MOUSE2 "+attack2"
bind MOUSE4 "+voicerecord"
bind MOUSE5 "clutch_mode_toggle"


m_rawinput "1" 
m_mouseaccel1 "0"
m_mouseaccel2 "0"

    cl_hud_healthammo_style "0" // show HP and ammo without bars and bullet icons
    hud_showtargetid "0" // Shows enemy name on screen
    cl_hud_playercount_pos "0" // Position for the playercount on screen
    cl_hud_radar_scale "1" // Changes the size/scale of the radar
    cl_hud_playercount_showcount "1" // forces show all players in the player count
    cl_hud_color "8" // Changes UI Color for HUD HP, Ammo, Money etc
    cl_hud_background_alpha "0.5" // Adjust HUD background alpha for colored elements
    cl_hud_bomb_under_radar "1" // shows bomb icon under radar instead of inventory 

bind w "lastinv"
bind r "+reload;r_cleardecals"
bind g "+use"
bind t "drop"

bind z "use weapon_flashbang"
bind x "use weapon_smokegrenade"
bind c "use weapon_hegrenade"
bind v "use weapon_molotov;use weapon_incgrenade"

bind o "messagemode"
bind p "messagemode2"

// MOUSE
alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
bind ctrl "noclip"
bind alt "+jumpthrow"

bind "h" "give weapon_hegrenade;give weapon_flashbang;give weapon_smokegrenade;give weapon_incgrenade;give weapon_molotov;give weapon_decoy"
bind "j" "cast_ray"


// CROSSHAIR. Este es un punto rojo y no se mueve.
// Para setear con un mapa, ir a: 
// 1. https://steamcommunity.com/sharedfiles/filedetails/?id=308490450
// 
cl_crosshair_drawoutline "0"
cl_crosshair_dynamic_maxdist_splitratio "0.0"
cl_crosshair_dynamic_splitalpha_innermod "1"
cl_crosshair_dynamic_splitalpha_outermod "0.300000"
cl_crosshair_dynamic_splitdist "5"
cl_crosshair_friendly_warning "1"
cl_crosshair_outlinethickness "0.5"
cl_crosshair_sniper_show_normal_inaccuracy "0"
cl_crosshair_sniper_width "1"
cl_crosshair_t "0"
cl_crosshairalpha "255"
cl_crosshaircolor "5"
cl_crosshaircolor_b "0"
cl_crosshaircolor_g "0"
cl_crosshaircolor_r "255"
cl_crosshairdot "1"
cl_crosshairgap "-4.000000"
cl_crosshairgap_useweaponvalue "0"
cl_crosshairsize "0.500000"
cl_crosshairstyle "4";
cl_crosshairthickness "0"
cl_crosshairusealpha "1"

// RADAR
cl_radar_always_centered "0"
cl_radar_scale "0.3"
cl_radar_icon_scale_min "1"
cl_hud_radar_scale "1.15"


cl_bob_lower_amt "5"
cl_bobamt_lat "0.1"
cl_bobamt_vert "0.1"
cl_bobcycle "0.98"

viewmodel_fov "0" // 0 se ve menos arma, 68 se ve mas. en realidad creo que 54 es el minimo
viewmodel_offset_x "2.5" maximo, -2 minimo. menos es mas al centro
viewmodel_offset_y "2" // 2 maximo, -2 minimo. 
viewmodel_offset_z "-2" // -2 minimo. 2 maximo. mas es mas arriba.

cl_viewmodel_shift_left_amt "0"  // este par de hueas no hacen nada pero estaban en el tut
cl_viewmodel_shift_right_amt "0"
    
cl_bob_lower_amt "0"
cl_bobamt_lat "0"
cl_bobamt_vert "0"
cl_bobcycle "2"
    
    
    

viewmodel_recoil "0"

net_graph "1"
net_graphheight "9999"
bind "TAB" "+scorenet"
alias "+scorenet" "+showscores; net_graphheight 0"
alias "-scorenet" "-showscores; net_graphheight 9999"
cl_autowepswitch 0
host_writeconfig
echo "nonamesitos cfg"
