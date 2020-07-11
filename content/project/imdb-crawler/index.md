---
title: IMDb Web Crawler
summary: Um *web data extractor* para os filmes listados na seção de lançamentos do [IMDb](https://www.imdb.com/movies-coming-soon/?ref_=inth_cs)
tags:
- Data Mining
date: "2019-07-11T03:22:00Z"
---

Web Scraping para download de informações relacionadas aos filmes presentes no site IMDb, na seção de lançamentos. Atualmente, a ferramenta captura o título, ano de lançamento, diretores, estrelas, descrição, duração, nota, gêneros e a imagem de capa de cada filme da lista. As informações são salvas em um arquivo no formato json lines. As imagens são baixadas e salvas numa pasta separada.

O projeto utiliza python como linguagem de programação, a biblioteca scrapy para extração de dados do site em questão, e a biblioteca pytest para rodar os testes. Seu código fonte é publico e está em [meu github](https://github.com/tkovs/imdb_scrapy), livre para forks e contribuições. Para executar, basta seguir os passos descritos no README do repositório.