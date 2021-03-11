Comment créer un nouvelle objet :
    {
    "tag" : "_POULETCRUD",
    "name" : "Sandwich poulet crudité",
    "description" : "Le bon poulet crud du crous à 1 euro, merci l'état providence.",
    "price" : 2,
    "value" : 1,
    "type" : "BUFFER",
	
//BUFFER
    "type_var" : "CLICK_AMOUNT",
    "op" : "ADD",
    "maxLevel" : 5,

//SKILL
	"type_skill" : "RACKET",
    "duration" : 10,
    "cooldown" : 20
    },

-> Rajouter deux accolades : elles représentent un objet, ici une amélioration.
-> Si ce n'est pas le dernier objet, rajouter une virgule derrière la dernière accolade.
-> Rajouter 7 variable comme l'exemple ci dessus avec exactement les même noms.
-> tag : il doit commencer par un _ (underscore) et être en majuscule sans espace.
-> name : Le nom, libre.
-> description : libre
-> price : le prix, obligatoirement un entier.
-> type : BUFFER ou SKILL le buffer est une amélioration d'une variable, un skill est une action débloquable.
-> type_var : Si BUFFER vous pouvez choisir d'améliorer une seul variable par upgrade, voici la liste des variables :
    - CLICK_AMOUNT : nombre de $ par click
    - CLICK_TIME : reduit le delais entre les clicks
    - DELIVERY_TIME : temps de livraison
    - DELIVERY_AMOUNT : rémunération de la livraison
    - IMPOSITION : taxe de l'ursaff en %
 Note : Si skill mettre NONE
-> op : L'opération qu'on souhaite appliquer à la variable choisie :
    - ADD : additionne la variable à la valeur de l'upgrade
    - MULTIPLY : muliplie la variable à la valeur de l'upgrade
    - SET : Assigne la variable à la valeur de l'upgrade (préférer ne pas l'utiliser)
-> value : valeur de l'upgrade, peut être un nombre entier ou à virgule (10^-7) utiliser dans le buffer et le skill
-> maxLevel : le nombre de level max que peut bénéficier l'amélioration, à chaque lvl l'effet va être appliquer une nouvelle fois.
-> type_skill : le skill impacté par l'upgrade :
    - RACKET : Skill de braquer une banque
    - STOCK_MARKET : Skill placement en bourse
Note : Nous pouvons en ajouter de nouveau personnalisé
-> duration : la durée de la compétence(skill),mettre -1 si instantanée
-> cooldown : la durée de recharge de la compétence (mettre -1 si pas de recharge)
