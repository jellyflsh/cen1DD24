Espace de gestion de fichiers du cours M1 CEN DD 2024
https://eyak09.github.io/cen1DD24/


requête wikidata html :

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    SELECT ?système_solaire ?auteur_ou_autrice__chaîne_ ?sujet_ou_thème_principal ?sujet_ou_thème_principalLabel ?titre ?date_de_publication WHERE {
        SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],mul,en". }
        ?système_solaire wdt:P921 wd:Q544.
        OPTIONAL {  }
        OPTIONAL {  }
        OPTIONAL { ?système_solaire wdt:P2093 ?auteur_ou_autrice__chaîne_. }
        OPTIONAL {  }
        OPTIONAL { ?système_solaire wdt:P921 ?sujet_ou_thème_principal. }
        OPTIONAL {  }
        OPTIONAL {  }
        OPTIONAL { ?système_solaire wdt:P1476 ?titre. }
        OPTIONAL {  }
        OPTIONAL { ?système_solaire wdt:P577 ?date_de_publication. }
      }   
</body>
</html>
