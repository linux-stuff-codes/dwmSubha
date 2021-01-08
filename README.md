# My DWM config

## Patches applied : 

- 5.8.2-swap
- anybar-polybar-tray-fix-20200810-bb2e722
- centeredmaster-6.1
- centeredwindowname-20180909-6.2
- cool-autostart-6.2
- cyclelayouts-20180524-6.2
- fixborders-6.2
- focusmaster-20200717-bb2e722
- fullgaps-6.2
- gaps-6.0
- gridmode-20170909-ceac8c9
- gridmode-5.8.2
- hide_vacant_tags-6.2
- inplacerotate-6.2
- restartsig-20180523-6.2

## Key Bindings

/* modifier                     key        function        argument */
{ MODKEY,                       XK_p,      spawn,          {.v = dmenucmd }},
{ MODKEY|ShiftMask,	            XK_f,      spawn,        SHCMD(TERMINAL " -e vifm") },
{ MODKEY|ShiftMask,	            XK_v,      spawn,        SHCMD(TERMINAL "-e bitwarden-dmenu") },
{ MODKEY,	                    XK_Return, spawn,          {.v = termcmd } }, //st
{ MODKEY,	                    XK_x,      spawn,          {.v = flamecmd } }, //flameshot
{ MODKEY,	                    XK_w,      spawn,          {.v = qucmd } }, //qutebrowser
{ MODKEY,	                    XK_F6, 	   spawn,          {.v = thunarcmd } }, //thunar
{ MODKEY,                       XK_b,      togglebar,      {0} },
{ MODKEY,                       XK_j,      focusstack,     {.i = +1 } },
{ MODKEY,                       XK_k,      focusstack,     {.i = -1 } },
{ MODKEY|ShiftMask,             XK_j,      inplacerotate,  {.i = +1} },
{ MODKEY|ShiftMask,             XK_k,      inplacerotate,  {.i = -1} },
{ MODKEY|ShiftMask,             XK_h,      inplacerotate,  {.i = +2} },
{ MODKEY|ShiftMask,             XK_l,      inplacerotate,  {.i = -2} },
{ MODKEY,                       XK_i,      incnmaster,     {.i = +1 } },
{ MODKEY,                       XK_d,      incnmaster,     {.i = -1 } },
{ MODKEY,                       XK_h,      setmfact,       {.f = -0.05} },
{ MODKEY,                       XK_l,      setmfact,       {.f = +0.05} },
{ MODKEY|ShiftMask,                        XK_Return, zoom,           {0} },
{ MODKEY,                       XK_Tab,    view,           {0} },
{ MODKEY,                       XK_q,      killclient,     {0} },
{ MODKEY,                       XK_t,      setlayout,      {.v = &layouts[0]} },
{ MODKEY,                       XK_f,      setlayout,      {.v = &layouts[1]} },
{ MODKEY,                       XK_m,      setlayout,      {.v = &layouts[2]} },
{ MODKEY,                       XK_u,      setlayout,      {.v = &layouts[3]} },
{ MODKEY,                       XK_o,      setlayout,      {.v = &layouts[4]} },
{ MODKEY,                       XK_g,      setlayout,      {.v = &layouts[5]} },
{ MODKEY,                       XK_space,  setlayout,      {0} },
{ MODKEY,                       XK_space,  setlayout,      {0} },
{ MODKEY|ShiftMask,             XK_space,  togglefloating, {0} },
{ MODKEY,                       XK_0,      view,           {.ui = ~0 } },
{ MODKEY|ShiftMask,             XK_0,      tag,            {.ui = ~0 } },
{ MODKEY|ShiftMask,             XK_comma,  tagmon,         {.i = -1 } },
{ MODKEY|ShiftMask,             XK_period, tagmon,         {.i = +1 } },
{ MODKEY,                       XK_minus,  setgaps,        {.i = -1 } },
{ MODKEY,                       XK_equal,  setgaps,        {.i = +1 } },
{ MODKEY|ShiftMask,             XK_equal,  setgaps,        {.i = 0  } },
 MODKEY|ShiftMask|ControlMask,             XK_c,      quit,           {0} },
{ MODKEY|ShiftMask|ControlMask,             XK_q,      quit,           {1} },
TAGKEYS(                        XK_1,                      0)
TAGKEYS(                        XK_2,                      1)
TAGKEYS(                        XK_3,                      2)
TAGKEYS(                        XK_4,                      3)
TAGKEYS(                        XK_5,                      4)
TAGKEYS(                        XK_6,                      5)
TAGKEYS(                        XK_7,                      6)
TAGKEYS(                        XK_8,                      7)
TAGKEYS(                        XK_9,                      8)
{
