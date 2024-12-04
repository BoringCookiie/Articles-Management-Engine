User :
•	Voir les articles
•	Ajouter des commentaires
Admin :
•	Create, update, delete articles
•	Management des categories
Features :
•	Les articles sont organisés par des catégories
•	Tags pour les articles
Structure de base de donnees : 
•  users:
•	id, name, email, password, created_at, updated_at.
•	This will store information about the users, including the authors.
•  articles:
•	id, title, content, category_id, author_id, created_at, updated_at.
•	author_id is a foreign key referencing the users table to indicate the author of the article.
•  categories:
•	id, name, created_at, updated_at.
•  tags:
•	id, name, created_at, updated_at.
•  article_tag (pivot table):
•	article_id, tag_id.
•  comments:
•	id, article_id, user_id, content, created_at, updated_at.



