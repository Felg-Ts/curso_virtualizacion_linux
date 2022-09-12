# Introducción a Linux Containers (LXC)

**LinuX Containers**, también conocido por el acrónimo **LXC**, es una tecnología de virtualización ligera o por contenedores, que es un método de virtualización en el que, sobre el núcleo del sistema operativo se ejecuta una capa de virtualización que permite que existan múltiples instancias aisladas de espacios de usuario, en lugar de solo uno. A estas instancias la llamamos **contenedores**.

**LXC** pertenece a los denominados **contenedores de sistemas**, su gestión y ciclo de vida es similar al de una máquina virtual tradicional. Está mantenido por Canonical y la página oficial es [linuxcontainers.org](https://linuxcontainers.org/).

## Instalación de LXC

Vamos a trabajar sobre una distribución GNU/Linux Debian 11. Para la instalación de LXC ejecutamos:

```
apt install lxc
```

lxc-create -t download -n u1 -- -d ubuntu -r DISTRO-SHORT-CODENAME -a amd64