# Steam Summer Minigame 2015 Auto-play Optimizer #

### Purpose ###

This javascript automatically plays the 2015 Steam Summer minigame for you in a semi-optimal way.

It goes beyond the autoclicker scripts already out there. It will keep you in the lane where you'll make the
most money, activate abilities as they are available and best apply, and possibly purchase upgrades and
powerups for you.

### How to use ###

1. Open `autoPlay.js` in a text editor.
2. Select All, Copy
3. In a browser (Chrome, Firefox, IE), log in to Steam, navigate to the minigame page, and start playing the game.
4. For your sanity, turn off sound and music.
5. Hit F12 to bring up the developer console.
6. Navigate to the Console or Script section, where you can enter javascript and see javascript output.
7. Paste into the javascript input, and hit Enter.
8. The game should now play itself, you should leave it running in the background. If you're not sure if it
is auto-playing, try changing lanes. If it jumps back almost immediately, it's working.

To stop the script, type `window.clearTimeout(thingTimer);` into the console and hit Enter.

### TODO ###

- use abilities if available and a suitable target exists:
	 - Tactical Nuke on a Spawner if below 60% and above 30% of its health
	 - Cluster Bomb and Napalm if the current lane has a spawner and 2+ creeps
	 - Good Luck if available
	 - Metal Detector if a spawner death is imminent (predicted in > 2 and < 7 seconds)
	 - Morale Booster if available and lane has > 2 live enemies
	 - Decrease Cooldowns if another player used a long-cooldown ability < 10 seconds ago
	
- purchase abilities and upgrades intelligently

- check if it's a boss level, handle boss levels appropriately

- prefer lane with a dying creep as long as all living Spawners have >40% health