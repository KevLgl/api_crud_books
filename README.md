# CesiCar - Api/BackOffice
Cette documentation va vous aider à lancer l'api localement

## ENVIRONMENT
| Language | version     | Description                |
| :-------- | :------- | :------------------------- |
| `php` | `8.1.18` | **Required**. 8.1 minimum |
| `node` | `18.15.0` |  |
| `npm` | `9.5.0` |  |

<details>
<summary>INSTALLATION</summary>

## 1/ Clone project
```bash
  git clone repositoryName
```

## 2/ install vendors
```bash
  composer install
```
## 3/ install nodes
```bash
npm install
```

## 4/ Create .env
```bash
Create file .env.local in your root folder
```
Add this line with your DB parametes :
```bash
DATABASE_URL="mysql://login:password@127.0.0.1:3306/databasename?serverVersion=yourmysqlversion"
```

## 5/ Create the Database
```bash
php bin/console doctrine:database:create
```

## 6/ Apply DB migrations :
```bash
php bin/console doctrine:s:u --force
```

## 8/ Start API 
```bash
symfony server:start
```
</details>

<details>
<summary>UPDATES / PULL</summary>



Access API
127.0.0.1:8000/api

## Access api using helper
127.0.0.1:8000/_profiler
-> help : https://symfonycasts.com/screencast/api-platform/profiler
</details>
