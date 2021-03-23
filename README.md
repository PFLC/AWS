![](https://de8964361f4bb909de8d-fe8b524ce0801bda0a4b2a48b0c06837.ssl.cf4.rackcdn.com/aKP5jfzpYGi6onA5crCDocysvw9ggtPgErjm5QPWLo6EPoGUVyiYziQKc42nuiDH.1532667105/AWSLogocloud.png)

Pasos para tener su LAMP server en Ubuntu 20 dentro de AWSEducate

- Acceder a su beca de AWSEducate.com de $50 dolares y via CONSOLA invocar EC2 
- EC2: Plan básico de Ubuntu 20 “FREE TIER” (libre de cobro)
- EC2: Seleccionar todo por DEFAULT
- EC2: SECURITY GROUPS habilitar "HTTP, HTTPS y SSH" de la lista de firewall de AWS apuntando a 0.0.0.0 (todo el mundo accesa)
- EC2: Anotar la direccion IP para acceder en el siguiente paso.
- EC2: Teclear "llave" de acceso con un nombre de archivo fácil de recordar (ejemplo: llavesita.pem)
- Descargar: TERMIUS.com o Git For Windows https://git-scm.com/download/win para WINDOWS
- Descargar: en macOS y Linux es opcional pero puede usar TERMIUS.com si lo prefiere, para Android e Iphone es bienvenido instalarlo.
- VIDEO PARTE 1:https://youtu.be/YwmyVAnQ0RI

Dos vias para acceder a continuación:

# ACCEDER AL SERVIDOR via TERMIUS
- Agregar la llavesita.pem al KEYCHAIN (o llavero) de la APP en Android/iphone solo copiar el TEXTO en area PrivateKEY
- -Video para Iphone: https://youtu.be/71hE_9ke6k4
- Agregar HOST (Direccion-ip-de-AWS)
- Agregar IP Direccion-ip-de-AWS
- Anotar el usuario es "ubuntu" minusculas sin contraseña
- KEY es la *llavesita.pem* que esta descargas en su PC al crear AWS EC2 instancia
- Y conectarse.
- NOTA: poner bien la direccion IP no agregar espacios despues o antes, TERMIUS marca error.


# ACCEDER CON GIT-FOR-WINDOWS, macOS y Linux
$ cd descargar (el directorio donde esta la llavesita.pem)
$ chmod 400 llavesita.pem
$ ssh -i llavesita.pem ubuntu@Direccion-ip-de-AWS

# INCIAR INSTALACION LAMP
´´´
sudo su
apt-get -y install wget git
git clone https://github.com/teddysun/lamp.git
cd lamp
chmod 755 *.sh
./lamp.sh
´´´
Y esperar 25 minutos promedio, por tal ocuparemos crear nuestro DOMINIO GRATUITO en NAME.COM con la beca de GitHub Pro
VIDEO PARTE 2: https://youtu.be/4qD030SzmH8



