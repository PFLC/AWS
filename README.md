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

Dos vias para acceder a continuación:

# ACCEDER AL SERVIDOR via TERMIUS
- Agregar la llavesita.pem al KEYCHAIN (o llavero) de la APP
