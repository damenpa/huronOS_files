# huronOS

Guía rápida de descarga, configuración y despliegue de huronOS.

## Descarga de la imagen

Las imágenes se publican en el mirror oficial:

- <https://mirrors.huronos.org/huronOS/alpha/>

```bash
wget https://mirrors.huronos.org/huronOS/alpha/huronOS-alpha-0.4-amd64.iso
```

## Archivo de configuración del HDF

El archivo que contiene la URL del HDF se encuentra en:

```text
/run/initramfs/memory/system/huronOS/data/configs/sync-server.conf
```

## Aplicar el wallpaper

```console
root@huronOS:/home/contestant# hos-wallpaper --automatic
/tmp/verify-download-62044 /home/contestant
/home/contestant
```

## Ejemplo de instalación

```bash
./install.sh --directives-url https://raw.githubusercontent.com/damenpa/huronOS_files/main/directives.hdf --directives-server-ip 1.1.1.1 --root-password toorx
```
