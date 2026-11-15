# Banana NPC Mod by theacefes for oBG2, BG2EE, and EET

Thankee, Claude, for handling this!

- Installs on Baldur's Gate II (SoA/ToB), BGT, BG2:EE and EET. The installer refuses other games.

- All text moved to tra files (tra/english). EE games load a UTF-8 copy (tra/english_ee), so the ellipses and dashes in Banana!'s lines show correctly on EE.

- EE portraits: larger copies (54x84 and 169x266) are installed on BG2:EE and EET.

- Sound: the Ogg files are installed with WeiDU's HANDLE_AUDIO, which works on Windows, macOS and Linux. The old batch files only worked on Windows, and the macOS/Linux branch called scripts that were never included, so the install failed there.

- Bug fix: in Throne of Bhaal the party tables pointed at files the mod never had (K#Ban25P, K#Ban25B, K#Bana25), so kicking Banana! out gave no dialogue, she had no banters and her script (the one that makes her leave) was replaced by nothing. They now use her real files.

- Bug fix: when she "flees into the backlit horizon" after being kicked out, she now really leaves and goes back to the Copper Coronet, where she can be asked to rejoin. Before, she stood still and repeated the kick-out conversation every time you talked to her.

- Bug fix: the original overwrote the first entry of SONGLIST.2DA with its own blank song. This is now only done when that entry is not already a blank song (EE games and BG2 Fixpack have one).

- Installer updated to WeiDU 251.

- New: in Throne of Bhaal, the Fate Spirit in the Pocket Plane can summon Banana! ("Bring me Banana!..."). If she travelled with you in Shadows of Amn, she is brought over; if you never met her, or she "browned" and left, a new Banana! appears. If you met her but never let her join, the Fate Spirit cannot reach her. On EET this uses EET's own NPC transition function, so it also works in games started in ToB.
