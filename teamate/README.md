# Hyperledger Fabric Class Samples 예제

## [basic-network](https://github.com/bc8c/BS22_class-examples/tree/main/basic-network).

Network configuration

- 2 organizations ( ORG1 and ORG2 )
- 2 peers ( one peer for each organization )
- 2 couchdb (one couchdb for each peer )

## [basic-network-3Org](https://github.com/bc8c/BS22_class-examples/tree/main/basic-network-3Org).

teamte 를 복사해서 새로 만들어서 해보자.
hzTest라는 폴더를 하나 만들어서 한다.

순서대로 켜보자

네트워크 실행
./startnetwork.sh
./createchannel.sh
./setAnchorPeerUpdate.sh 
./deployCC.sh ( 왜이렇게 오래걸리지?)
—————————————
application 폴더로 이동해서

npm i

./ccp/ccp-generate.sh 만든다.
./getCert.sh

node addToWallet.js
appUser 가 잘 들어가고
node server.js
browser 에서 teamate 확인 할 수 있다.

http://localhost:5984/_utils/#login
id : admin
pw : adminpw

couch db 접속방법

Q) npm error
A) node module 폴더가 없으면 안된다. 
application 폴더에서 npm i 해야한다.

{"credentials":{"certificate":"-----BEGIN CERTIFICATE-----\nMIICmTCCAkCgAwIBAgIUFIsDVCoZW89+JZZapitbKcYwQJEwCgYIKoZIzj0EAwIw\naDELMAkGA1UEBhMCVVMxFzAVBgNVBAgTDk5vcnRoIENhcm9saW5hMRQwEgYDVQQK\nEwtIeXBlcmxlZGdlcjEPMA0GA1UECxMGRmFicmljMRkwFwYDVQQDExBmYWJyaWMt\nY2Etc2VydmVyMB4XDTIyMDMxNzExMjcwMFoXDTIzMDMxNzExMzIwMFowXTELMAkG\nA1UEBhMCVVMxFzAVBgNVBAgTDk5vcnRoIENhcm9saW5hMRQwEgYDVQQKEwtIeXBl\ncmxlZGdlcjEPMA0GA1UECxMGY2xpZW50MQ4wDAYDVQQDEwV1c2VyMTBZMBMGByqG\nSM49AgEGCCqGSM49AwEHA0IABAW05jMePi5EHMOvxulkeYO1jg/EZdlozQCMLgEl\nfH1rODdbebVXtK3jcI+bv8rz+T32JOTmp4FATID9rSJekq2jgdIwgc8wDgYDVR0P\nAQH/BAQDAgeAMAwGA1UdEwEB/wQCMAAwHQYDVR0OBBYEFO7qGMrSuA0SjoiZRhOk\nh1Gqp+YxMB8GA1UdIwQYMBaAFMOBrIcZYeyee6xazM1Eiw8KThT1MBUGA1UdEQQO\nMAyCCmJzdHVkZW50dmIwWAYIKgMEBQYHCAEETHsiYXR0cnMiOnsiaGYuQWZmaWxp\nYXRpb24iOiIiLCJoZi5FbnJvbGxtZW50SUQiOiJ1c2VyMSIsImhmLlR5cGUiOiJj\nbGllbnQifX0wCgYIKoZIzj0EAwIDRwAwRAIgTr8WFfDgqDfz6Hn70etnC5lyMCTq\nMOkxqXCdSK0yHJgCIDh35z3cgGhDgKab2eBiqmrzqvABSvoyHPbMDcIeYaop\n-----END CERTIFICATE-----\n","privateKey":"-----BEGIN PRIVATE KEY-----\nMIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wawIBAQQgao2g8Q4HRRpD5UDh\na4cJjiHcqMg/BHFXiUrjTLzKAZihRANCAAQFtOYzHj4uRBzDr8bpZHmDtY4PxGXZ\naM0AjC4BJXx9azg3W3m1V7St43CPm7/K8/k99iTk5qeBQEyA/a0iXpKt\n-----END PRIVATE KEY-----\n"},"mspId":"Org1MSP","type":"X.509","version":1}