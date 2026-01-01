# Le Langage de Programmation

## Un langage de programmation simple de type C. La principale différence est son typage dynamique similaire à JavaScript pour les valeurs (une chaîne peut être implicitement convertie en nombre, mais des types plus complexes ne peuvent **pas** être convertis implicitement).

### Expressions:
- Les expressions arithmétiques et logiques: `1+1`, `a && b`, `x || y`
- Opérateurs de comparaison: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Opérateurs arithmétiques: `+`, `-`, `*`, `/`, `%`, `**` (puissance)
- Opérateurs de décalage: `<<`, `>>`
- Opérateur logique NOT: `!`
- `{item0, item1, ...}` pour déclarer un tableau (array)
- `(item0, item1, ...)` pour déclarer un tuple
- Les chaînes de caractères: `"texte"` ou `'texte'`
- Accès aux éléments: `identifiant[index]` ou `identifiant[index0][index1]...`
- Accès aux membres: `objet.membre` ou `objet.membre.sous_membre`
- Appels de fonction: `fonction(arg1, arg2, ...)`

### Déclaration d'objet:
- `{type} {nom};`
- `{type} {nom} = {expr};`
- `{nom} = {expr};` (assignation à un objet existant)
- `{nom} {opérateur_assignation} {expr};` où opérateur_assignation peut être `=`, `+=`, `-=`, etc.

### Structures de contrôle:
#### If:
```
if (expr) {
    // liste d'instructions
}
```
```
if (expr) {
    // liste d'instructions
} else {
    // liste d'instructions
}
```

#### While:
```
while (expr) {
    // liste d'instructions
}
```

### Déclaration de fonction:
```
fun {type_retour} {nom}({type} {param1}, {type} {param2}, ...) {
    // liste d'instructions
}
```

### Blocs:
- Les blocs peuvent être créés avec `{ }` pour organiser le code

### Types de tokens:
- **Keyword** (mots-clés): `if`, `else`, `while`, `fun`
- **Identifier** (identifiants): noms de variables, fonctions, types
- **Operator** (opérateurs): `+`, `-`, `*`, `/`, `%`, `**`, `==`, `!=`, `<`, `>`, `<=`, `>=`, `&&`, `||`, `!`, `<<`, `>>`, `=`, etc.
- **Separator** (séparateurs): `(`, `)`, `[`, `]`, `{`, `}`, `,`, `;`
- **Number** (nombres): littéraux numériques incluant les décimaux
- **String** (chaînes): littéraux de texte entre `"` ou `'`

### Priorité des opérateurs (du plus faible au plus fort):
1. `||` (OR logique)
2. `&&` (AND logique)
3. `==`, `!=`, `<`, `>`, `<=`, `>=` (comparaisons)
4. `+`, `-` (addition, soustraction)
5. `<<`, `>>` (décalages)
6. `*`, `/`, `%` (multiplication, division, modulo)
7. `**` (puissance)
8. `!` (NOT logique)
