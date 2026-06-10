# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

luego de creado el proyecto, instalar ansible.
Antes de empezar, asegúrate de tener Python instalado (se recomienda Python 3). Puedes verificarlo ejecutando:
```sh
python3 --version
```
posteriormente configurar el repositorio oficial (PPA) y luego instalarlo así:

```sh
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```
verifica que la instalación este correcta mediante
```sh
ansible --version
```
Con ansible instalado creamos los archivos deploy.yml y hosts.ini que encuentras en el repositorio.

Y finalmente ejecutas el playbook deploy.yml mediante el comando

```sh
ansible-playbook -i hosts.ini deploy.yml -K
```
# pruebas-gestion
