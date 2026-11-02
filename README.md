# Rounds

Structure identification drill. One page, one JSON file per set, one or more images per set.

Open a set
- rounds.html?set=larynx-anterior
- rounds.html?set=larynx-posterior
- rounds.html?set=bronchial-tree

Files
- rounds.html: the tool.
- sets/<id>.json: frames (images), structure list, captions, hit zones, marker positions, clue questions.
- images/: model photos.
- audio/<set id>/<structure id>-name.m4a, -caption.m4a, -clue1.m4a ... : optional recorded clips. If a clip is missing the browser reads the text aloud. Both .m4a and .webm work.
- audio/intro.mp3: optional opening music. Starts when the student presses Begin, fades out when the drill appears.

Author mode
- rounds.html?set=<id>&author=1
- Drag points, click to add a point, double-click a point to remove it, drag the pin and the number.
- Edit name, accepted alternates, pronunciation hint, caption.
- Record the name prompt, caption, and clue clips with the red buttons. Download all clips gives you a zip; unzip it into audio/<set id>/.
- Copy JSON, paste over sets/<id>.json.

Rounds
- 0 Tour, 1 Find it, 2 Name it, 3 Recall, 4 Clues, 5 Teach it. A clean pass unlocks the next round. Progress is saved in the browser.

Embedding
- Canvas: iframe to the GitHub Pages URL. The page sends its height to the parent frame.
