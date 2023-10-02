# How to use querySelector()

Pour utiliser document.querySelector() dans votre code JavaScript, vous devez d'abord importer le module `document`. Vous pouvez le faire en ajoutant la ligne suivante au début de votre code :

JavaScript

```
import { document } from "https://unpkg.com/jsdom@16.2.0/dist/jsdom.min.js";
```

Utilisez le code avec précaution. 

content_copy

Une fois que vous avez importé le module `document`, vous pouvez utiliser la méthode `querySelector()` pour rechercher un élément dans le document. La syntaxe est la suivante :

JavaScript

```
const element = document.querySelector(selector);
```

Utilisez le code avec précaution.


Où `selector` est un sélecteur CSS qui correspond à l'élément que vous souhaitez rechercher.

Par exemple, la ligne suivante recherchera un élément `div` avec la classe `my-class` :

JavaScript

```
const element = document.querySelector(".my-class");
```

Utilisez le code avec précaution.


Si l'élément est trouvé, la méthode `querySelector()` retournera un objet `Element` qui représente l'élément. Sinon, elle retournera `null`.

Vous pouvez ensuite utiliser l'objet `Element` pour accéder aux propriétés et aux méthodes de l'élément. Par exemple, la ligne suivante affichera le contenu de l'élément :

JavaScript

```
const element = document.querySelector(".my-class");
console.log(element.textContent);
```

Utilisez le code avec précaution.



Voici quelques exemples d'utilisation de document.querySelector() :

JavaScript

```
// Rechercher un élément par son id
const element = document.querySelector("#my-id");

// Rechercher un élément par son nom
const element = document.querySelector("input[name='my-input']");

// Rechercher un élément par sa classe
const element = document.querySelector(".my-class");

// Rechercher un élément par son type
const element = document.querySelector("img");

// Rechercher un élément par son tag
const element = document.querySelector("div");
```

Utilisez le code avec précaution. 

content_copy

**Obtenir la valeur d'un input avec document.querySelector()**

Pour obtenir la valeur d'un input avec document.querySelector(), vous pouvez utiliser la méthode `value` de l'objet `Element`. La syntaxe est la suivante :

JavaScript

```
const element = document.querySelector("input[name='my-input']");
const value = element.value;
```

Utilisez le code avec précaution.

content_copy

Par exemple, la ligne suivante affichera la valeur d'un input dont l'attribut `name` est `my-input` :

JavaScript

```
const element = document.querySelector("input[name='my-input']");
const value = element.value;
console.log(value);
```

Utilisez le code avec précaution.

content_copy

**Rechercher plusieurs éléments avec document.querySelector()**

Si vous souhaitez rechercher plusieurs éléments avec document.querySelector(), vous pouvez utiliser la méthode `querySelectorAll()`. La syntaxe est la suivante :

JavaScript

```
const elements = document.querySelectorAll(selector);
```

Utilisez le code avec précaution.

content_copy

Où `selector` est un sélecteur CSS qui correspond aux éléments que vous souhaitez rechercher.

Par exemple, la ligne suivante recherchera tous les éléments `div` avec la classe `my-class` :

JavaScript

```
const elements = document.querySelectorAll(".my-class");
```

Utilisez le code avec précaution.

content_copy

L'objet `NodeList` retourné par la méthode `querySelectorAll()` contient un élément `Element` pour chaque élément correspondant au sélecteur spécifié. Vous pouvez ensuite accéder aux éléments de la liste en utilisant une boucle `for` ou une boucle `forEach`.

JavaScript

```
const elements = document.querySelectorAll(".my-class");

for (const element of elements) {
  console.log(element.textContent);
}
```

Utilisez le code avec précaution. 

content_copy

**Conclusion**

La méthode `querySelector()` est un outil puissant qui vous permet de rechercher des éléments dans le document. Elle est facile à utiliser et peut être utilisée pour une variété de tâches, telles que l'obtention de la valeur d'un input ou la recherche d'un élément par son id ou sa classe.

tuneshare

more_vert

add_photo_alternate
