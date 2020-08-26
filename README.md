<!--
# Bi-LSTM-CHAR-NER
A fork edit version of https://github.com/Determined22/zh-NER-TF By add Other Features and Char embedding layer on English Corpus 
-->

<!--
*** Thanks for checking out this README Template. If you have a suggestion that would
*** make this better, please fork the repo and create a pull request or simply open
*** an issue with the tag "enhancement".
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

<!--
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
-->


<!-- PROJECT LOGO -->
<br />
<p align="center">
  <!--
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>
  -->
  
  <!--
  <h3 align="center">Best-README-Template</h3>
  -->
  <h3 align="center">Bi-LSTM-CHAR-NER</h3>

  <p align="center">
    <!--An awesome README template to jumpstart your projects!-->
    A fork edit version of https://github.com/Determined22/zh-NER-TF By add Other Features and Char embedding layer on English Corpus 
    <br />
    <!--
    <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a>
    -->
    <br />
    <br />
    <!--
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    -->
    <a href="bilstm-char-test.ipynb">View Demo</a>
    <!--
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
    -->
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  <!--
  * [Prerequisites](#prerequisites)
  -->
  * [Installation](#installation)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)



<!-- ABOUT THE PROJECT -->
## About The Project

<!--
[![Product Name Screen Shot][product-screenshot]](https://example.com)
-->


<!--
There are many great README templates available on GitHub, however, I didn't find one that really suit my needs so I created this enhanced one. I want to create a README template so amazing that it'll be the last one you ever need.

Time Series Forecast is useful in retail analysis in data analysis and mining. When it comes to hts data --- a data format that apply decoposition on massive
data, Many models have built on them. You can have a look at https://otexts.com/fpp2/hts.html
Nowadays, Many R packages have be developed. And you can find Scikit-Hts this python framework to perform similar tasks.
But there are many limits as follows:
* R packages such as gts and Scikit-Hts seems only support uni-feature time series, that you can not add other feature related with time series.
* Scikit-Hts have some Bugs with bottom up situation, which can be seen at https://github.com/carlomazzaferro/scikit-hts/issues/35
* Complex params fine-tuned on Prophet and the above framework (Scikit-Hts) may be difficult.

So, This project can be a Demo to overcome above limits.
And achieve cv mape below 0.08.
-->
NER is a basic task in NLP. 
This a fork edit version of https://github.com/Determined22/zh-NER-TF By add Other Features and Char embedding layer 

This project use dataset download from https://github.com/kamalkraj/BERT-NER data dir.
Because the edit is simple, only release two jupyter notebooks for record.

By add Char embedding layer, The model accuracy improve from average 70% to 80% training from scratch.
 <!--
Here's why:
* Your time should be focused on creating something amazing. A project that solves a problem and helps others
* You shouldn't be doing the same tasks over and over like creating a README from scratch
* You should element DRY principles to the rest of your life :smile:

Of course, no one template will serve all projects since your needs may be different. So I'll be adding more in the near future. You may also suggest changes by forking this repo and creating a pull request or opening an issue.

A list of commonly used resources that I find helpful are listed in the acknowledgements.
-->
### Built With
<!--
This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.
* [Bootstrap](https://getbootstrap.com)
* [JQuery](https://jquery.com)
* [Laravel](https://laravel.com)
-->
* [TensorFlow 1](https://github.com/tensorflow/tensorflow)


<!-- GETTING STARTED -->
## Getting Started
<!--
This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.
-->

<!--
### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
```sh
npm install npm@latest -g
```
-->

### Installation
<!--
* pip
```sh
pip3 install -r requirements.txt
```
-->
Install TensorFlow 1 and requirements according to https://github.com/Determined22/zh-NER-TF

<!--
1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
```sh
git clone https://github.com/your_username_/Project-Name.git
```
3. Install NPM packages
```sh
npm install
```
4. Enter your API in `config.js`
```JS
const API_KEY = 'ENTER YOUR API';
```
-->


<!-- USAGE EXAMPLES -->
## Usage
<!--
Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_
-->
1. Download Data from https://github.com/kamalkraj/BERT-NER/tree/dev/data
<!--
```sh
bash download.sh
```
-->

2. Generate features like follows
<!--
```sh
python3 script/feature-construct.py
python3 script/agg_feature_construct.py
```
-->
<p>
-DOCSTART- -X- -X- O
</p>
&nbsp;

<p>
EU NNP B-NP B-ORG

rejects VBZ B-VP O

German JJ B-NP B-MISC

call NN I-NP O

to TO B-VP O

boycott VB I-VP O

British JJ B-NP B-MISC

lamb NN I-NP O

. . O O
</p>
&nbsp;

<p>
Peter NNP B-NP B-PER

Blackburn NNP I-NP I-PER
</p>
&nbsp;

BRUSSELS NNP B-NP B-LOC

1996-08-22 CD I-NP O
</p>
&nbsp;

<p>
<a href="bilstm-char-train.ipynb">1. Data Process and Network Train</a>
</p>

<p>
<a href="bilstm-char-test.ipynb">2. Model Validation and conclusion decode</a>
</p>

<!--
3. Params search by Hyperopt
```sh
python3 script/hts-params-explore.py
```
4. Run Demo
```sh
python3 script/run-best-hts.py
```
-->

<!-- ROADMAP -->
## Roadmap
<!--
See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a list of proposed features (and known issues).

<p>
<a href="notebooks/time-series-explore.ipynb">Time Series Data Analysis Notebook</a>
</p>
You can also step by step run Jupyter Notebooks in /notebooks dir.
-->
<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

<!--
Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com
-->
svjack - svjackbt@gmail.com

<!--
Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)
-->
Project Link: [https://github.com/svjack/Bi-LSTM-CHAR-NER](https://github.com/svjack/Bi-LSTM-CHAR-NER)


<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
<!--
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)
* [Animate.css](https://daneden.github.io/animate.css)
* [Loaders.css](https://connoratherton.com/loaders)
* [Slick Carousel](https://kenwheeler.github.io/slick)
* [Smooth Scroll](https://github.com/cferdinandi/smooth-scroll)
* [Sticky Kit](http://leafo.net/sticky-kit)
* [JVectorMap](http://jvectormap.com)
* [Font Awesome](https://fontawesome.com)
-->




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=flat-square
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=flat-square
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=flat-square
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=flat-square
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=flat-square
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png

