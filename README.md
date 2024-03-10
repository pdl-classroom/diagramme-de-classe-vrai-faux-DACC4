# Diagramme de classe

![Classes](uml/classes.png)

## Vrai ou faux

Etant donné le diagramme de domaine ci-dessus, les assertions suivantes sont-elles vraies ou fausses ? 
- Etudiant est une classe d’association
- Un étudiant peut participer à autant de cours qu’il veut
- Plusieurs professeurs peuvent enseigner la même discipline
- Un professeur peut enseigner plusieurs disciplines
- Un cours peut être enseigner à 2 étudiants
- Un cours peut être enseigner à 20 étudiants

1. **Étudiant est une classe d’association** : Faux. Dans le diagramme, "Étudiant" est représenté comme une classe normale, pas comme une classe d'association. Les classes d'association sont utilisées pour modéliser une relation entre deux classes (ou plus), généralement avec des attributs ou des opérations propres à cette relation. Ici, "Étudiant" ne semble pas jouer ce rôle.

2. **Un étudiant peut participer à autant de cours qu’il veut** : Faux. La multiplicité entre "Étudiant" et "Cours" est spécifiée comme "5..30", ce qui signifie qu'un étudiant doit participer à au moins 5 cours et peut participer à un maximum de 30 cours. Il ne peut donc pas participer à un nombre illimité de cours.

3. **Plusieurs professeurs peuvent enseigner la même discipline** : Impossible à déterminer avec certitude sans informations supplémentaires sur les règles de gestion spécifiques du modèle. Le diagramme montre une relation de "1" à "*" entre "Professeur" et "Discipline", ce qui indique qu'un professeur peut enseigner plusieurs disciplines, mais ne précise pas si plusieurs professeurs peuvent enseigner la même discipline.

4. **Un professeur peut enseigner plusieurs disciplines** : Vrai. La multiplicité "1" -- "*" entre "Professeur" et "Discipline" indique qu'un professeur peut être associé à plusieurs disciplines (de 1 à plusieurs).

5. **Un cours peut être enseigné à 2 étudiants** : Faux. La multiplicité "5..30" entre "Étudiant" et "Cours" signifie qu'un cours doit être enseigné à un minimum de 5 étudiants. Par conséquent, un cours ne peut pas être enseigné à seulement 2 étudiants selon ce modèle.

6. **Un cours peut être enseigné à 20 étudiants** : Vrai. Étant donné la multiplicité "5..30", un cours peut effectivement être enseigné à 20 étudiants, car ce nombre se situe dans l'intervalle spécifié.

## Question ouverte

Représentez la même association avec la notation UML « petit losange » 

- Quelles informations perd-on par rapport au diagramme ci-dessus ? 
