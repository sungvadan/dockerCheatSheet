#commande boot2docker
`boot2docker up  # Permet de démarrer la machine contenant docker`
`boot2docker stop # Permet de l'arrêter`
`boot2docker ssh  # Permet de se connecter en ssh `
`boot2docker ip # Permet d'obtenir l'ip de la machine`
`boot2docker ip # afficher ip de docker`

#Monter le dossier de partage

`cd /var/lib/boot2docker/`
`touch /var/lib/boot2docker/bootlocal.sh`
`mkdir /var/www`
`mount -t vboxsf www /var/www`


#commande docker



## lister toutes les images
`docker images`


##execute une commande dans le contenneur
`docker exec -ti apche bash #apache est le nom du contenneur`

## lister les contenneurs qui sont en train de tourner
`docker ps -a`

## run un  contenneur
`docker run --name apache --rm -p 80:80 tutum/apache-php`

