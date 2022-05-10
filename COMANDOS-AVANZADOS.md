# Comandos avanzados GIT

## Introducción

En esta sección nos centraremos en problematicas en la que necesitamos ejecutar mas de un comando.
Tambien podremos encontrar solución a posibles errores

## 1.Como trabajar con una rama remota

Primero descargamos desde el repositorio remoto

```bash
git clone https://github.com/airarrazabald/Comandos-git.git
```

Nos posicionamos en la carpeta creada Comandos-git

```bash
cd comandos-git
```

Ya posicionados ejecutamos el comando

```bash
git checkout -b Correccion-comandos
```

Si necesitamos subir la rama al repositorio remoto el siguiente comando lo creara si no existe

```bash
git push origin Correccion-comandos
```

## 2.Solución al error 'failed to push some refs to'

Este error se origina al momento de realizar push al repositorio remoto.
El origen de este problema lo desconozco al momento de escribir estas notas.
Una posible solución y que me funciono es agregar el head al momento de realizar el push
Comando con error:

```bash
git push origin Correccion-comandos
```

Comando agregando HEAD para que si funcione

```bash
git push origin HEAD:Correccion-comandos
```

Considerar que esto aplica solo si presentes el error que se comentta en el titulo failed to push some refs to
