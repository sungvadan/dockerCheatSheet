#commande boot2docker
`boot2docker up  # Permet de démarrer la machine contenant docker`

`boot2docker stop # Permet de l'arrêter`

`boot2docker ssh  # Permet de se connecter en ssh `

`boot2docker ip # Permet d'obtenir l'ip de la machine`

`boot2docker ip # afficher ip de docker`

#configurer boot2docker

`cd /var/lib/boot2docker/`

`touch /var/lib/boot2docker/bootlocal.sh`

`mkdir /var/www`

`mount -t vboxsf www /var/www`

`echo 'alias composer=\'docker run -ti --rm -v $(pwd):/app composer/composer\'' >> home/docker/.ashrc`


#commande docker

## run un  contenneur
1. `docker run --name apache --rm -p 80:80 -v /var/www:/app tutum/apache-php -e ALLOW_OVERRIDE=true`
    * `-rm #supprimer machine lors d'arrêter`
    * `-p port`
    * `-v monter dossierr`
    * `-e variable environnement`
    



## lister toutes les images
`docker images`


##execute une commande dans le contenneur
`docker exec -ti apche bash #apache est le nom du contenneur`

## lister les contenneurs qui sont en train de tourner
`docker ps -a`




