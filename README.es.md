# Compartir el formato de mensajes de GIT commit
> Sin configuración específica de GIT, compartir el mismo format de mensajes de GIT entre todo el equipo de desarrolladores

![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)

Sin necesidad de configuración de GIT, tener un formato común de mensajes de GIT commit para poder utilizarlo por todo el equipo de desarrollo utilizando hooks nativos de GIT

![](example.gif)

## Instalación

OS X, Linux & Windows:

```
npm install
```

## Ejemplo de uso

NPM instalará los paquetes de npm `husky` y `commitlint`. Estos paquetes son 
los responsables de instalar y lanzar los hooks de GIT.

Dentro del fichero `package.json` encontrarás la configuración necesaria para
`husky`.
En este caso de uso, utilzamos los hooks de GIT `commit-msg` y `post-merge`.

```
"husky": {
  "hooks": {
    "commit-msg": "commitlint -E HUSKY_GIT_PARAMS",
    "post-merge": "npm install"
  }
}
```

_Más información, por favor, visita [https://moisesbm.wordpress.com](https://moisesbm.wordpress.com)._

## Meta

Moisés Belchín – [@moises_b_m](https://twitter.com/moises_b_m) – moisesbelchin@gmail.com

Distribuido bajo lincencia MIT. Echa un vistazo a ``LICENSE`` para más información.

[https://github.com/mbelchin/](https://github.com/mbelchin/)

## Contribuir

1. Haz un fork (<https://github.com/mbelchin/git-messages-format/fork>)
2. Crea una nueva rama (`git checkout -b feature/fooBar`)
3. Haz un commit de tus cambios (`git commit -am '<type>(scope): add some fooBar'`)
4. Haz push de tu rama (`git push origin feature/fooBar`)
5. Crea un nuevo Pull Request
