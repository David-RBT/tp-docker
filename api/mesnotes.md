Pour l'api 
j'ai d'abord crée un dockerfile avec les même info que le front les seul différences étaient le nom du dossier et aussi le port exposé 
j'ai aussi crée un fichier .dockerignore pour filtrer certains dossiers.
comme commande j'ai utilisé 
docker build -t mon-api .
et je l'ai lancé dans docker desktop et j'ai réussi à voir le message
ensuite pour la partie de render 
j'ai utilisé 
 docker tag mon-api davidbekale/mon-api
 ensuite 
 docker push davidbekale/mon-api
 et après sur render j'ai configuré manuellement
 au niveau du docker compose 
 j'ai utilisé docker compose up mais il ny'a que le premère image qui se lance