:abc: English | [:mahjong: 简体中文](https://github.com/my8100/scrapydweb/blob/master/README_CN.md)

# ScrapydWeb: A full-featured web UI for Scrapyd cluster management, with Scrapy log analysis & visualization supported.

[![PyPI - scrapydweb Version](https://img.shields.io/pypi/v/scrapydweb.svg)](https://pypi.org/project/scrapydweb/)
[![Downloads - total](https://pepy.tech/badge/scrapydweb)](https://pepy.tech/project/scrapydweb)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/scrapydweb.svg)](https://pypi.org/project/scrapydweb/)
[![Coverage Status](https://coveralls.io/repos/github/my8100/scrapydweb/badge.svg?branch=master)](https://coveralls.io/github/my8100/scrapydweb?branch=master)
[![GitHub license](https://img.shields.io/github/license/my8100/scrapydweb.svg)](https://github.com/my8100/scrapydweb/blob/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/url/https/github.com/my8100/scrapydweb.svg?style=social)](https://twitter.com/intent/tweet?text=@my8100_%20ScrapydWeb:%20A%20full-featured%20web%20UI%20for%20Scrapyd%20cluster%20management,%20with%20Scrapy%20log%20analysis%20%26%20visualization%20supported.%20%23python%20%23scrapy%20%23scrapyd%20%23webscraping%20%23scrapydweb%20&url=https%3A%2F%2Fgithub.com%2Fmy8100%2Fscrapydweb)


##
![overview](https://raw.githubusercontent.com/my8100/scrapydweb/master/screenshots/overview.png)

## Scrapyd :x: ScrapydWeb :x: LogParser
### :book: Recommended Reading
[:link: How to efficiently manage your distributed web scraping projects](https://medium.com/@my8100/https-medium-com-my8100-how-to-efficiently-manage-your-distributed-web-scraping-projects-55ab13309820)


## :star: Features
<details>
<summary>View contents</summary>

- :diamond_shape_with_a_dot_inside: Scrapyd Cluster Management
  - :100: All Scrapyd JSON API Supported
  - :ballot_box_with_check: Group, filter and select any number of nodes
  - :computer_mouse: **Execute command on multinodes with just a few clicks**

- :mag: Scrapy Log Analysis
  - :bar_chart: Stats collection
  - :chart_with_upwards_trend: **Progress visualization**
  - :bookmark_tabs: Logs categorization

- :battery: Enhancements
  - :package: **Auto eggify your projects**
  - :male_detective: **Integrated with [:link: *LogParser*](https://github.com/my8100/logparser)**
  - :e-mail: **Email notice**
  - :iphone: Mobile UI
  - :closed_lock_with_key: Basic auth for web UI

</details>


## :eyes: Preview
- [:framed_picture: Screenshots](https://github.com/my8100/files/tree/master/scrapydweb/README.md)

- [:film_strip: Gif Demo](https://github.com/my8100/files/tree/master/scrapydweb/README_GIF.md)


## :computer: Getting Started
<details>
<summary>View contents</summary>

### :warning: Prerequisites
:heavy_exclamation_mark: **Make sure that [:link: Scrapyd](https://github.com/scrapy/scrapyd) has been installed and started on all of your hosts.**

:bangbang: Note that for remote access, you have to manually set 'bind_address = 0.0.0.0' in [:link: the configuration file of Scrapyd](https://scrapyd.readthedocs.io/en/latest/config.html#example-configuration-file)
and restart Scrapyd to make it visible externally.

### :arrow_down: Install
- Use pip:
```bash
pip install scrapydweb
```

- Use git:
```bash
git clone https://github.com/my8100/scrapydweb.git
cd scrapydweb
python setup.py install
```

### :arrow_forward: Start
1. Start ScrapydWeb via command `scrapydweb`. (a config file would be generated for customizing settings at the first startup.)
2. Visit http://127.0.0.1:5000 **(It's recommended to use Google Chrome for a better experience.)**

### :globe_with_meridians: Browser Support
The latest version of Google Chrome, Firefox, and Safari.

</details>


## :heavy_check_mark: Running the tests
<details>
<summary>View contents</summary>

<br>

```bash
$ git clone https://github.com/my8100/scrapydweb.git
$ cd scrapydweb

# To create isolated Python environments
$ pip install virtualenv
$ virtualenv venv/scrapydweb
# Or specify your Python interpreter: $ virtualenv -p /usr/local/bin/python3.7 venv/scrapydweb
$ source venv/scrapydweb/bin/activate

# Install dependent libraries
(scrapydweb) $ python setup.py install
(scrapydweb) $ pip install pytest
(scrapydweb) $ pip install coverage

# Make sure Scrapyd has been installed and started, then update the custom_settings item in tests/conftest.py
(scrapydweb) $ vi tests/conftest.py
(scrapydweb) $ curl http://127.0.0.1:6800

(scrapydweb) $ coverage run --source=scrapydweb -m pytest tests/test_a_factory.py -s -vv
(scrapydweb) $ coverage run --source=scrapydweb -m pytest tests -s -vv
(scrapydweb) $ coverage report
# To create an HTML report, check out htmlcov/index.html
(scrapydweb) $ coverage html
```

</details>


## :building_construction: Built With
<details>
<summary>View contents</summary>

<br>

- Front End
  - [:link: jQuery](https://github.com/jquery/jquery)
  - [:link: Vue.js](https://github.com/vuejs/vue)
  - [:link: Element](https://github.com/ElemeFE/element)
  - [:link: ECharts](https://github.com/apache/incubator-echarts)
- Back End
  - [:link: Flask](https://github.com/pallets/flask)
  - [:link: Flask-Compress](https://pypi.org/project/Flask-Compress/)
  - [:link: Requests](https://github.com/requests/requests)

</details>


## :clipboard: Changelog
Detailed changes for each release are documented in the [:link: HISTORY.md](https://github.com/my8100/scrapydweb/blob/master/HISTORY.md).


## :man_technologist: Author
| [<img src="https://github.com/my8100.png" width="100px;"/>](https://github.com/my8100)<br/> [<sub>my8100</sub>](https://github.com/my8100) |
| --- |


## :busts_in_silhouette: Contributors
| [<img src="https://github.com/simplety.png" width="100px;"/>](https://github.com/simplety)<br/> [<sub>Kaisla</sub>](https://github.com/simplety) |
| --- |


## :copyright: License
This project is licensed under the GNU General Public License v3.0 - see the [:link: LICENSE](https://github.com/my8100/scrapydweb/blob/master/LICENSE) file for details.
