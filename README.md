<a name="readme-top"></a>

<div align="center">
<a href="https://github.com/midudev/landing-gta-vi">
  <img width="300px" src="https://raw.githubusercontent.com/midudev/landing-gta-vi/refs/heads/main/src/assets/full-logo.webp" alt="Logo de Grand Theft Auto" width="800" />
</a>

## Landing de la web del Grand Theft Auto VI
 [Reportar error](https://github.com/midudev/landing-gta-vi/issues) · [Sugerir algo](https://github.com/midudev/landing-gta-vi/issues)

</div>


## Para empezar

### Prerequisitos

- NVM (recomendado para asegurar versión de Node) ver [documentación oficial](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating)

  ```sh
  nvm use
  # o
  nvm use <version>
  ```

  > Si quieres automatizar el proceso, puedes crear un script siguiendo la [documentación oficial](https://github.com/nvm-sh/nvm?tab=readme-ov-file#calling-nvm-use-automatically-in-a-directory-with-a-nvmrc-file)

<details>
    <summary>Pequeño script de automatización</summary>
    
- En Linux/MacOS:
    ```sh
    # .bashrc | .zshrc | cualquier archivo de configuración
    # pequeño script para cambiar de version al entrar al directorio
    cd() {
  builtin cd "$@"
        if [[ -f .nvmrc ]]; then
            nvm use > /dev/null
            # Si quieres que te diga la versión
            nvm use
        fi
    }
    ```

- En Windows:

  ```powershell
  # $PROFILE
  function Change-Node-Version {
    param($path)
    & Set-Location $path
    $pwd = pwd
    if ( Test-Path "$pwd\\.nvmrc" ) {
        $version = Get-Content .nvmrc
        nvm use $version
    }
  }
  New-Alias -Name cd -Value Change-Node-Version -Force -Option AllScope
  ```

  </details>

- PNPM (es nuestra recomendación por su eficiencia y rapidez)

  ```sh
  npm install -g pnpm
  ```

- o NPM

  ```sh
  npm install npm@latest -g
  ```

### Instalación

1. Clona el repositorio

   ```sh
   git clone https://github.com/midudev/landing-gta-vi.git
   ```

2. Instala los paquetes de NPM

   ```sh
   pnpm install
   ```

3. Ejecuta el proyecto
   ```sh
   pnpm run dev
   ```

<p align="right"><a href="#readme-top">Up</a></p>

## Contribuir al proyecto

Las contribuciones son lo que hacen que la comunidad de código abierto sea un lugar increíble para aprender, inspirar y crear. ¡Cualquier contribución que hagas es **muy apreciada**!

Si tienes alguna sugerencia que podría mejorar el proyecto, por favor haz un [_fork_](https://github.com/midudev/landing-gta-vi/fork) del repositorio y crea una [_pull request_](https://github.com/midudev/landing-gta-vi/pulls). También puedes simplemente abrir un [_issue_](https://github.com/midudev/landing-gta-vi/issues) con la etiqueta "enhancement".

Aquí tienes una guía rápida:

1. Haz un [_fork_](https://github.com/midudev/landing-gta-vi/fork) del Proyecto
2. Clona tu [_fork_](https://github.com/midudev/landing-gta-vi/fork) (`git clone <URL del fork>`)
3. Añade el repositorio original como remoto (`git remote add upstream <URL del repositorio original>`)
4. Crea tu Rama de Funcionalidad (`git switch -c feature/CaracteristicaIncreible`)
5. Realiza tus Cambios (`git commit -m 'Add: alguna CaracterísticaIncreible'`)
6. Haz Push a la Rama (`git push origin feature/CaracteristicaIncreible`)
7. Abre una [_pull request_](https://github.com/midudev/landing-gta-vi/pulls)

Por favor, consulta nuestra [guía de contribución](https://github.com/midudev/landing-gta-vi/blob/master/fork.md) para saber cómo puedes empezar de la mejor manera y siguiendo [buenas prácticas](https://github.com/midudev/landing-gta-vi/blob/main/fork.md#buenas-prácticas-).

### Contribuir desde Stackblitz

Si deseas contribuir en este proyecto, puedes usar StackBlitz

[![Abrir en Stackblitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/midudev/landing-gta-vi)


## 🛠️ Sistemas Utilizados

- [![Astro][astro-badge]][astro-url] - El Framework que se usa en general en la Pagina Web
- [![Tailwind CSS][tailwind-badge]][tailwind-url] - Dependencia que deja atras el uso de CSS


<p align="right"><a href="#readme-top">Up</a></p>

[astro-url]: https://astro.build/
[typescript-url]: https://www.typescriptlang.org/
[tailwind-url]: https://tailwindcss.com/
[animations-url]: https://tailwindcss-animations.vercel.app/
[astro-badge]: https://img.shields.io/badge/Astro-fff?style=for-the-badge&logo=astro&logoColor=bd303a&color=352563
[typescript-badge]: https://img.shields.io/badge/Typescript-007ACC?style=for-the-badge&logo=typescript&logoColor=white&color=blue
[tailwind-badge]: https://img.shields.io/badge/Tailwind-ffffff?style=for-the-badge&logo=tailwindcss&logoColor=38bdf8
[animations-badge]: https://img.shields.io/badge/@midudev/tailwind-animations-ff69b4?style=for-the-badge&logo=node.js&logoColor=white&color=blue
[contributors-shield]: https://img.shields.io/github/contributors/midudev/landing-gta-vi.svg?style=for-the-badge
[contributors-url]: https://github.com/midudev/landing-gta-vi/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/midudev/landing-gta-vi.svg?style=for-the-badge
[forks-url]: https://github.com/midudev/landing-gta-vi/network/members
[stars-shield]: https://img.shields.io/github/stars/midudev/landing-gta-vi.svg?style=for-the-badge
[stars-url]: https://github.com/midudev/landing-gta-vi/stargazers
[issues-shield]: https://img.shields.io/github/issues/midudev/landing-gta-vi.svg?style=for-the-badge
[issues-url]: https://github.com/midudev/landing-gta-vi/issues
