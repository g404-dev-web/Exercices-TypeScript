# TypeScript - Exercices pratiques - Partie 1

Ce README contient des exercices pratiques pour la partie 1, qui couvre l'introduction à TypeScript, la syntaxe de base, les types de données et les variables.
Pensez à lire la documentation pour comprendre les types que vous allez utiliser lors de ces exercices.

## Exercice 1 : Installation et configuration

1. Installe Node.js et npm (si ce n'est pas déjà fait).
2. Installe TypeScript globalement en utilisant la commande `npm install -g typescript`.
3. Crée un nouveau dossier pour ton projet et initialise un fichier `package.json` en utilisant la commande `npm init -y`.
4. Crée un fichier `tsconfig.json` avec la commande `tsc --init`.

## Exercice 2 : Syntaxe de base et types de données

1. Crée un fichier `basic-types.ts` dans ton projet.
2. Déclare des variables avec les types suivants : `string`, `number`, `boolean`, `any`, `unknown`, `null`, `undefined`, `void`, `never`, `Array`, et `Tuple`.
3. Initialise les variables avec des valeurs appropriées et ajoute les dans des `console.log()`.
4. Compile le fichier TypeScript en JavaScript en utilisant la commande `tsc basic-types.ts`.
5. Exécute le fichier JavaScript généré avec Node.js en utilisant la commande `node basic-types.js`.

## Exercice 3 : Enumérations et objets

1. Crée un fichier `enums-objects.ts` dans ton projet.
2. Déclare une énumération `DaysOfWeek` avec les jours de la semaine.
3. Crée un objet `person` avec les propriétés `firstName`, `lastName`, `age`, et `dayOfBirth` (utilise l'énumération `DaysOfWeek` pour cette dernière propriété).
4. Compile et exécute le fichier comme dans l'exercice 2.

## Exercice 4 : Fonctions et assertions de type

1. Crée un fichier `functions-type-assertions.ts` dans ton projet.
2. Écris une fonction `add` qui prend deux paramètres de type `number` et retourne leur somme.
3. Écris une fonction `greet` qui prend un paramètre de type `string` et retourne une chaîne de caractères de salutation.
4. Utilise des assertions de type pour convertir une variable de type `unknown` en un type spécifique (par exemple, `string` ou `number`).
5. Compile et exécute le fichier comme dans l'exercice 2.


## Exercices pratiques - Partie 2 : Classes, interfaces, décorateurs et génériques

### Exercice 1 : Classes et héritage

1. Crée un fichier `classes.ts` dans ton projet.
2. Déclare une classe `Animal` avec les propriétés `name` et `age`, ainsi qu'une méthode `speak()` qui affiche un message dans la console.
3. Crée une classe `Dog` qui hérite de la classe `Animal` et redéfinit la méthode `speak()` pour afficher un message spécifique aux chiens.
4. Crée une classe `Cat` qui hérite de la classe `Animal` et redéfinit la méthode `speak()` pour afficher un message spécifique aux chats.
5. Instancie les classes `Dog` et `Cat` et appelle leur méthode `speak()`.
6. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 2 : Interfaces

1. Crée un fichier `interfaces.ts` dans ton projet.
2. Déclare une interface `Person` avec les propriétés `firstName`, `lastName` et `age`, ainsi qu'une méthode `introduce()` qui retourne une chaîne de caractères.
3. Crée une classe `Student` qui implémente l'interface `Person` et définit la méthode `introduce()`.
4. Instancie la classe `Student` et appelle sa méthode `introduce()`.
5. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 3 : Décorateurs

1. Crée un fichier `decorators.ts` dans ton projet.
2. Déclare un décorateur de classe `logClass` qui affiche le nom de la classe décorée dans la console.
3. Déclare un décorateur de méthode `logMethod` qui affiche le nom de la méthode décorée et ses arguments dans la console.
4. Applique les décorateurs `logClass` et `logMethod` à une classe et à l'une de ses méthodes.
5. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 4 : Génériques

1. Crée un fichier `generics.ts` dans ton projet.
2. Déclare une fonction générique `identity` qui prend un argument de type générique `T` et retourne cet argument.
3. Utilise la fonction `identity` avec différents types de données (par exemple, `string`, `number`, `boolean`).
4. Déclare une interface générique `KeyValuePair` avec deux types génériques `K` et `V`, représentant une paire clé-valeur.
5. Crée une classe `Dictionary` qui implémente l'interface `KeyValuePair` et permet de stocker des paires clé-valeur.
6. Instancie la classe `Dictionary` et ajoute quelques paires clé-valeur.
7. Compile et exécute le fichier comme dans les exercices précédents.



## Exercices pratiques - Partie 3 : Modules, espaces de noms, gestion des erreurs et outils de développement

### Exercice 1 : Modules

1. Crée un fichier `math.ts` dans ton projet.
2. Exporte une fonction `add` qui prend deux paramètres de type `number` et retourne leur somme.
3. Exporte une fonction `subtract` qui prend deux paramètres de type `number` et retourne leur différence.
4. Crée un fichier `main.ts` dans ton projet.
5. Importe les fonctions `add` et `subtract` depuis le module `math.ts` et utilise-les pour effectuer quelques opérations.
6. Compile et exécute le fichier `main.ts` comme dans les exercices précédents.

### Exercice 2 : Espaces de noms

1. Crée un fichier `shapes.ts` dans ton projet.
2. Déclare un espace de noms `Shapes` avec des classes `Circle` et `Rectangle`.
3. Exporte les classes `Circle` et `Rectangle` depuis l'espace de noms `Shapes`.
4. Crée un fichier `main-ns.ts` dans ton projet.
5. Importe les classes `Circle` et `Rectangle` depuis l'espace de noms `Shapes` et instancie-les.
6. Compile et exécute le fichier `main-ns.ts` comme dans les exercices précédents.

### Exercice 3 : Gestion des erreurs

1. Crée un fichier `error-handling.ts` dans ton projet.
2. Écris une fonction `divide` qui prend deux paramètres de type `number` et retourne leur quotient.
3. Ajoute une gestion des erreurs à la fonction `divide` pour vérifier si le diviseur est égal à zéro et, dans ce cas, lance une exception.
4. Utilise la fonction `divide` dans un bloc `try-catch` pour gérer l'exception et afficher un message d'erreur approprié.
5. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 4 : Outils de développement

1. Installe l'extension TypeScript pour ton éditeur de code préféré (par exemple, Visual Studio Code).
2. Configure l'extension pour utiliser la version de TypeScript installée dans ton projet.
3. Explore les fonctionnalités de l'extension, telles que la vérification de type en temps réel, les suggestions de code, la navigation dans le code et le débogage.
4. Utilise les outils de développement pour améliorer la qualité de ton code et résoudre les problèmes plus rapidement.



## Exercices pratiques - Partie 4 : Types avancés, utilitaires de type, décorateurs avancés et meilleures pratiques

### Exercice 1 : Types avancés

1. Crée un fichier `advanced-types.ts` dans ton projet.
2. Déclare un type `Person` avec les propriétés `firstName`, `lastName` et `age`.
3. Déclare un type `Employee` qui étend le type `Person` et ajoute une propriété `position`.
4. Crée une fonction `printEmployee` qui prend un paramètre de type `Employee` et affiche ses informations dans la console.
5. Utilise la fonction `printEmployee` avec un objet de type `Employee`.
6. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 2 : Utilitaires de type

1. Crée un fichier `type-utilities.ts` dans ton projet.
2. Utilise l'utilitaire de type `Partial` pour créer un type `PartialPerson` basé sur le type `Person` défini précédemment.
3. Utilise l'utilitaire de type `Pick` pour créer un type `PersonName` qui contient uniquement les propriétés `firstName` et `lastName` du type `Person`.
4. Utilise l'utilitaire de type `Omit` pour créer un type `PersonWithoutAge` qui exclut la propriété `age` du type `Person`.
5. Crée des objets de type `PartialPerson`, `PersonName` et `PersonWithoutAge` et utilise-les dans des fonctions ou des opérations appropriées.
6. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 3 : Décorateurs avancés

1. Crée un fichier `advanced-decorators.ts` dans ton projet.
2. Déclare un décorateur de propriété `logProperty` qui affiche le nom de la propriété décorée et sa valeur dans la console lorsqu'elle est modifiée.
3. Déclare un décorateur de paramètre `logParameter` qui affiche le nom du paramètre décoré et sa valeur dans la console lorsqu'il est passé à une méthode.
4. Applique les décorateurs `logProperty` et `logParameter`à une classe, à l'une de ses propriétés et à l'un de ses paramètres de méthode.
5. Compile et exécute le fichier comme dans les exercices précédents.

### Exercice 4 (Conseil Bonus) : Meilleures pratiques

1. Utilise des alias de type pour améliorer la lisibilité et la maintenabilité de ton code.
2. Utilise des interfaces pour définir des contrats entre les classes et les objets.
3. Préfère les `const` assertions pour les objets et les tableaux immuables.
4. Utilise des types génériques pour créer des fonctions et des classes réutilisables.
5. Applique les principes SOLID pour améliorer la qualité et la flexibilité de ton code TypeScript.
