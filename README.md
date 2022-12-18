# FightWebSVR
a long shot at making a working angry birds fight server that can be used with Apache

WARNING: THIS IS WHERE MY NOTES COME IN. AKA THE SHIT YOU PROBS WONT UNDERSTAND LMAO

/login, /account, /raid are all /POST
/newstage does not exist, instead /newstage/ is used, meaning an index.html file is used since blank file names aren't possible in Windows or any other OS
fill most responses with {"status:2000"}
slots (aka /slot) currently  unused, needs something other than {"status:2000"}
/login is a basic login for the game, goes unused in the iOS port (fixes KPL)
/account is sort of unused?? as in the game loads this bullshit but i don't know it's function yet.
upgrade gives a KMG error. //TODO: Fix this shit lmaooooooooo
update on upgrade (01:09am GMT): it now works!
