
<h1 align="center">PetaConnect Aipet.id Apps With Matchmaking Ai </h1> <br/>




![Logo](https://raw.githubusercontent.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/main/image/PetaConnect%20Apet.id%20Apps%20with%20Matchmaking%20Ai.jpg)


## Description
An Android-based application designed to solve the problem of stray dog overpopulation in Bali by connecting stray dogs with potential suitable owners.

## Motto : 

<p align="center">"Bersama PETA Connect, Mengubah Overpopulasi Menjadi Kesempatan Adopsi yang Menyenangkan."</p>

## Team PetaConnect

| Name | Path | Bangkit ID | Sosial Media |
| ------- | ------- | ------- | ------- |
| Wahyu Sahri Rhamadhan | Cloud Computing | C525BSY3282 | [Linkedin](https://www.linkedin.com/in/wahyu-sahri-rhamadhan/) |
| Kesya Nursyahada | Machine Learning | M296BSX1003  | Baris 2, Kolom 4 |
| Anya Ningrum Nur’afifah | Machine Learning | M296BSX1008  | Baris 3, Kolom 4 |
| Darmawan Kristiaji | Machine Learning | M318BSY0867 | Baris 3, Kolom 4 |
| Ilham Gusti Syah Putro | Mobile Developer | A129BSY2465 | Baris 3, Kolom 4 |
| Muhammad Ahsanur Rafi | Cloud Computing | C296BSY4312 | Baris 3, Kolom 4 |


## Screeshot
## Features

- Login/Register
- Onboarding 
- Dasboard
- Recomendation
- Dog Detail
- Location For Dog on Maps
- Profile
- Clinic Service 
- Maps Selter
- Guide Dog


## Badges

Program tools : 

![Flask](https://img.shields.io/badge/-Flask-05122A?style=flat&logo=flask)&nbsp;
![Git](https://img.shields.io/badge/-Git-05122A?style=flat&logo=git)&nbsp;
![GitHub](https://img.shields.io/badge/-GitHub-05122A?style=flat&logo=github)&nbsp;
![PHP](https://img.shields.io/badge/--%20php?style=flat&logo=php&logoColor=white&label=PHP%20Programing&labelColor=blue&color=31BAD2)&nbsp;
![laravel](https://img.shields.io/badge/--%20php?style=flat&logo=laravel&logoColor=white&label=Laravel%20Framewrok&labelColor=%23AA1128&color=red)&nbsp;
![MySQL](https://img.shields.io/badge/--%20MYSQL?style=flat&logo=Mysql&label=MYSQL&labelColor=white&color=blue)&nbsp;
![Postman](https://img.shields.io/badge/postman-11?style=flat&logo=postman&color=black)&nbsp;
![Dokcer](https://img.shields.io/badge/docker-11?style=flat&logo=docker&labelColor=black&color=blue)&nbsp;
![Static Badge](https://img.shields.io/badge/kotlin-102?style=flat&logo=kotlin&labelColor=black&color=blue)

![Static Badge](https://img.shields.io/badge/python-1?style=flat&logo=python&labelColor=yellow&color=blue)


## Infrastructur


![infrastuctur](https://raw.githubusercontent.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/main/image/infrastuctur-desin-spesification.jpg)


## Cloud Computing Documentation


## A. Installation

### # in Local Meachine Server/ backend






clone project

```bash
  git clone https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI.git
```

Go to the project directory

```bash
  cd CC/backend-Aipet-app/src
```

upgrade Composer

```bash
  composer update
```

CP .env.example to .env

```bash
  cp .env.example .env
```

key generate Laravel

```bash
  php artisan:key generate
```

go test sever

```bash
  php artisan serve

```

Open link server

[http://127.0.0.1:8000](http://127.0.0.1:8000)

### finaly picture
if you success install your local

![Logo](https://raw.githubusercontent.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/main/image/server.jpg)




## Deployment in Google Cloud


### Making Infrastructur

**A. Virtual Machine**

you can follow my spesification

![Logo](https://raw.githubusercontent.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/main/image/sepecification-vm.png)

### or

Creating a virtual machine in Google Cloud, make sure to select the same zone as the other instance to use to store the instance, or you can visit [Documentation](https://cloud.google.com/compute/docs/instances/create-start-instance) link provided by Google for instance creation.



**B. Bucket Storage**

1. Create Bucket Storage in Google CLoud, you can follow  [Documentation](https://cloud.google.com/storage/docs/creating-buckets) link provided by Google 

2. Go to IAM Google Cloud, you can follow [Role IAM](https://cloud.google.com/storage/docs/access-control/iam-roless)
3. Getting App key and go to file CC/backend-Aipet-app/src click credential.json, copy paste in there with you credential
4. Go change with your bucket name in your file, go CC\backend-Aipet-app\src\app\Http\Controllers\GoogleCloudStorageController.php

```bash
  private $bucket = '['YOUR BUCKET NAME']';
```
local

```bash
   'keyFilePath' => '['PATH YOUR CREDENTIAL.JSON']',
```
in docker

```bash
   'keyFilePath' => '['/var/www/app/credensial.json']',
```


**C. Cloud SQL**

1. Go create Cloud SQL in google cloud you can follow and read  [Documentation](https://cloud.google.com/sql/docs/mysql)
2. You can choose in public IP (Recomended) or Private IP
3. Give access in your VM in Conection -> write your IP VM
3. And go change in your .env your backend in CC/backend-Aipet-app/src

```bash
#seeting for coud sql
DB_CONNECTION=mysql
DB_HOST=['YOUR PUBLIC IP SQL']
DB_PORT=3306
DB_DATABASE=['YOUR DATABASE NAME']
DB_USERNAME=['YOUR USER']
DB_PASSWORD=['YOUR DB_PASSWORD]
```


## Running Dokcer in VM

go your vm you with clone project in your local project, or you can clone in project repo

**VM Requirement**
* Laravel 10
* PHP version 8.1
* [Dokcer](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04)
* Docker-Compose

```bash
   sudo apt  install docker-compose
```
* git
```bash
   sudo apt install git
```

**Docker Installation**

get root file there CC/backend-Aipet-app

```bash
   docker-compose up -d --build
```
get run your public ip your vm


Enjoy :v

## Documentation API 

File Api Documentation name file "openapi (1).json"
* [File Api Documentation ](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/tree/main/CC/backend-Aipet-app/postmantest)

Link Swagger.io
* [Swagger.io](https://editor.swagger.io/)

## Mobile Documetation
| ![Gambar 1](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/fd7aa84c-964c-44a3-8668-a76914c664e0) | ![Gambar 2](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/62add4b5-eef9-4658-8719-32a34c411985) | ![Gambar 3](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/d1cdeb9f-1e8c-48de-b392-e3f38a28ca5d) |
| --- | --- | --- |
| ![Gambar 4](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/e4aa0452-eeb9-4cfb-93e5-9201e6a88fd1) | ![Gambar 5](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/98629ca3-a637-4d70-b33a-1df513ed2ca0) | ![Gambar 6](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/2e946d62-9e7d-4b38-b0c6-46607f17fb07) |
| ![Gambar 7](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/84659d09-21f9-433d-9170-c4f37d3f7505) | ![Gambar 8](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/12d43fc4-0184-445d-85a0-0512df9ef174) | ![Gambar 9](https://github.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/assets/93174860/cc696a14-4361-4137-925c-36c4a8d08dc7) |
## ML Documentation
