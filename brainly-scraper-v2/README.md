![brainly-scraper-languages](https://socialify.git.ci/hansputera/brainly-scraper-languages/image?description=1&font=Raleway&forks=1&issues=1&language=1&owner=1&pulls=1&stargazers=1&theme=Light)

This library retrieves data from Brainly that has been designed to avoid `403 Forbidden` exception.

> To avoid such errors, you can fill in a valid country code. You can test the 10 languages or country codes available to see if your server hosting country location or location is rejected.

See https://github.com/hansputera/brainly-scraper-languages/blob/master/AVAILABLE_LANGUAGES.md

# 馃拤 Installation
- Using NPM : `npm install brainly-scraper-v2`
- Using YARN : `yarn add brainly-scraper-v2`

# 馃摐 How to use
> WARNING:  Make sure the country code you entered in the constructor is correct.

- Code

```js
const { Brainly } = require("brainly-scraper-v2");
const brain = new Brainly("id"); // 'id' - Default to 'id'

// New Method 'searchWithMT' in (v2.0.8) (You don't need to enter country code in the constructor.)
brain.searchWithMT("es", "Pythagoras").then(console.log).catch(console.error);
// Also, you can use old method (<=v2.0.8) (You need to enter correctly country code in the constructor).
brain.search('es', "Pythagoras").then(console.log).catch(console.error);
```

- Output

```json
[
    {
        "question": {
            "id": 5070014,
            "content": "Pythagoras naci贸 en el a帽o 580 a.c  y muri贸 en el a帽o 501. 驴Que edad tenia Pythagoras C煤ando muri贸?",
            "attachments": [],
            "author": {
                "id": 3467036,
                "avatar_url": "https://es-static.z-dn.net/files/d9d/8f696cce4d637d278ba011b6159642b8.jpg",
                "deleted": false,
                "url": "https://brainly.lat/app/profile/3467036",
                "rank": "Aspirante",
                "username": "BeeluuCabj"
            }
        },
        "answers": [
            {
                "content": "Como naci贸 y muri贸 a.c.... \n" +
          "-501-(-580) -- -501+580= 79... Edad que ten铆a cuando muri贸.",
                "attachments": [],
                "rates": 4,
                "rating": 3.75
            }
        ]
    }, { ... }
]
```

# 鈿欙笍 Issues and Bugs
If you have problems using this library, you can create an issue in the [github repository](https://github.com/hansputera/brainly-scraper-languages). Remember, don't forget to read the instructions and try.

# 馃敩 Hosting testing
## Replit.com
Free and paid hosting replit already tested. The country codes that pass are Indonesia, Spain, India, Portuguese, and Philipines.


Ever tried and tested on other hosting? Please send us your feedback in PR. That would be very helpful 馃槉.

# 鉁嶏笍 Contributions
Do you want to contribute with this library for the better? Very well, fork this [github repository](https://github.com/hansputera/brainly-scraper-languages) then install dependencies to your directory. Happy coding 馃榿
