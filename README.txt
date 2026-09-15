PUT YOUR THREE SONGS IN THIS FOLDER
===================================

Rename your files to exactly these three names:

  music1-opening.mp3        -> plays from the moment the card opens (opening pages)
  music2-celebration.mp3    -> plays on the celebration / sky-lantern screen
  music3-cake.mp3           -> plays from the cake-cutting screen to the final page

That is all. Keep this "music" folder next to happy-birthday-card.html and
nothing inside the HTML needs to be edited.

Using a different format (m4a / ogg / wav) or different names?
Open happy-birthday-card.html, find these three lines near the top of <body>
and change only the src="..." values:

  <audio id="music1" src="music/music1-opening.mp3" preload="auto" loop></audio>
  <audio id="music2" src="music/music2-celebration.mp3" preload="auto" loop></audio>
  <audio id="music3" src="music/music3-cake.mp3" preload="auto" loop></audio>

Notes
-----
* Each song loops until its section ends, so short tracks are fine.
* If a file is missing, the card quietly falls back to its built-in score
  instead of breaking.
* Phones block audio until the first tap, so the music starts on the
  "tap to begin" screen. That is a browser rule, not a bug.
