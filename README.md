# dockerSQLtoLocal
## 專案說明
### 專案名稱: 使用pgAdmin操作Docker上的PostgreSQL
**詳情請參閱[DockerPostgreSQLPgAdmin實作說明.pdf 檔案]
(https://github.com/jerry7776112/dockerSQLtoLocal/blob/main/DockerPostgreSQLPgAdmin%E5%AF%A6%E4%BD%9C%E8%AA%AA%E6%98%8E.pdf)**
### 實作說明
* 使用Docker所提供的PostgreSQL
* 使用本地端pgAdmin連線Docker上的PostgreSQL
* 使用本地端pgAdmin與Docker上的PostgreSQL互動
* 將相關指令寫入MakeFile

### 前置準備
* pgAdmin下載
<https://www.pgadmin.org/download/>
* minGW 下載
<https://sourceforge.net/projects/mingw/postdownload>
* Docker 下載
<https://docs.docker.com/desktop/install/windows-install/>

### 實務知識
* Docker 初探
* 使用powershell 連線至 Docker PostgreSQL
* 本地pgAdmin與Docker PostgreSQL連線
* MakeFile使用

### Flow
![flowchart](https://github.com/jerry7776112/dockerSQLtoLocal/blob/main/flow/flow1.png "flowchart")

#### pgAdmin 
為一可介面化操作與管理PostgreSQL的應用程式
#### MinGW
* MinGW為可在**Windows環境執行** Linux make 指令為主的一個工具程式，並且經由讀取一個叫做 MakeFile 的檔案，自動化建構軟體。
* 簡單說，就是可透過將**重複且複雜的指令**撰寫在MakeFile中，使用make指令去呼叫**重複複雜的指令**，這樣可省去大量編譯的時間

### 會使用到的Docker指令
* docker ps: 查看運作中的container
* docker ps –a: 查看所有container，不論是否運作中
* docker images: 查看images
* docker pull [image_name]: 下載images
* docker run: 執行啟動images
* docker exec –it: 操作images
* docker stop: 終止關閉運作
