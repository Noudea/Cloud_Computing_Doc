# Api Recettes

Créé par: Nicolas Oudea
Dernière modification: October 24, 2022 5:50 PM
Dernière modification par: Nicolas Oudea
Heure de création: October 24, 2022 11:42 AM

| Recette |  |
| --- | --- |
| ID |  |
| Nom |  |
| Temps |  |
| HowTo |  |
| Produits |  |

## Route API GET : */recettes*

Description : 

Cette route permet de récupérer l’ensemble des recettes du restaurant.

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
    

## Route API GET : */recette/:id*

Description : 

Cette route permet de chercher une recette

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
    
    > Code réponse **200** : Opération réussie
    > 
    
    ```json
    {
    		
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
    

## Route API POST : */recette*

Description : 

Cette route permet de créer une recette

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
    

## Route API PUT : */recette/:id*

Description : 

Cette route permet de modifier une recette

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
    

## Route API DELETE : */recette/:id*

Description : 

Cette route permet de supprimer une recette

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