<img align="right" src="https://github.com/gislersoft/quoragame/blob/master/quora-logo.png" width="30%" height="30%" style="text-align:center">

# Quora - Abandoned Planet

Quora is a free open source video game used to teach some basic game development using the Unity Engine, the colaborators of this project are basically students of the Universidad Autónoma de Occidente UAO in Cali Colombia.

## Story Plot 2

Is the future year 3145 A.D the Homo Sapiens has been vanished from five planets (Earth, Moon, Mars and Europa) in the solar system for unknown reasons, Only Earth 2 and it´s moon Quora are known as the latest Homo Sapiens Colonies. Earth 2 has lost contact with any Homo Sapiens in Quora (4 years ago),  Quora is at 2 years travel distance from Earth 2 a first mission was sent to the planet looking to solve the mistery but the contact was lost. Earth 2 has send one last mission with no return ticket of one man the Astronaut, Physicist and Soldier Commander Alexandre Bob Martinez Wang.

## Level 1 - The landing

Commander Alexandre is entering on his spaceship to the Quora atmosphere, after landing near to the last known Homo Sapiens base he will discover the solitude and dangers of Quora.

### Level 1 - Mission 1

The Commander needs to shutdown the Sentinel Robot that is in "Base defend mode", but the doors of the base are locked and the switch to shutdown the robot is inside the base, find a way to enter into the base without being killed by the Sentinel. Watch your oxigen and temperature levels.

## Developers Guide

This guide is to download the repository and colaborate with the game, there are some rules and steps that must be followed before you can commit a change.

### Setup

For Windows users:

> **IMPORTANT!!** : Please, before sending any change to the repo verify that you are using **EXACTLY** this Unity version: **``` 2018.1.6f1 Personal ```**

1. Download git https://git-scm.com/downloads
2. Create a public github account
3. Go to https://github.com/gislersoft/quoragame and fork the repository.
4. Create a Unity Project in any local folder. Example: C:\Users\gislersoft\Documents\Unity\UAO\VideoJuegos3D\QuoraRepo
5. Switch to Visible Meta Files in **Edit** → **Project Settings** → **Editor** → **Version Control Mode** → Visible Meta Files
6. Switch to Force Text in **Edit** → **Project Settings** → **Editor** → **Asset Serialization Mode** → Force Text
7. Open git bash (From step 1).
8. ``` cd "C:\Users\gislersoft\Documents\Unity\UAO\VideoJuegos3D\QuoraRepo" ```
9. ``` git init ```
10. ``` git remote add origin https://github.com/gislersoft/quoragame.git ```
11. ``` git remote add fork https://github.com/<YOUR GIT HUB USER HERE>/quoragame.git ```
12. ``` git fetch --all ``` Note: This will take a while until all objects are downloaded.
13. ``` git reset --hard origin/master ``` This will discard all your local changes and just overwrite everything with a copy from the remote branch

### Final checks

Verify with  ``` git status ``` that the only change is the scene you just create, your expected output should be:

 ``` 
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        Assets/Prueba.unity
        Assets/Prueba.unity.meta

nothing added to commit but untracked files present (use "git add" to track)
 ``` 
 
 Verify with ```git remote -v``` that your repo pointer are correct your expected output should be:
 
  ``` 
 $ git remote -v
fork    https://github.com/<YOUR GITHUB USERNAME>/quoragame.git (fetch)
fork    https://github.com/<YOUR GITHUB USERNAME>/quoragame.git (push)
origin  https://github.com/gislersoft/quoragame.git (fetch)
origin  https://github.com/gislersoft/quoragame.git (push)
 ``` 

 If is your firstime using git then configure your basic information using this commands, please do this before send your first commit.

  ``` 
  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"
  ``` 

### Useful commands

Here are some useful GIT commands with their respective explanation in spanish.

- ```git status``` // Verificar los cambios
- ```git remote -v``` // Verificar los apuntadores a los repositorios
- ```git add <file>``` // Agregar el archivo a el cambio
- ```git add .``` // Agregar todos los archivos (Usar con cautela)
- ```git rm <file>``` // Marcar como borrado en el cambio
- ```rm <file>``` //Borrar el archivo del sistema de archivos
- ```git commit -m "bla bla bla"``` // Crear el commit con un mensaje
- ```git push <apuntador> <branch>``` // Enviar los cambios al repositorio y branch apuntados
- ```git pull <apuntador> <branch>``` // Traer los cambios del repositorio y branch apuntados
- ```git remote add <apuntador> <url del repo>``` //Crea un nuevo apuntador para el repositorio dado
- ```git remote remove <apuntador>``` // Borrar el apuntador del repositorio

### Code of conduct (Mejores Prácticas)
- NO USAR ESPACIO EN LOS NOMBRES NADIE QUIERE TENER QUE AGREGAR DOBLE COMILLA EN gitbash
- No enviar PR super masivos (Muchos archivos en un solo PR) usar commits atomicos.
- Usar CamelCase para el nombramiento de variables, metodos, Clases, Texturas, Modelos y Carpetas. Ejemplo: ```MiCarpeta``` , ```miVariable```, ```miMetodo```, ```MiClase```, ```miTextura.png```, ```MiTextura.png```, ```MiModelo```, ```miModelo```.
- Leer los readme de cada carpeta
- Colocar los modelos en una carpeta agrupada.
- Agrupar de manera coherente archivos relacionados entre si cómo por ejemplo archivos relacionados a un mismo modelo.
- Evitar tocar las escenas si no necesito realmente tocarlas, en su lugar utilizar escenas de pruebas y colocarlas en la carpeta de escenas de prueba.
- Utilizar o español o inglés en los comentarios o el código, pero evitar mezclarlos de manera que sea dificil leer el código. Ejemplo de evitar esto: ```int ammo = 20; int municionRate = 10```.
- Los modelos deben estar terminados y haber pasado el proceso de calidad.
- Cumplir con el principio de la menor sorpresa y que las clases y metodos tengan sentido. (Clean Code)


