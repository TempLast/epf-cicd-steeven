# EPF CI/CD — Steeven Leroyer

**Qu'est-ce qui déclenche la pipeline ? Pouvez-vous la déclencher autrement ?**
- La pipeline est déclenché grâce au push que l'on execute dans notre fichier yml. On peut déclencher la pipeline autrement avec un script ou exécuter le fichier manuellement.

**Où s'exécute-t-elle ? Sur quel système d'exploitation ? Qui fournit cette machine ?**
- La pipeline s'exécute dans la branche du main avec l'utilisation de Ubuntu (WSL).

**Que se passe-t-il si une commande échoue ? Le step suivant s'exécute-t-il ? Comment l'avez-vous vérifié ?**
- Si une commande échoue elle ne s'exécute pas et bloque l'exécution complète de la pipeline (exemple erreur de synthaxe). Pour vérifier on va modifier un run pour que la commande échoue en faisant une erreur de synthaxe, avec l'aide des logs on peut apercevoir quelle va être l'erreur avec l'endroit ou elle ce situe.

**À quoi cela pourrait-il servir sur un vrai projet ? Donnez trois exemples de commandes utiles.**
- Cela permettrait d'exécuter automatiquement certaine "tâches".

**Qu'est-ce qui vous semble compliqué ? Qu'est-ce qui vous semble « magique » ?**
-
