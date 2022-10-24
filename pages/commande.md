# Api Gestion des commandes de plats cuisinés avec quantité et prix

Créé par: Nicolas Oudea
Dernière modification: October 24, 2022 5:49 PM
Dernière modification par: Nicolas Oudea
Heure de création: October 24, 2022 11:43 AM

| Commande |  |
| --- | --- |
| ID |  |
| Plats |  |
| Date |  |
| Client |  |
| Prix |  |

## Route API GET : */commandes*

Description : 

Cette route permet de récupérer l’ensemble des commandes.

---

- Voir détails
    
    ### Paramètres d’entrée
    
    Aucun
    
    ---
    
    ### Réponses
    
    > Code réponse **200** : Opération réussie
    > 
    
    ```json
    {
    		recettes : [
    			{
    				"id": "354",
    				"nom": "Butter Chicken",
    				"temps": 
    			}
    		]
    }
    ```
    
    > Code réponse **400** : Bad Request
    > 
    
    ```json
    {
      errors : [
    		{
    			"idMessage": "163534DFFH22",
    		  "message": "Erreur synthaxe manquante ou invalide"
    		}
    	]
    }
    ```
    

## Route API GET : */commande/:id*

Description : 

Cette route permet de chercher une commande

---

- Voir détails
    
    ### Paramètres d’entrée
    
    ```jsx
    {
      _id: "6789UHGVHI",
    }
    ```
    
    ---
    
    ### Réponses
    
    > Code réponse **200** : Opération réussie
    > 
    
    ```json
    {
    		_id : "" 
    }
    ```
    
    > Code réponse **400** : Bad Request
    > 
    
    ```json
    {
      errors : [
    		{
    			"idMessage": "163534DFFH22",
    		  "message": "Erreur synthaxe manquante ou invalide"
    		}
    	]
    }
    ```
    

## Route API POST : */commande*

Description : 

Cette route permet de créer une commande

---

- Voir détails
    
    ### Paramètres d’entrée
    
    ```jsx
    {
      "_id": "6789UHGVHI",
    }
    ```
    
    ---
    
    ### Réponses
    
    > Code réponse **201** : Opération réussie
    > 
    
    ```json
    {
    		//renvoir recette
    }
    ```
    
    > Code réponse **400** : Bad Request
    > 
    
    ```json
    {
    	name : "salut",
    	description : "" 
    }
    ```
    

## Route API PUT : */commande/:id*

Description : 

Cette route permet de modifier un commande

---

- Voir détails
    
    ### Paramètres d’entrée
    
    ```jsx
    {
      "_id": "6789UHGVHI",
    	"name": "",
    	"": ""
    }
    ```
    
    ---
    
    ### Réponses
    
    > Code réponse **200** : Opération réussie
    > 
    
    ```json
    {
    		"idMessage": "163534DFFH22",
    		"message": "Successfully updated"
    }
    ```
    
    > Code réponse **201** : Opération réussie, création d’un objet
    > 
    
    ```json
    {
    		"idMessage": "163534DFFH22",
    		"message": "Successfully created"
    }
    ```
    
    > Code réponse **400** : Bad Request
    > 
    
    ```json
    {
      "idMessage": "163534DFFH22",
    	"message": "Error, bad request"
    }
    ```
    

## Route API DELETE : */commande/:id*

Description : 

Cette route permet de supprimer un commande

---

- Voir détails
    
    ### Paramètres d’entrée
    
    ```jsx
    {
      "_id": "6789UHGVHI",
    }
    ```
    
    ---
    
    ### Réponses
    
    > Code réponse **201** : Opération réussie
    > 
    
    ```json
    {
    		//renvoir recette
    }
    ```
    
    > Code réponse **400** : Bad Request
    > 
    
    ```json
    {
    	name : "salut",
    	description : "" 
    }
    ```