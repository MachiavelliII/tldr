# docker build

> Construit une image à partir d'un Dockerfile.
> Plus d'informations : <https://docs.docker.com/reference/cli/docker/buildx/build/>.

- Construire une image Docker en utilisant le Dockerfile du répertoire courant :

`docker build .`

- Construire une image Docker à partir d'un Dockerfile situé à une URL précisée :

`docker build {{github.com/creack/docker-firefox}}`

- Construire une image Docker et l'étiquette :

`docker build {{[-t|--tag]}} {{nom:etiquette}} .`

- Construit une image Docker sans contexte de construction :

`docker build {{[-t|--tag]}} {{nom:etiquette}} - < {{Dockerfile}}`

- Ne pas utiliser le cache lors de la construction de l'image :

`docker build --no-cache {{[-t|--tag]}} {{nom:etiquette}} .`

- Construire une image Docker utilisant un Dockerfile spécifique :

`docker build {{[-f|--file]}} {{Dockerfile}} .`

- Construire avec des variables personnalisées définies à la volée :

`docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .`
