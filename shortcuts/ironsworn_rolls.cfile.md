__
^actionRoll.*([0-9])$
__
function roll(max) { return Math.trunc(Math.random() * max + 1); }

$1 = Number($1) || 1;
actionRoll = roll(6);
actionScore = actionRoll + $1;
challengeA = roll(10);
challengeB = roll(10);

return "š² " + actionScore + " āµ (" + actionRoll + ") D6 + " + $1 + "\nš² " + challengeA + " āµ (" + challengeA + ") D10\nš² " + challengeB + " āµ (" + challengeB + ") D10";
__
Returns Ironsworn action roll.

__
^challengeRoll$
__
function roll(max) { return Math.trunc(Math.random() * max + 1); }

challengeA = roll(10);
challengeB = roll(10);

return "š² " + challengeA + " āµ (" + challengeA + ") D10\nš² " + challengeA + " āµ (" + challengeA + ") D10";
__
Returns Ironsworn challenge roll.

__
^oracleRoll$
__
function roll(max) { return Math.trunc(Math.random() * max + 1); }

oracle = roll(100);

return "š² " + oracle + " āµ (" + oracle + ") D100";
__
Returns Ironsworn oracle roll.
