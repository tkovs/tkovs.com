---
title: IMDb Web Crawler
summary: Um *web data extractor* para os filmes listados na seção de lançamentos do [IMDb](https://www.imdb.com/movies-coming-soon/?ref_=inth_cs)
tags:
- Data Mining
date: "2019-07-11T03:22:00Z"
---

Web Scraping para download de informações relacionadas aos filmes presentes no site IMDb, na seção de lançamentos. Atualmente, a ferramenta captura o título, ano de lançamento, diretores, estrelas, descrição, duração, nota, gêneros e a imagem de capa de cada filme da lista. As informações são salvas em um arquivo no formato json lines. As imagens são baixadas e salvas numa pasta separada.

O projeto utiliza python como linguagem de programação, a biblioteca scrapy para extração de dados do site em questão, e a biblioteca pytest para rodar os testes. Seu código fonte é publico e está em [meu github](https://github.com/tkovs/imdb_scrapy), livre para forks e contribuições. Para executar, basta seguir os passos descritos no README do repositório.

## Demonstração

No video abaixo eu mostro o projeto sendo executado, assim como o resultado.

{{< video library="1" src="crawl_imdb.mp4" controls="yes" >}}

JSON Lines gerado:

```json
{"title": "The Rental", "year": "2020", "genre": ["Horror", "Thriller"], "stars": ["Alison Brie", "Jovani Ridler", "Toby Huss", "Dan Stevens"], "director": "Dave Franco", "duration": null, "metascore": null, "description": "Two couples rent a vacation home for what should be a celebratory weekend get-away.", "image_urls": ["https://m.media-amazon.com/images/M/MV5BMjMwOGEyMTQtMDllMC00YTU3LTgyNzktYmEwY2Y4MjQzYmRkXkEyXkFqcGdeQXVyMjM4OTYzMTQ@._V1_UY209_CR0,0,140,209_AL_.jpg"]}
{"title": "Rebuilding Paradise", "year": "2020", "genre": ["Documentary"], "stars": [], "director": "Ron Howard", "duration": "95 min", "metascore": null, "description": "The community of Paradise, California, a town in the Sierra Nevada foothills, attempts to rebuild after devastating wildfires in 2018.", "image_urls": ["https://m.media-amazon.com/images/M/MV5BY2RkNjdmYmQtNjE0OC00MDdmLThkMDYtMmNkMmViNDcxOGIxXkEyXkFqcGdeQXVyMDgwMjQ4NQ@@._V1_UY209_CR2,0,140,209_AL_.jpg"]}
{"title": "Boys State", "year": "2020", "genre": ["Documentary"], "stars": ["Jack White", "Malec Moghadam"], "director": "Amanda McBaine", "duration": "109 min", "metascore": "74/100", "description": "A thousand 17-year-old boys from Texas join together to build a representative government from the ground up.", "image_urls": ["https://m.media-amazon.com/images/M/MV5BN2JmMzA1OTgtYTJmMC00Y2Q2LTg2ZWQtMzg2MWQ4MjFmODZkXkEyXkFqcGdeQXVyMjAwNTYzNDg@._V1_UX140_CR0,0,140,209_AL_.jpg"]}
{"title": "She Dies Tomorrow", "year": "2020", "genre": ["Comedy", "Drama", "Thriller"], "stars": ["Kate Lyn Sheil", "Jane Adams", "Kentucker Audley", "Katie Aselton"], "director": "Amy Seimetz", "duration": "84 min", "metascore": null, "description": "Amy thinks she's dying tomorrow...and it's contagious.", "image_urls": ["https://m.media-amazon.com/images/M/MV5BMTA5YWNkZDctOWUzMy00OGU0LThmYTQtYzJlZGQyZDkyNGEzXkEyXkFqcGdeQXVyMDM2NDM2MQ@@._V1_UY209_CR0,0,140,209_AL_.jpg"]}
{"title": "Words on Bathroom Walls", "year": "2020", "genre": ["Drama"], "stars": ["AnnaSophia Robb", "Walton Goggins", "Andy Garcia", "Molly Parker"], "director": "Thor Freudenthal", "duration": null, "metascore": null, "description": "A teenager coping with paranoid schizophrenia hopes his new experimental drug treatment will help him navigate high school and the outside world.", "image_urls": ["https://m.media-amazon.com/images/M/MV5BNDVlZWJiMWUtODkxMC00MjNlLWJlZjMtOTRjNTY1M2ViODE4XkEyXkFqcGdeQXVyODc3MjY5MjM@._V1_UX140_CR0,0,140,209_AL_.jpg"]}
{"title": "The Cuban", "year": "2019", "genre": ["Drama"], "stars": ["Ana Golja", "Louis Gossett Jr.", "Shohreh Aghdashloo", "Lauren Holly"], "director": "Sergio Navarretta", "duration": "109 min", "metascore": null, "description": "When a naive pre-med student named Mina gets her first job in a nursing home, an unexpected friendship with Luis, an elderly Cuban musician, reignites her love of music and changes her life forever.", "image_urls": ["https://m.media-amazon.com/images/M/MV5BZWFmYzFlNDMtNzNhYS00OTFhLWJjMjUtYjE2Y2I4MjBiMDNkXkEyXkFqcGdeQXVyNzE4OTk0MDU@._V1_UY209_CR2,0,140,209_AL_.jpg"]}
```

Uma das imagens baixadas:

![the rental](/img/the-rental.jpg)