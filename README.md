# getip [![GitHub](https://img.shields.io/github/license/mahdymirzade/getip)](./LICENSE.md)
📱 Get Private/Public IP &amp; IP's Geolocation.

## Installation
getip can be installed manually or using AUR.

### AUR [![AUR version](https://img.shields.io/aur/version/getip)](https://aur.archlinux.org/packages/getip) [![AUR votes](https://img.shields.io/aur/votes/getip)](https://aur.archlinux.org/packages/getip)
You can install [getip](https://aur.archlinux.org/packages/getip) with ArchLinux User Repository.

**AUR Helper:**
```bash
$ yay -S getip
```
**Without Helpers:**
```bash
$ git clone https://aur.archlinux.org/getip.git
$ cd getip
$ makepkg -si
```

### Manual Installation ![GitHub repo size](https://img.shields.io/github/repo-size/mahdymirzade/getip)
```bash
$ git clone https://github.com/MahdyMirzade/getip.git
$ cp getip/getip /usr/bin
$ getip v
```
> You may need to run some of these commands with root permissions. (sudo)

## Usage

[![getip usage gif](https://raw.githubusercontent.com/MahdyMirzade/MahdyMirzade/main/assets/getip/usage.gif)](https://asciinema.org/a/427949)

## Methods

**Table of methods:**

| Method | Description |
| --- | --- |
| help (h) | Show getip's help manual |
| version (v) | Show getip's version number |
| public (pub) | Show your public IP address |
| private (priv) | Show your private IP address |
| json (j) | Show you public IP's full information in Json |

**Sample output of each method:**

<details>
<summary><code>$ getip h</code></summary>
    
<div class="language-bash highlighter-rouge"><div class="highlight"><pre class="highlight"><code>Usage: /usr/bin/getip [METHOD]

General Methods:
    h,  help            Show this manual
    v,  version         Show version number

IP Information Methods:
    pub,    public      Get Your Public IP Address
    priv,   private     Get Your Private IP Address
    j,      json        Get Your Public IP's Full Information in Json

Other methods can be also grabbed from json output,
    for example this is your json output:
    {
        ...
        "continent": "Europe",
        "country": "Germany",
        "region": "Bavaria",
        "city": "Nuremberg",
        "latitude": 49.4254092,
        "longitude": 11.0796553,
        ...
    }
    and if you want to get IP's country:
    $ /usr/bin/getip country
    Output: Germany

Full info: https://mahdymirzade.github.io/getip
</code></pre></div></div>

</details>

<details>
<summary><code>$ getip v</code></summary>
    
<div class="language-bash highlighter-rouge"><div class="highlight"><pre class="highlight"><code>       _
  __ _(_)_ __       getip (Geolocation, Private/Public IP) v1.0.1
 / _` | | '_ \      Copyright (C) 2021 Mahdy Mirzade
| (_| | | |_) |
 \__, |_| .__/      This program may be freely redistributed under
 |___/  |_|         the terms of the GNU General Public License.

</code></pre></div></div>

</details>

<details>
<summary><code>$ getip pub</code></summary>
    
<div class="language-bash highlighter-rouge"><div class="highlight"><pre class="highlight"><code>49.**.**.55</code></pre></div></div>

</details>

<details>
<summary><code>$ getip priv</code></summary>
    
<div class="language-bash highlighter-rouge"><div class="highlight"><pre class="highlight"><code>192.168.43.163</code></pre></div></div>

</details>


<details>
<summary><code>$ getip j</code></summary>
    
<div class="language-bash highlighter-rouge"><div class="highlight"><pre class="highlight"><code>{
  "ip": "49.**.**.55",
  "success": true,
  "type": "IPv4",
  "continent": "Europe",
  "continent_code": "EU",
  "country": "Germany",
  "country_code": "DE",
  "country_flag": "https://cdn.ipwhois.io/flags/de.svg",
  "country_capital": "Berlin",
  "country_phone": "+49",
  "country_neighbours": "CH,PL,NL,DK,BE,CZ,LU,FR,AT",
  "region": "Bavaria",
  "city": "Gunzenhausen",
  "latitude": 123,
  "longitude": 456,
  "asn": "AS24940",
  "org": "Hetzner Online GmbH",
  "isp": "Hetzner Online GmbH",
  "timezone": "Europe/Berlin",
  "timezone_name": "Central European Standard Time",
  "timezone_dstOffset": 0,
  "timezone_gmtOffset": 3600,
  "timezone_gmt": "GMT +1:00",
  "currency": "Euro",
  "currency_code": "EUR",
  "currency_symbol": "€",
  "currency_rates": 0.841,
  "currency_plural": "euros",
  "completed_requests": 157
}
</code></pre></div></div>

</details>
  
