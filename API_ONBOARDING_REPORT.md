Universidad del Valle de Guatemala
Sistemas y Tecnologías Web
Esteban Montenegro - 241262


# API Onboarding Report
## API Summary
- Name: Cat Facts
- Base URL: https://catfact.ninja
- Authentication: None


## Endpoints Table
| Method |      URL      |  Query Params  | Headers | Expected Status | Obtained Status |
|________|_______________|________________|_________|_________________|_________________|
| GET    | /facts        | none           | none    | 200             | 200             |
| GET    | /facts/id     | none           | none    | 200             | 404             |
| GET    | /facts        | limit=5        | none    | 200             | 200             |
| GET    | /breeds       | none           | none    | 200             | 200             |
| GET    | /fakeendpoint | none           | none    | 404             | 404             |
| GET    | /facts        | limit=abc      | none    | 400             | 404             |


## Evidence
### Successful Response 1
{
    "current_page": 1,
    "data": [
        {
            "fact": "Unlike dogs, cats do not have a sweet tooth. Scientists believe this is due to a mutation in a key taste receptor.",
            "length": 114
        },
        {
            "fact": "When a cat chases its prey, it keeps its head level. Dogs and humans bob their heads up and down.",
            "length": 97
        },
        {
            "fact": "The technical term for a cat’s hairball is a “bezoar.”",
            "length": 54
        },
        {
            "fact": "A group of cats is called a “clowder.”",
            "length": 38
        },
        {
            "fact": "A cat can’t climb head first down a tree because every claw on a cat’s paw points the same way. To get down from a tree, a cat must back down.",
            "length": 142
        }
    ],
    "first_page_url": "https://catfact.ninja/facts?page=1",
    "from": 1,
    "last_page": 67,
    "last_page_url": "https://catfact.ninja/facts?page=67",
    "links": [
        {
            "url": null,
            "label": "Previous",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=1",
            "label": "1",
            "active": true
        },
        {
            "url": "https://catfact.ninja/facts?page=2",
            "label": "2",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=3",
            "label": "3",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=4",
            "label": "4",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=5",
            "label": "5",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=6",
            "label": "6",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=7",
            "label": "7",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=8",
            "label": "8",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=9",
            "label": "9",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=10",
            "label": "10",
            "active": false
        },
        {
            "url": null,
            "label": "...",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=66",
            "label": "66",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=67",
            "label": "67",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=2",
            "label": "Next",
            "active": false
        }
    ],
    "next_page_url": "https://catfact.ninja/facts?page=2",
    "path": "https://catfact.ninja/facts",
    "per_page": 5,
    "prev_page_url": null,
    "to": 5,
    "total": 332
}


### Successful Response 2
{
    "current_page": 1,
    "data": [
        {
            "fact": "Cats have 3 eyelids.",
            "length": 20
        },
        {
            "fact": "Cats walk on their toes.",
            "length": 24
        },
        {
            "fact": "Most cats adore sardines.",
            "length": 25
        }
    ],
    "first_page_url": "https://catfact.ninja/facts?page=1",
    "from": 1,
    "last_page": 11,
    "last_page_url": "https://catfact.ninja/facts?page=11",
    "links": [
        {
            "url": null,
            "label": "Previous",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=1",
            "label": "1",
            "active": true
        },
        {
            "url": "https://catfact.ninja/facts?page=2",
            "label": "2",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=3",
            "label": "3",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=4",
            "label": "4",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=5",
            "label": "5",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=6",
            "label": "6",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=7",
            "label": "7",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=8",
            "label": "8",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=9",
            "label": "9",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=10",
            "label": "10",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=11",
            "label": "11",
            "active": false
        },
        {
            "url": "https://catfact.ninja/facts?page=2",
            "label": "Next",
            "active": false
        }
    ],
    "next_page_url": "https://catfact.ninja/facts?page=2",
    "path": "https://catfact.ninja/facts",
    "per_page": 3,
    "prev_page_url": null,
    "to": 3,
    "total": 33
}


### Successful Response 3
{
    "current_page": 1,
    "data": [
        {
            "breed": "Abyssinian",
            "country": "Ethiopia",
            "origin": "Natural/Standard",
            "coat": "Short",
            "pattern": "Ticked"
        },
        {
            "breed": "Aegean",
            "country": "Greece",
            "origin": "Natural/Standard",
            "coat": "Semi-long",
            "pattern": "Bi- or tri-colored"
        },
        {
            "breed": "American Curl",
            "country": "United States",
            "origin": "Mutation",
            "coat": "Short/Long",
            "pattern": "All"
        },
        {
            "breed": "American Bobtail",
            "country": "United States",
            "origin": "Mutation",
            "coat": "Short/Long",
            "pattern": "All"
        },
        {
            "breed": "American Shorthair",
            "country": "United States",
            "origin": "Natural",
            "coat": "Short",
            "pattern": "All but colorpoint"
        },
        {
            "breed": "American Wirehair",
            "country": "United States",
            "origin": "Mutation",
            "coat": "Rex",
            "pattern": "All but colorpoint"
        },
        {
            "breed": "Arabian Mau",
            "country": "Arabian Peninsula",
            "origin": "Natural",
            "coat": "Short",
            "pattern": ""
        },
        {
            "breed": "Australian Mist",
            "country": "Australia",
            "origin": "Crossbreed",
            "coat": "Short",
            "pattern": "Spotted and Classic tabby"
        },
        {
            "breed": "Asian",
            "country": "developed in the United Kingdom (founding stock from Asia)",
            "origin": "",
            "coat": "Short",
            "pattern": "Evenly solid"
        },
        {
            "breed": "Asian Semi-longhair",
            "country": "United Kingdom",
            "origin": "Crossbreed",
            "coat": "Semi-long",
            "pattern": "Solid"
        },
        {
            "breed": "Balinese",
            "country": "developed in the United States (founding stock from Thailand)",
            "origin": "Crossbreed",
            "coat": "Long",
            "pattern": "Colorpoint"
        },
        {
            "breed": "Bambino",
            "country": "United States",
            "origin": "Crossbreed",
            "coat": "Hairless/Furry down",
            "pattern": ""
        },
        {
            "breed": "Bengal",
            "country": "developed in the United States (founding stock from Asia)",
            "origin": "Hybrid",
            "coat": "Short",
            "pattern": "Spotted/Marbled"
        },
        {
            "breed": "Birman",
            "country": "developed in France (founding stock from Burma)",
            "origin": "Natural",
            "coat": "Semi Long",
            "pattern": "Colorpoint"
        },
        {
            "breed": "Bombay",
            "country": "developed in the United States (founding stock from Asia)",
            "origin": "Crossbred",
            "coat": "Short",
            "pattern": "Solid"
        },
        {
            "breed": "Brazilian Shorthair",
            "country": "Brazil",
            "origin": "Natural",
            "coat": "Short",
            "pattern": "All"
        },
        {
            "breed": "British Semi-longhair",
            "country": "United Kingdom",
            "origin": "",
            "coat": "Medium",
            "pattern": "All"
        },
        {
            "breed": "British Shorthair",
            "country": "United Kingdom",
            "origin": "Natural",
            "coat": "Short",
            "pattern": "All"
        },
        {
            "breed": "British Longhair",
            "country": "United Kingdom",
            "origin": "",
            "coat": "Long",
            "pattern": ""
        },
        {
            "breed": "Burmese",
            "country": "Burma and Thailand",
            "origin": "Natural",
            "coat": "Short",
            "pattern": "Solid"
        },
        {
            "breed": "Burmilla",
            "country": "United Kingdom",
            "origin": "Crossbreed",
            "coat": "Short/Long",
            "pattern": ""
        },
        {
            "breed": "California Spangled",
            "country": "United States",
            "origin": "Crossbreed",
            "coat": "Short",
            "pattern": "Spotted"
        },
        {
            "breed": "Chantilly-Tiffany",
            "country": "United States",
            "origin": "",
            "coat": "",
            "pattern": ""
        },
        {
            "breed": "Chartreux",
            "country": "France",
            "origin": "Natural",
            "coat": "Short",
            "pattern": "Solid"
        },
        {
            "breed": "Chausie",
            "country": "France",
            "origin": "Hybrid",
            "coat": "Short",
            "pattern": "Ticked"
        }
    ],
    "first_page_url": "https://catfact.ninja/breeds?page=1",
    "from": 1,
    "last_page": 4,
    "last_page_url": "https://catfact.ninja/breeds?page=4",
    "links": [
        {
            "url": null,
            "label": "Previous",
            "active": false
        },
        {
            "url": "https://catfact.ninja/breeds?page=1",
            "label": "1",
            "active": true
        },
        {
            "url": "https://catfact.ninja/breeds?page=2",
            "label": "2",
            "active": false
        },
        {
            "url": "https://catfact.ninja/breeds?page=3",
            "label": "3",
            "active": false
        },
        {
            "url": "https://catfact.ninja/breeds?page=4",
            "label": "4",
            "active": false
        },
        {
            "url": "https://catfact.ninja/breeds?page=2",
            "label": "Next",
            "active": false
        }
    ],
    "next_page_url": "https://catfact.ninja/breeds?page=2",
    "path": "https://catfact.ninja/breeds",
    "per_page": 25,
    "prev_page_url": null,
    "to": 25,
    "total": 98
}


### 404 Error
{
    "message": "Not Found",
    "code": 404
}


