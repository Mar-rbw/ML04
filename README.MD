dvc init para inicializar Dvc
Para trackear nuestro dataset con dvc
pip install dvc-gdrive
dvc remote modify gdrive-remote gdrive_client_id '64685754570-beml0vv155lsjbi2j46ccnk8tfiqs5t6.apps.googleusercontent.com'
dvc remote modify gdrive-remote gdrive_client_secret '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'
dvc remote add -d gdrive-remote gdrive://folder

# Reemplaza /ruta/al/archivo/ por la ruta real donde guardaste el archivo JSON
$env:GOOGLE_APPLICATION_CREDENTIALS="C:\Users\Marce\OneDrive\Documentos\Github\ML04\ml04-87b10-firebase-adminsdk-fbsvc-45dbab7a05.json"

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