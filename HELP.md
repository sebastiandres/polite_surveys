# HELP

# Conda

## Crear el ambiente
conda create -n polite_survey

## Instalar librerías
Desde requirements:
source activate polite_survey
pip install -r requirements.txt

## Borrar el ambiente
conda deactivate
conda env remove -n polite_survey

## Mostrar todos los ambientes
conda env list

# Ambiente

## Lanzar en local
gunicorn --config gunicorn_config.py app:app

## Lanzar en server (Segun ProcFile)
gunicorn --worker-tmp-dir /dev/shm --config gunicorn_config.py app:app


