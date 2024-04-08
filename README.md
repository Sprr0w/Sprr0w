console.log("Simulando creación de la carpeta 'GitHub' en Google Drive");

name: Simular creación de carpeta en Google Drive

on:
  push:
    branches:
      - main  # o el nombre de tu rama principal

jobs:
  simular-creacion-carpeta:
    runs-on: ubuntu-latest
    steps:
    - name: Checkout del repositorio
      uses: actions/checkout@v2

    - name: Ejecutar script falso de creación de carpeta
      run: node fake_script.js