# Compartir el formato de mensajes de GIT commit
> Sin configuración específica de GIT, compartir el mismo formato de mensajes de GIT entre todo el equipo de desarrolladores

![GitHub](https://img.shields.io/github/license/mbelchin/git-messages-format.svg)
![GitHub release](https://img.shields.io/github/release/mbelchin/git-messages-format.svg)


[![Twitter](https://img.shields.io/twitter/url/https/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fmbelchin%2Fgit-messages-format&hashtags=git,hooks,developers,commit,format)


*Lee esta información en otros idiomas: [English](README.md), [Español](README.es.md).*

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

_Más información, por favor, visita [https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/](https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/)._

## Author

[Moisés Belchín](https://moisesbm.wordpress.com)


[@moises_b_m](https://twitter.com/moises_b_m)


[https://github.com/mbelchin/](https://github.com/mbelchin/)

Distribuido bajo lincencia MIT. Echa un vistazo a ``LICENSE`` para más información.

[https://github.com/mbelchin/](https://github.com/mbelchin/)

## Documentación

Para obtener una información más detallada acerca de este paquete, por favor, dirígete a :
[https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/](https://moisesbm.wordpress.com/2018/09/15/git-commit-messages-shareable-format/)

## Discusión

Este proyecto fue creado para encontrar una manera simple de compartir el mismo estilo de mensajes de GIT con todo un equipo de desarrolladores.

Si consideras que algunas cosas podrían mejorarse o si conoces alguna otra herramienta más sencilla o con una configuración más fácil, por favor, abre un hilo de debate para que todos nos podamos beneficiar de todas las mejoras que surjan.

## Contribuir

1. Haz un fork (<https://github.com/mbelchin/git-messages-format/fork>)
2. Crea una nueva rama (`git checkout -b feature/fooBar`)
3. Haz un commit de tus cambios (`git commit -am '<type>(scope): add some fooBar'`)
4. Haz push de tu rama (`git push origin feature/fooBar`)
5. Crea un nuevo Pull Request
