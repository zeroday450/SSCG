[SEGMENT 03] Garanties réelles et périmètre de validité

SSCG ne chiffre rien. Il ne signe rien. Il ne détecte pas les intrusions et ne produit aucun log de sécurité. Ce qu'il garantit est d'un autre ordre : un LLM opérant strictement en N2 ne peut pas produire, même involontairement, une information exploitable sur le système réel. Pas par contrainte cryptographique. Par impossibilité structurelle, le réel n'existe pas dans son espace de travail.

Cette garantie est conditionnelle. Elle tient tant que trois propriétés sont maintenues simultanément : la table de résolution reste localement confinée, N2 ne contient aucune valeur brute, et le périmètre symbolique couvre l'intégralité des états que le système réel peut produire. Si l'une de ces propriétés cède, la garantie cède avec elle. Pas partiellement. Entièrement.

Le cas de rupture le plus structurel n'est pas une attaque. C'est la dérive silencieuse du périmètre. Un élément réel non cartographié introduit un état que N2 ne peut pas représenter. Le moteur ne peut ni le traduire ni l'ignorer sans risque. La seule réponse valide est le blocage. Ce blocage n'est pas récupérable depuis l'espace symbolique, il exige une intervention humaine directe sur SSCG.txt. L'opérateur n'est pas un superviseur optionnel. Il est une dépendance structurelle du système.

La non-injectivité de N1 → N2 introduit une limite distincte. Plusieurs éléments réels peuvent partager un rôle sémantique, c'est une propriété voulue. Elle devient un vecteur si un adversaire introduit un élément dans N0 en ciblant un rôle déjà actif. Le modèle continue d'agir sur ce qu'il croit être le même rôle. SSCG ne détecte pas cette substitution. Ce cas n'est pas résolu. Il est posé comme limite explicite du modèle.

Ce que SSCG garantit est précis et borné. Ce qu'il ne garantit pas l'est tout autant.
