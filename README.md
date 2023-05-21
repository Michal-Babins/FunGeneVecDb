# FunGeneVecDb
Creating vectorized collections from fungal sequences.


## Install
For base requirments
`pip -r install requirements.txt`
manage db connections through docker compose for development 
`docker-compose up -d`
`docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 -d --name mysql mysql:5.7`


## Concept
Vector DB's can be used as a way to vectorize sequencing data, either nucleotides or AAs with the proper embedding models. 
Then we can leverage the vector search to do eitehr similarity search or a list of common algorithms:
- Euclidian Distance
- Edit distance
- Cosine Similarity
- Jaccard Index
- Hamming Distance

And if we wanted to hold the vectorized sequences for downstream analysis like logistic regression or SVM's we could as well. 
