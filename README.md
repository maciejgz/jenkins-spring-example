Aplikacja spring boot releasowej na heroku przy użyciu jenkins stawianym na dockerze.

Elementy do konfiguracji:
- uruchomienie jenkinsa z dockera - koniecznie utworzyć volume
- w jenkinsie zainstalować wszystkie dodatki
- job jenkinsa zdefiniowany w Jenkinsfile na repo
- konfiguracja mavena w jenkinsie
- dodanie jako zmiennej sytemowej HEROKU_API_KEY (klucz konta) w jenkinsie - to jest wymagane przez heroku maven plugin do deployu aplikacji bez podawania danych w pom



### start jenkins using docker-compose
`docker-compose -f docker/jenkins.yml up -d`

Docker is up on:
    
        http://192.168.99.100:8080/





