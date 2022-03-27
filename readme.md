<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



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



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/NelisV/fs-scenery-project">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">FS Scenery Map Project</h3>

  <p align="center">
    A community driven project to map flight simulation scenery. 
    <br />
    <a href="https://github.com/NelisV/fs-scenery-project"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/NelisV/fs-scenery-project">View Demo</a>
    ·
    <a href="https://github.com/NelisV/fs-scenery-project/issues">Report Bug</a>
    ·
    <a href="https://github.com/NelisV/fs-scenery-project/issues">Request Feature</a>
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
    <li><a href="#dataset">DataSet</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

Welcome to the FS Scenery Map Project, an open source mapping project to track flight simulation scenery. Anyone is invited to contribute to this datasource, add-on developers/publishers included. As long as a contribution can be backed with a public announcement it will generally be accepted.

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

* [GeoJSON](https://datatracker.ietf.org/doc/html/rfc7946)
* [QGIS](https://qgis.org)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- DATASET -->
## DataSet
A product supporting multiple simulators should have separate entries for each simulator.
### airports.geojson
GeoJSON file containing 'airport scenery' products as Point geometry.<br>
When adding new airports, use the coordinates from the [OurAirports repository](https://github.com/davidmegginson/ourairports-data).
#### Properties
- Product title `title`
- Product status `status` - announced/released
- ICAO code `icao`
- Developer `developer`
- Publisher `publisher`
- Release date `release` - ISO 8601 datetime in UTC
- Last updated on `update` - ISO 8601 datetime in UTC
- Tested simulator version `sim` - example: `xplane_11.53`, `prepar3d_5.3.17.28160`, `msfs_1.23.12.0`
- Product link `url`
- Product description `desc_txt` - max 128 characters utf-8
- Tags `tags` - string containing comma separated list. example: `'GSX, freeware, SODE'` 

### scenery.geojson
GeoJSON file containing 'region scenery' products covering a certain geographic area as Polygon geometry.
#### Properties
- Product title `title`
- Product status `status` - announced/released
- Developer `developer`
- Publisher `publisher`
- Release date `release` - ISO 8601 datetime in UTC
- Last updated on `update` - ISO 8601 datetime in UTC
- Tested simulator version `sim` - example: `xplane_11.53`, `prepar3d_5.3.17.28160`, `msfs_1.23.12.0`
- Product link `url`
- Product description `desc_txt` - max 128 characters utf-8
- Tags `tags` - string containing comma separated list

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [ ] Start the project
    - [x] Git repo
    - [x] License
    - [ ] Readme
- [ ] Define data structure
- [ ] Start dataset
    - [ ] Open up to community contributors

See the [open issues](https://github.com/NelisV/fs-scenery-project/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

The easiest way to edit this data and contribute is using QGIS, an open source GIS toolkit. Make sure to only push valid GeoJSON.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Open the relevant file in QGIS
4. Make your changes
5. Validate your changes
6. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
7. Push to the branch (`git push origin feature/AmazingFeature`)
8. Open a pull request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the GPL-3.0 License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

[NelisV](https://github.com/NelisV)

Project link: [https://github.com/NelisV/fs-scenery-project](https://github.com/NelisV/fs-scenery-project)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [OurAirports](https://github.com/davidmegginson/ourairports-data)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/NelisV/fs-scenery-project.svg?style=for-the-badge
[contributors-url]: https://github.com/NelisV/fs-scenery-project/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/NelisV/fs-scenery-project.svg?style=for-the-badge
[forks-url]: https://github.com/NelisV/fs-scenery-project/network/members
[stars-shield]: https://img.shields.io/github/stars/NelisV/fs-scenery-project.svg?style=for-the-badge
[stars-url]: https://github.com/NelisV/fs-scenery-project/stargazers
[issues-shield]: https://img.shields.io/github/issues/NelisV/fs-scenery-project.svg?style=for-the-badge
[issues-url]: https://github.com/NelisV/fs-scenery-project/issues
[license-shield]: https://img.shields.io/github/license/NelisV/fs-scenery-project.svg?style=for-the-badge
[license-url]: https://github.com/NelisV/fs-scenery-project/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png