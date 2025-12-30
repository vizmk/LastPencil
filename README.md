# LastPencil
# Last Pencil Game – Java

This is a console-based Java implementation of the classic Last Pencil game.

Two players take turns removing 1, 2, or 3 pencils from a pile.
The player who takes the last pencil loses.

One player is human (John), the other (Jack) is a bot that follows a winning strategy based on simple game theory.

---

GAME RULES

- The game starts with a given number of pencils.
- Players alternate turns.
- On each turn, a player removes 1, 2, or 3 pencils.
- Taking the last pencil means losing the game.

---

BOT STRATEGY

The bot always tries to force the opponent into a losing position.

Losing positions:
1, 5, 9, 13, ...

Winning positions:
- 2, 6, 10, 14, ...  -> take 1 pencil
- 3, 7, 11, 15, ...  -> take 2 pencils
- 4, 8, 12, 16, ...  -> take 3 pencils

If the bot starts in a losing position, it makes any valid move.

---

FEATURES

- Full input validation
- Strict output formatting
- Deterministic bot behavior
- Single-file Java solution
- Fully compliant with Hyperskill automated tests

---

HOW TO RUN

Compile:
javac Main.java

Run:
java Main

---

NOTES

All output messages and formatting are intentional and required to pass automated tests.
Changing strings or line order may cause test failures.
