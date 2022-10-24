# Api Gestion des stocks et prix de produits alimentaires

Créé par: Nicolas Oudea
Dernière modification: October 24, 2022 5:49 PM
Dernière modification par: Nicolas Oudea
Heure de création: October 24, 2022 11:43 AM

| Produit |  |
| --- | --- |
| ID |  |
| Nom |  |
| Prix |  |
| Stock |  |

## Route API GET : */produits*

Description : 

Cette route permet de récupérer l’ensemble des produits.

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
    

## Route API GET : */produit/:id*

Description : 

Cette route permet de chercher un produit

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
    

## Route API POST : */produit*

Description : 

Cette route permet de créer un produit

---

- Voir détails
    
    ### Paramètres d’entrée
    
    ```jsx
    {
    	"name": "test",
      "prix": 30,
      "stock": 6
    }
    ```
    
    ---
    
    ### Réponses
    
    > Code réponse **201** : Opération réussie
    > 
    
    ```json
    {
    	"name": "test",
    	"prix": 30,
    	"stock": 6,
    	"_id": "63569df4bab7774d9124c453",
    	"createdAt": "2022-10-24T14:18:07.044Z",
    	"updatedAt": "2022-10-24T14:18:07.044Z",
    }
    ```
    
    > Code réponse **400** : Bad Request
    > 
    
    ```json
    {
    	"name" : "salut",
    	"description" : "" 
    }
    ```
    

## Route API PUT : */produit/:id*

Description : 

Cette route permet de modifier un produit

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
    

## Route API DELETE : */produit/:id*

Description : 

Cette route permet de supprimer un produit

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