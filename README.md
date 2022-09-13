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
  <a href="https://github.com/AmineSoukara/EgyBest-API">
    <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FAmineSoukara%2FEgyBest-Api&count_bg=%23FF0000&title_bg=%23555555&icon=tinder.svg&icon_color=%23FF0000&title=Hits&edge_flat=false" alt="hits" />
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

##

<div align="center">

# 👨‍💻 Dev & Support:
<a href="https://bio.link/aminesoukara"><img src="https://img.shields.io/badge/@AmineSoukara-000000?style=flat&logo=messenger&logoColor=white?logoWidth=100"></a>
<a href="https://t.me/EgyBestBotSupport"><img src="https://img.shields.io/badge/Group-FF0000?style=flat&logo=telegram&logoColor=white?logoWidth=100"></a>
<a href="https://t.me/EgyBestBotOriginal"><img src="https://img.shields.io/badge/Channel-FF0000?style=flat&logo=telegram&logoColor=white?logoWidth=100"></a>

##

# ⚠️ Note:
- For Personal Use Only, Don't Create Or Build Something Huge With This API Without Permission Otherwise You Will Be Banned
- This Project Is Licensed Under The [GNU General Public License v3.0](https://github.com/AmineSoukara/EgyBest-Api/blob/main/LICENSE)

##

# ⭐️ Features:
<div align="left">

* [x] Smart Search
* [x] Extract Full Info From Url (Movie-Serie/Anime)
* [x] Extract: Story - Image - Title - Trailer - Actors Info - Note - Rating Percent - Quality
* [x] Extract Download and Stream Links With Full Info
* [x] Extract Similar Movies
* [x] Extract Seasons / Episodes
* [x] Extract Previous And Next Episode
* [x] Extract Movies Or Series From Paths
* [x] And More ...

<div align="center">

##

# 🕹 Libraries:
<a href="https://github.com/AmineSoukara/Py-EgyBest-Api"><img src="https://img.shields.io/badge/Python-8000FF?style=flat&logo=github&logoColor=white?logoWidth=100"></a>
<a href="https://github.com/AmineSoukara/Java-EgyBest-Api"><img src="https://img.shields.io/badge/Java-8000FF?style=flat&logo=github&logoColor=white?logoWidth=100"></a>

##

# ❤️ Used By :

<a href="https://t.me/EgyBestXBot"><img src="https://img.shields.io/badge/@EgyBestXBot-FF0000?style=flat&logo=telegram&logoColor=black"></a>
<a href="https://github.com/recloudstream/cloudstream"><img src="https://img.shields.io/badge/CloudStream-FF0000?style=flat&logo=kotlin&logoColor=black"></a>
<a href="https://pypi.org/project/Py-EgyBest-Api/"><img src="https://img.shields.io/badge/PyEgyBestApi-FF0000?style=flat&logo=pypi&logoColor=white?logoWidth=100"></a>

##

# 🪐 Docs / Examples:
<div align="left">

<details>	
  <summary><b> How To Use ?</b></summary>

## 🎰 Mandatory Configs 

* [x] Make Sure You Have All These Mandatory Configs, API Will Not Work Without it
```
API_URL - ACCESS_TOKEN - REFRESH_TOKEN - ID - PASSWORD
```
* [x] You Can Get it From:
<div align="center">
<a href="https://t.me/EgyBestAPIBot"><img src="https://img.shields.io/badge/@EgyBestAPIBot-FFFF00?style=flat&logo=telegram&logoColor=white?logoWidth=100"></a>

<div align="left">

# /dls:

<details>
<summary><b> Extract Download and Stream Links With Full Info</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  v     |  False   | Number | 1-2 Return As list 3-4 As Dict, Default 1 |
|  url   |  True    | String | Episode or Movie link |
### Method:
- GET
### Example:
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
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/dls_v1.json"><img src="https://img.shields.io/badge/Output–V1-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/dls_v2.json"><img src="https://img.shields.io/badge/Output–V2-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/dls_v3.json"><img src="https://img.shields.io/badge/Output–V3-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/dls_v4.json"><img src="https://img.shields.io/badge/Output–V4-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>


# /search:

<details>
<summary><b> Smart Search</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  type     |  False   | String | types: all-serie-movie-anime-show, default: all |
|  query   |  True    | String | title (Show - Movie ...) |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"query": "hulk", "type": "movie"}                      
URL = API +  "/search"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/search.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>

# /seasons:

<details>
<summary><b> Extract Seasons</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | Show/Serie link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/series/the-walking-dead"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL}                      
URL = API +  "/seasons"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_seasons.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>


# /episodes:

<details>
<summary><b> Extract Episodes</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | Season link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/season/the-walking-dead-season-11"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL}                      
URL = API +  "/episodes"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_episodes.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>


# /info:

<details>
<summary><b> Extract Full Info From Url</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | Show / Serie / Movie, link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/movie/top-gun-maverick-2022"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL}                      
URL = API +  "/info"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_info.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>


# /info (separate information)

<details>
<summary><b> Extract Story - Image - Title - Trailer - Actors Info - Note - Rating Percent - Quality</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | Show-Serie or Movie link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/movie/top-gun-maverick-2022"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL}
                
URL_actors = API +  "/actors"
response_actors = requests.get(URL_actors, headers=HEADERS, params=PARAMS)
print(response_actors.json())

URL_note = API +  "/note"
response_note = requests.get(URL_note, headers=HEADERS, params=PARAMS)
print(response_note.json())

URL_trailer = API +  "/trailer"
response_trailer = requests.get(URL_trailer, headers=HEADERS, params=PARAMS)
print(response_trailer.json())

URL_title = API +  "/title"
response_title = requests.get(URL_title, headers=HEADERS, params=PARAMS)
print(response_title.json())

URL_thumbnail = API +  "/thumbnail"
response_thumbnail = requests.get(URL_thumbnail, headers=HEADERS, params=PARAMS)
print(response_thumbnail.json())

URL_story = API +  "/story"
response_story = requests.get(URL_story, headers=HEADERS, params=PARAMS)
print(response_story.json())

URL_rating_percent = API +  "/rating_percent"
response_rating_percent = requests.get(URL_rating_percent, headers=HEADERS, params=PARAMS)
print(response_rating_percent.json())

URL_quality = API +  "/quality"
response_quality = requests.get(URL_quality, headers=HEADERS, params=PARAMS)
print(response_quality.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_actors.json"><img src="https://img.shields.io/badge/Output–Actors-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_trailer.json"><img src="https://img.shields.io/badge/Output–Trailer-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_title.json"><img src="https://img.shields.io/badge/Output–Title-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_thumbnail.json"><img src="https://img.shields.io/badge/Output–Thumbnail-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_story.json"><img src="https://img.shields.io/badge/Output–Story-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_note.json"><img src="https://img.shields.io/badge/Output–Note-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_quality.json"><img src="https://img.shields.io/badge/Output–Quality-01DF01?style=flat&logo=json&logoColor=black"></a>
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_rating_percent.json"><img src="https://img.shields.io/badge/Output–RatingPercent-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>


# /page:

<details>
<summary><b> Extract Data From A Specific Path</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  number |  False   | Number | number of page, default 1 |
|  path   |  True    | String | path eg: movies/top - movies/latest .. |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"path": "movies/latest", "number": 1}                      
URL = API +  "/page"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_page.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>



# /pages:

<details>
<summary><b> Extract Multiple Data From A Specific Path</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  limit |  False   | Number | number of pages, default 1 |
|  path   |  True    | String | path eg: movies/top - movies/latest .. |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"path": "movies/latest", "limit": 3}                      
URL = API +  "/pages"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_pages.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>




# /table:

<details>
<summary><b> Extract Table Info From Page</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | (Show / Episode / Movie ..)  link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/movie/top-gun-maverick-2022"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL, "v": 2}                      
URL = API +  "/table"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_table.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>



# /previous_next:

<details>
<summary><b> Extract Previous And Next Episode</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | Episode link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/episode/westworld-2016-season-4-ep-3"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL, "v": 2}                      
URL = API +  "/previous_next"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_previous_next.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>



# /similar:

<details>
<summary><b> Extract Similar Movies</b></summary>

### Parameters:
|  Name  | Required |  Type  | Description |
|--------|----------|--------|-------------|
|  url   |  True    | String | Movie link |
### Method:
- GET
### Example:
```py
import requests
                 
TOKEN = "abcd123"
API = "http://0.1.2.3"
EGY_URL = "https://www.egybest.org/movie/top-gun-maverick-2022"       
HEADERS = {'Authorization': 'Bearer ' + TOKEN, 'Accept': 'application/json', 'Content-Type': 'application/json'}
PARAMS = {"url": EGY_URL, "v": 2}                      
URL = API +  "/similar"

response = requests.get(URL, headers=HEADERS, params=PARAMS)

print(response.status_code)
print(response.json())
```
<a href="https://github.com/AmineSoukara/EgyBest-Api/blob/main/examples/get_similar_movies.json"><img src="https://img.shields.io/badge/Output-01DF01?style=flat&logo=json&logoColor=black"></a>

</details>



</details>

##

![⭐️](https://telegra.ph/file/b132a131aabe2106bd335.gif)
