# teamate

# hyperledger fabric sample 

## pre-condition

* curl, docker, docker-compose, go, nodejs, python 
* hyperledger fabric-docker images are installed
* GOPATH are configured
* hyperledger bineries are installed (cryptogen, configtxgen ... etcs)

# -network

## 1. generating crypto-config directory, genesis.block, channel and anchor peer transactions

cd network

./generate.sh

## 2. starting the network, create channel and join 

./start.sh

# -chaincode

## 3. chaincode install, instsantiate and test(invoke, query, invoke)

./cc_tea.sh instantiate v1.0

# -prototype

cd ../prototype

## 4. nodejs module install

npm install

## 5. certification works

node enrollAdmin.js

node registerUser.js

## 6. server start

node server.js

## 7. open web browser and connect to localhost:8080



## 8. prototype 사이트맵 구조



![Untitled Diagram](https://user-images.githubusercontent.com/25717861/89747296-245ce100-daf9-11ea-9b39-77e2b4955abe.png)



## -web_template

#### 1. teamate/nework 이동

```powershell
cd network
```



#### 2.  ./teardown.sh 실행을 통해 container 제거

```powershell
./teardown.sh
```



#### 3. ./start.sh 실행을 통한 network 실행

```powershell
./start.sh
```



#### 4. ./cc_tea.sh 실행을 통한 chaincode install

```powershell
./cc_tea.sh
```



#### 5. web_template 로 이동 후 npm을 이용한 라이브러리 설치

```powershell
cd .. && cd web_template && npm install
```



#### 6. enrollAdmin.js 실행을 통한 adminID 등록 

###### web_template폴더안에 wallet 폴더가 존재하면 삭제후 다음과 같은 명령어 실행

```powershell
node enrollAdmin.js
```



#### 7. registerUser.js 실행을 통한 user등록

```shell
node registerUser.js
```



#### 8. Server 실행

```powershell
node server.js
```



#### 9. web_template Architecture

![ezgif com-video-to-gif (2)](https://user-images.githubusercontent.com/25717861/89754659-becc1d00-db17-11ea-96f4-a8fed08626ee.gif)







![Untitled Diagram (1)](https://user-images.githubusercontent.com/25717861/89753964-2339ad00-db15-11ea-9ea5-6f9b48f5f1a8.png)



#### 10.Web_template 시나오 보드

![Untitled Diagram (2)](https://user-images.githubusercontent.com/25717861/89756220-d4901100-db1c-11ea-9559-844ec31a0d74.png)



#### 11. Web_template Uml 

![Untitled Diagram (3)](https://user-images.githubusercontent.com/25717861/89759173-84b54800-db24-11ea-808d-2bffd4b50390.png)



