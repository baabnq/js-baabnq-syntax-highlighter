# js-baabnq-syntax-highlighter

This is a baabnq syntax highlighter and lexer written in pure javascript.
It's not as impressive as it sounds, trust me, lol. 
It just goes through the letters one-by-one and assembles them into tokens, 
which it then classifies and assigns a color to. 
It then inserts colored spans into the source container according to the tokens, which the lexer isolated.
The only technical limitation to this is that the cursor position gets messed up in
an editable element through the highlighting process.
That is annoying but really hard to counteract, as saving and restoring
the cursor position in a contenteditable element is really inconsistent and unnecessarily difficult.

