### Argument splitter français
Cette fonction permet de diviser automatiquement un texte français en phrases verbales distinctes. Une phrase verbale contient un sujet et un verbe conjugué et représente une action ou un argument unique. Les phrases complexes contiennent souvent plusieurs phrases verbales, les séparer permet donc d'identifier des unités de sens.

La fonction repose sur une liste de symboles de ponctuation et de connecteurs logiques utilisés en français. Le plus souvent, les phrases verbales sont articulées via la ponctuation et les connecteurs.

La fonction découpe itérativement le texte sur les symboles de ponctuations et les connecteurs et analyse les morceaux de phrases obtenus à l'aide du parsing SpaCy. Si les deux morceaux obtenus contiennent tous deux un sujet et un verbe conjugué, alors le "split" est gardé, dans l'autre cas le split est rejété.
