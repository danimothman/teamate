## README.md



# teamate

# hyperledger fabric sample

## pre-condition

- curl, docker, docker-compose, go, nodejs, python
- hyperledger fabric-docker images are installed
- GOPATH are configured
- hyperledger bineries are installed (cryptogen, configtxgen ... etcs)

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



**8. prototype 사이트맵 구조**

![](C:\Users\22\Downloads\Untitled Diagram.png)

-web_template

1. teamate/network 이동

   `cd network`

2. ./teardown.sh 실행을 통해 container 제거

   `./teardown.sh`

3. ./start.sh 실행을 통한 network 실행

   `./start.sh`

4. ./cc_tea.sh 실행을 통한 chaincode install

   `./cc_tea.sh`

5. web_template로 이동 후 npm을 이용한 라이브러리 설치

   `cd .. && cd web_template && npm install`

6. enrollAdmin.js 실행을 통한 adminID등록

   web_template폴더안에 wallet 폴더가 존재하면 삭제후 다음과 같은 명령어 실행

   `node enrollAdmin.sh`

7. registerUser.js 실행을 통한 

   `node registerUser.sh`

8. sd

   ![](C:\Users\22\Downloads\Untitled Diagram (1).png)

9. web_template Architecture

   ![](C:\Users\22\Downloads\Untitled Diagram (1) (1).png)

10. web_template 시나리오 보드

    ![](C:\Users\22\Downloads\화면 플로우 차트.png)

11. web_template(UML)

    ![](C:\Users\22\Downloads\UML-sequence.png)



    ```
    
    ```

    

12. dfd

    

13. 

14. 

15. 

16. 

17. 

18. 

19. 

    















