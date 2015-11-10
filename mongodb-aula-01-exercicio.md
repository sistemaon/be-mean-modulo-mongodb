# MongoDB - Aula 01 - Exercício
autor: Erni Augusto FOnseca Souza (Systema_On)

## Importando os restaurantes
Inspiron@Inspiron-PC MINGW64 ~/Desktop
$ mongoimport --db be-mean --collection restaurantes --drop --file restaurantes.json
2015-11-10T01:24:24.625-0200    connected to: localhost
2015-11-10T01:24:24.628-0200    dropping: be-mean.restaurantes
2015-11-10T01:24:27.431-0200    imported 25359 documents

## Contando os restaurantes
Inspiron@Inspiron-PC MINGW64 ~/Desktop
$ mongo
2015-11-10T01:25:17.127-0200 I CONTROL  Hotfix KB2731284 or later update is not installed, will zero-out data files
MongoDB shell version: 3.0.7
connecting to: test
use be-mean
switched to db be-mean
db.restaurantes.find({}).count()
25359

