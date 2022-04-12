네트워크 실행 순서

./startnetwork.sh
./createchannel.sh
./setAnchorPeerUpdate.sh 
./deployCC.sh

application 폴더로 이동해서

npm i

./ccp-generate.sh 만든다.
./getCert.sh

node addToWallet.js
appUser 가 잘 들어가고
node server.js
browser 에서 teamate 확인 할 수 있다.

Q) npm error
A) node module 폴더가 없으면 안된다. 
application 폴더에서 npm i 해야한다.

http://localhost:5984/_utils/#login
id : admin
pw : adminpw
couch db 접속방법
