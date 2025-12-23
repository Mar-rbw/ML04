dvc init para inicializar Dvc
Para trackear nuestro dataset con dvc
pip install dvc-gdrive
dvc remote add -d gdrive-remote gdrive://folder

# Reemplaza /ruta/al/archivo/ por la ruta real donde guardaste el archivo JSON
$env:GOOGLE_APPLICATION_CREDENTIALS="C:\Users\Marce\OneDrive\Documentos\Github\ML04\"

git tag -a v0 -m 'version 0'

Flow
1.-(Se agrega una imagen)
2.-dvc add dataset
3.-dvc push
4.- git tag -a <vX> -m '<version x>'
5.-git add .
6.- git commit -m 'nueva version'
7.-git push
8.- git push origin --tags

Pasar de una version a otra
git checkout tags/v0
dvc pull
