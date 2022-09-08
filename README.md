![RUN](https://github.com/AmineSoukara/EgyBest-Api/raw/main/api/static/rae.gif)

<div align="center">

> Unofficial EgyBest API.

<!-- Badges -->
<p>
  <a href="https://github.com/AmineSoukara/EgyBest-Api/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/aminesoukara/EgyBest-Api" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/aminesoukara/EgyBest-Api" alt="last update" />
  </a>
  <a href="https://github.com/AmineSoukara/EgyBest-Api/network/members">
    <img src="https://img.shields.io/github/forks/aminesoukara/EgyBest-Api" alt="forks" />
  </a>
  <a href="https://github.com/AmineSoukara/EgyBest-Api/stargazers">
    <img src="https://img.shields.io/github/stars/aminesoukara/EgyBest-Api" alt="stars" />
  </a>
  <a href="https://github.com/AmineSoukara/EgyBest-Api/issues/">
    <img src="https://img.shields.io/github/issues/aminesoukara/EgyBest-Api" alt="open issues" />
  </a>
  <a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/aminesoukara/EgyBest-Api.svg" alt="license" />
  </a>
</p>

<h4>
    <a href="https://www.egybest-api.ga/docs/api/">Docs</a>
  <span> · </span>
    <a href="https://github.com/AmineSoukara/EgyBest-Api/issues/">Report Bug</a>
  <span> · </span>
    <a href="https://github.com/AmineSoukara/EgyBest-Api/issues/">Request Feature</a>
  </h4>
</div>

<br />

<div align="center">


# 👨‍💻 Developer:
<a href="https://bio.link/aminesoukara"><img src="https://img.shields.io/badge/@AmineSoukara-000000?style=flat&logo=messenger&logoColor=white?logoWidth=100"></a>

# 💬 Support:
<a href="https://t.me/EgyBestBotSupport"><img src="https://img.shields.io/badge/Group-FF0000?style=flat&logo=telegram&logoColor=white?logoWidth=100"></a>
<a href="https://t.me/EgyBestBotOriginal"><img src="https://img.shields.io/badge/Channel-FF0000?style=flat&logo=telegram&logoColor=white?logoWidth=100"></a>

# 🕹 Libraries:
<a href="https://github.com/AmineSoukara/Py-EgyBest-Api"><img src="https://img.shields.io/badge/Python-8000FF?style=flat&logo=github&logoColor=white?logoWidth=100"></a>
<a href="https://github.com/AmineSoukara/Java-EgyBest-Api"><img src="https://img.shields.io/badge/Java-8000FF?style=flat&logo=github&logoColor=white?logoWidth=100"></a>


# 📝 License:
This Project Is Licensed Under The [GNU General Public License v3.0](https://github.com/AmineSoukara/EgyBest-Api/blob/main/LICENSE)

# ⚠️ Note:
- For Personal Use Only, Don't Create Or Build Something Huge With This API Without Permission Otherwise You Will Be Banned

# ⭐️ Features:
<div align="left">

* [x] Smart Search
* [x] Extract Full Info From Url (Movie-Serie/Anime)
* [x] Extract: Story - Image - Title - Trailer - Actors Info - Note
* [x] Extract Download and Stream Links With Full Info
* [x] Extract Similar Movies
* [x] Extract Seasons / Episodes
* [x] Extract Previous And Next Episode
* [x] Extract Movies Or Series From Paths

<div align="center">

# 🪐 Docs / Examples:
<div align="left">

<details>	
  <summary><b> How To Use ?</b></summary>

## ● Mandatory Configs 
```
[+] Make Sure You Get All These Mandatory Configs:
    [-] API_URL - ACCESS_TOKEN - REFRESH_TOKEN - ID - PASSWORD
    [-] You Can Get it From https://t.me/EgyBestAPIBot
[+] API Will Not Work Without it.
```

## /dls:
• Extract Download and Stream Links With Full Info
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
MOVIE_URL = "https://www.egybest.org/movie/top-gun-maverick-2022"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": MOVIE_URL, "v": 2}                      
URL = API +  "/dls"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/dls_v2.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>


</details>
