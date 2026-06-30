**Piattaforma Social:**

- Utenti, Post, Media, Commenti, Likes

# Utenti

- id            UNIQUE BIGINT PK NN 
- nome          VARCHAR(50) NN
- cognome       VARCHAR(50) NN 
- email         VARCHAR(50) NN  

# Post

- id            UNIQUE BIGINT PK NN 
- id_utente     FK NN
- descrizione   VARCHAR(255) 
- data          DATE
- tag           VARCHAR(255)

# Media

- id            UNIQUE BIGINT PK NN 
- id_utente
- tipo          VARCHAR(50)
- descrizione   VARCHAR(255) 
- data          DATE
- tag           VARCHAR(255) 

# Media_Post
- id_media          BIGINT UNIQUE 
- id_post           BIGINT UNIQUE
- data_creazione    DATE    

# Commenti

- id            UNIQUE BIGINT PK NN 
- id_utente     FK NN     
- data          DATE
- oggetto       VARCHAR(255) 

# Likes

- id            UNIQUE BIGINT PK NN 
- id_post       FK NN
- id_utente     FK NN    
- numeroLike    INT
  
