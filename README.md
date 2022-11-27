# Paper IO

Un jeu.

## Protocole

Structure packet:
{
  "d": object,
  "t": u64,
}

### C -> S

- 0 -> requête de connection
- 1 -> changement de direction

### S -> C

- 0 -> connection acceptée
- 1 -> joueur rejoint
- 2 -> joueur quitte
- 3 -> démarrage de la partie
- 4 -> spawn joueur
- 5 -> changement de direction
- 6 -> mort
- 7 -> fin de partie
