<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/CurtainShow/API-MyGES">
    <img src="https://media.cdnandroid.com/item_images/1201622/imagen-myges-0ori.jpg" alt="Logo">
  </a>

<h3 align="center"> MyGES API with Python </h3>

  <p align="center">
    <a href="https://github.com/CurtainShow/API-MyGES"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/CurtainShow/API-MyGES">View Demo</a>
    ·
    <a href="https://github.com/CurtainShow/API-MyGES/issues">Report Bug</a>
    ·
    <a href="https://github.com/CurtainShow/API-MyGES/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

### Built With
<div align="center">
  <img src="https://logos-world.net/wp-content/uploads/2021/10/Python-Emblem.png" alt="Logo" width="370" height="220" >
</div>


<p align="right">(<a href="#about-the-project">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

Prerequisites list of things you need to use the software and how to install them.

* PyEnv
  ```sh
  pip install pyenv
  ```

* Python 3.9.5 (or greater)
  ```sh
  pyenv virtualenv 3.9.5 NAME-ENV
  ```

* Activate your Virtual Env
  ```sh
  pyenv activate NAME-ENV
  ```
  
* MyGES (for the reporting file)
  ```sh
  pip install MyGES
  ```
  <p align="right">(<a href="#about-the-project">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

  ```python
  from MyGES import MyGesClient

  # Create your access to MyGES Client
  client = MyGesClient(name='YOUR-ID', password='YOUR-PASSWORD')

  # Access to your Informations
  userInformations = client.getProfile()

  # Access to your agenda, using date for start and end with the format DD/MM/YY
  userAgenda = client.getAgenda('DD/MM/YY', 'DD/MM/YY')

  # Access to your agenda for the next month
  userAgendaForTheNextMonth = client.getAgendaForTheNextMonth()

  # Access to your grades for the actual year
  userGrades = client.getGrades()

  # Access to your absence for the actual year
  client.getAbsences()

  # Access to your list of projects for the actual year
  client.getProjects()

  # Access to your teachers informations (name, mail, etc...)
  client.getTeachers()
  
  
  ```

<p align="right">(<a href="#about-the-project">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Create the connexion to the API
- [x] Create private functions for human understanding
- [x] Create main functions : login, getProfile, getAgenda, getAgendaForTheNextMonth, getGrades, getAbsences, getProjects, getTeachers
- [ ] Create a special function to retrieve only your projects 

See the [open issues](https://github.com/CurtainShow/API-MyGES/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#about-the-project">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#about-the-project">back to top</a>)</p>



<!-- CONTACT -->
## Contact

- Allan BARBOT - [@Veekah](https://github.com/CurtainShow)

Project Link: [https://github.com/CurtainShow/API-MyGES](https://github.com/CurtainShow/API-MyGES)

<p align="right">(<a href="#about-the-project">back to top</a>)</p>


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Python - Documentation](https://devdocs.io/python~3.11/)
* [MyGES - Website](https://www.myges.fr/#/)

<p align="right">(<a href="#about-the-project">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/CurtainShow/API-MyGES.svg?style=for-the-badge
[contributors-url]: https://github.com/CurtainShow/API-MyGES/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/CurtainShow/API-MyGES.svg?style=for-the-badge
[forks-url]: https://github.com/CurtainShow/API-MyGES/network/members
[stars-shield]: https://img.shields.io/github/stars/CurtainShow/API-MyGES.svg?style=for-the-badge
[stars-url]: https://github.com/CurtainShow/API-MyGES/stargazers
[issues-shield]: https://img.shields.io/github/issues/CurtainShow/API-MyGES.svg?style=for-the-badge
[issues-url]: https://github.com/CurtainShow/API-MyGES/issues
[license-shield]: https://img.shields.io/github/license/CurtainShow/API-MyGES.svg?style=for-the-badge
[license-url]: https://mit-license.org/
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/allan-barbot-57a0a2164/
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
