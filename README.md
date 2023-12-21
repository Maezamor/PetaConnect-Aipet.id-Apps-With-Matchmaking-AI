
<h1 align="center">PetaConnect Aipet.id Apps With Matchmaking Ai </h1> <br/>




![Logo](https://raw.githubusercontent.com/Maezamor/PetaConnect-Aipet.id-Apps-With-Matchmaking-AI/main/image/PetaConnect%20Apet.id%20Apps%20with%20Matchmaking%20Ai.jpg)


## Description
## Team PetaConnect

| Name | Path | Bangkit ID | Sosial Media |
| ------- | ------- | ------- | ------- |
| Baris 1, Kolom 1 | Baris 1, Kolom 2 | Baris 1, Kolom 3 | Baris 1, Kolom 4 |
| Baris 2, Kolom 1 | Baris 2, Kolom 2 | Baris 2, Kolom 3 | Baris 2, Kolom 4 |
| Baris 3, Kolom 1 | Baris 3, Kolom 2 | Baris 3, Kolom 3 | Baris 3, Kolom 4 |


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
   'keyFilePath' => '['PATH YOUR CREDENTIAL.JSON']',
```


**C. Cloud SQL**

1. Go create Cloud SQL in google cloud you can follow and read  [Documentation](https://cloud.google.com/sql/docs/mysql)

