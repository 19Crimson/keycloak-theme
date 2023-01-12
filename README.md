Репозиторий содержит файлы для модификации docker образа Keycloak

Работа файлов темы и локализации проверена на версии docker образа [jboss/keycloak v 15.1.1](https://hub.docker.com/r/jboss/keycloak/tags)

Клонируем файлы темы из репозитория

```git clone https://github.com/19Crimson/keycloak-theme.git```

Копируем файлы темы в контейнер

```docker cp {REPO_PATH}\keycloak-theme\aml {C_NAME}:/opt/jboss/keycloak/themes```

REPO_PATH - путь до папки с репозиторием keycloak-theme
C_NAME - имя контейнера

Чтобы переключить тему, необходимо зайти в админку и выбрать тему aml в  Themes -> Login Theme
