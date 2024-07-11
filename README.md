## About
Unofficial API of [Hamster Kombat](https://t.me/Hamster_kombat_bot/start?startapp=kentId101554083) telegram game to get daily cards and Morse and ...

## Usage
This fixed address contains the required data that you can read and use in your code:

[https://nabikaz.github.io/HamsterKombat-API/config.json](https://nabikaz.github.io/HamsterKombat-API/config.json)

## Sample codes

python:
```python
import requests

url = "https://nabikaz.github.io/HamsterKombat-API/config.json"
response = requests.get(url)
data = response.json()

print(data)
```

nodejs:
```js
import fetch from 'node-fetch';

const url = 'https://nabikaz.github.io/HamsterKombat-API/config.json';

fetch(url)
    .then(response => response.json())
    .then(data => {
        console.log(data);
    })
    .catch(error => {
        console.error('Error:', error);
    });
```

php:
```php
<?php
$url = 'https://nabikaz.github.io/HamsterKombat-API/config.json';
$json = file_get_contents($url);
$data = json_decode($json, true);

print_r($data);
```

go:
```go
package main

import (
	"encoding/json"
	"fmt"
	"io/ioutil"
	"net/http"
)

func main() {
	url := "https://nabikaz.github.io/HamsterKombat-API/config.json"

	resp, err := http.Get(url)
	if err != nil {
		fmt.Println("Error:", err)
		return
	}
	defer resp.Body.Close()

	body, err := ioutil.ReadAll(resp.Body)
	if err != nil {
		fmt.Println("Error:", err)
		return
	}

	var data map[string]interface{}
	json.Unmarshal(body, &data)

	fmt.Println(data)
}
```

## How it works
This is a collaborative work of a group of friends who periodically record the required data on this project.

## Participation
If you want to participate in updating the file, contact @NabiKAZ on Telegram or Twitter.

## Supporter
Nothing! Just give a star on the GitHub page, we will be happy. (:

## Donation
If this project was useful for you and you are willing, you can make me happy by giving a Star at the top of this GitHub page. Also this is my wallet address for Donate: \
USDT (TRC20): `TEHjxGqu5Y2ExKBWzArBJEmrtzz3mgV5Hb`
