[SEGMENT 01] Administrer un système réel via un LLM non fiable


Un LLM pilotant un OS réel, avec des privilèges réels, dans un contexte où une erreur ne se rembourse pas. L'hypothèse de départ est directe.

Le problème l'est aussi. Un LLM branché directement sur un système critique n'est pas un assistant. C'est une surface d'exposition permanente. Vulnérable à son fournisseur, à ses données d'entraînement, aux attaques par prompt, aux corrélations que personne ne maîtrise entièrement.

Ce n'est pas une limitation à contourner. C'est une propriété structurelle de l'objet.

Le déploiement local ne change rien. Un LLM auto-hébergé conserve les mêmes poids, les mêmes corrélations, les mêmes vecteurs d'attaque via le texte. La menace n'est pas l'endroit où le modèle tourne. C'est le fait qu'il voit la machine telle qu'elle est.

La question ne porte donc pas sur la confiance. Elle porte sur ceci : comment utiliser un modèle potentiellement compromis sans que sa compromission affecte le système qu'il administre. Lui donner les clés fonctionnelles. Ne jamais lui donner les clés structurelles.

SSCG est construit pour casser ce lien.

Le système réel n'est pas projeté dans le texte. Il est traduit dans un vocabulaire symbolique où chaque chemin, chaque identité, chaque service est réduit à un rôle abstrait, interchangeable, réversible, mais uniquement localement. Cette réversibilité reste dans le moteur de résolution. Elle ne remonte jamais vers le LLM.

Le modèle peut demander des opérations, raisonner sur des identités et des services, exploiter son contexte et sa mémoire. Il ne voit jamais la topologie réelle, les valeurs réelles, les invariants du système. Il administre un espace symbolique. Uniquement cela.

Sa fragilité devient un paramètre du modèle. Pas une exception gérée après coup.

Ce segment pose le cadre du problème. Il ne décrit pas encore SSCG. Le suivant détaille les trois niveaux de représentation, les invariants qui encadrent la traduction entre monde réel et monde symbolique, et les conditions où cette abstraction cesse d'être valide.
