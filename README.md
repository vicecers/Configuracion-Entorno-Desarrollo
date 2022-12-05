
## Git

Instalar Git:

```sh
$ sudo apt-get install git
```

Configurar usuario global:

```sh
$ git config --global user.name "Mi nombre"
$ git config --global user.email "mi@correo.com"
```


## JRE

Instalar Java

```sh
$ sudo apt install default-jre
```

## JDK

Default JDK

```sh
$ sudo apt-get install default-jdk
```

JDK 11

```sh
$ sudo apt install openjdk-11-jdk
```

JDK 9

```sh
$ sudo apt install openjdk-9-jdk
```

JDK 8

```sh
$ sudo apt install openjdk-8-jdk
```

update-alternatives (Gestor de versiones java)

```sh
$ sudo update-alternatives --config java
```

set JAVA_HOME

```sh
export JAVA_HOME=/usr/lib/jvm/{jdk_install_dir}
export PATH=$JAVA_HOME/bin:$PATH
```

Ejemplo, JDK 8:

```sh
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
export PATH=$JAVA_HOME/bin:$PATH
```


## VSCODE

Instalar VSCODE

Actualizar Linux Mint
```sh
sudo apt update && sudo apt upgrade -y
```
Instalar paquetes requeridos
```sh
sudo apt install software-properties-common apt-transport-https wget -y
```
Importar repositorio de código de Visual Studio
```sh
sudo wget -O- https://packages.microsoft.com/keys/microsoft.asc | sudo gpg --dearmor | sudo tee /usr/share/keyrings/vscode.gpg
```
En segundo lugar, importe el Repositorio de Microsoft Visual Source con el siguiente comando en su terminal.
```sh
echo deb [arch=amd64 signed-by=/usr/share/keyrings/vscode.gpg] https://packages.microsoft.com/repos/vscode stable main | sudo tee /etc/apt/sources.list.d/vscode.list
```
Instalar código de Visual Studio
```sh
sudo apt update
sudo apt install code -y
```
