Clase 02 - Git Desarrollo Colaborativo
Para ver el estado de los archivos y en que área de git están
git status
Para pasar los archivos del Working Directory al Staging Area (index area)
git add .
git add <carpeta>/<archivo>
git add <carpeta1>/<archivo1> <carpeta1>/<archivo2> <carpeta1>/<archivo3>
Para pasar de SA a el LR
git commit # Editor de texto para colocar el mensaje
git commit -m "mensaje descriptivo"
Diferencia entre el archivo/s que están Working Directory contra el Local Repo
git diff # compara el archivo que está en WD con el archivo que está en LR
Ver el contenido del commit
git show <hash>
git show 01b82c5
Ver de manera corta el status de los archivos y en que área están
git status --short
Ver timeline de commits
git log --oneline # forma corta
git log # forma larga (detallada)
git log --oneline -<cantidad de commits> 
git log --oneline -2 # ver una cantidad de commit especifica
Subir el repo local al remoto
git push
Agregar la url del remoto al local
git remote add <alias> <url-al-remoto>
git remote add origin https://github.com/mlapeducacionit/80746-git-desarrollo-colaborativo.git
Controlar que se haya colocando la url en el local
git remote 
git remote -v # más dentalle
Para subir al repositorio remoto
git push -u <remoto> <rama>
git push -u origin main # relacionar la rama local con la remota
git push # Una vez asociadas (relacionadas) no necesito volver a indicarle el remoto y la rama