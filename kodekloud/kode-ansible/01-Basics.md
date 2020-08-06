# Instalación de Helm

_Esta guía os muestra cómo se debe hacer para instalar helm en nuestro ordenador_

## Release 2.14.3

Es necesario descargar la [release v2.14.3](https://github.com/helm/helm/releases/tag/v2.14.3)

### Instalación en linux

_El proceso de instalación es el siguiente:_


Descargar la release
```
$ wget https://get.helm.sh/helm-v2.14.3-linux-amd64.tar.gz
```
Una vez descargada la release, desempaquetar el fichero

```
$ tar -zxvf helm-v2.14.3-linux-amd64.tar.gz
```

luego ingresar en la carpeta descomprimida, y mover los ficheros helm y tiller a la ruta /usr/local/bin

```
$ mv linux-amd64/helm linux-amd64/tiller /usr/local/bin

```

#### Validación

Después de mover los ficheros, se procede a validar que tanto helm como tiller estén correctamente instalados.

```
$ helm version
$ tiller version
```

### Instalación en Windows

_El proceso de instalación es el siguiente:_

Instalar a través del gestor de paquetes de Windows chocolatey. Para más información visite [chocolatey](https://chocolatey.org/) 

```
> choco install kubernetes-helm --version=2.14.3
```

#### Validación

Después de que termine el proceso de instalación, se procede a validar que el helm este correctamente instalados

```
> helm version
```

### Instalación en MAC

_El proceso de instalación es el siguiente:_

Instalar a través del gestor de paquetes de MAC homebrew. Para más información visite [homebrew](https://brew.sh/index_es) 

```
brew install helm
```

#### Validación

Después de que termine el proceso de instalación, se procede a validar que el helm este correctamente instalados

```
helm version
```
