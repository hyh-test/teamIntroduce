item smiluation

기능들
--request POST \ --url http://localhost:3018/api/sign-up \  회원가입기능
--request POST \  --url http://localhost:3018/api/sign-in \ 로그인기능
--request GET \ --url http://localhost:3018/api/users \ 로그인한 유저에 대한 조회기능 (JWT인증)
--request POST \  --url http://localhost:3018/api/character \ 로그인한 유저에 대해서 캐릭터 생성   (JWT인증) { body 안에 name : " " 가 필요}
--request GET \  --url http://localhost:3018/api/character/:charcterid \ 로그인한 유저에 대해서 캐릭터 상세 조회   (JWT인증)   { :charcterid 에 대해서 조회}
--request DELETE \  --url http://localhost:3018/api/character/:charcterid \로그인한 유저에 대해서 캐릭터 아이디에 해당하는 캐릭터 삭제  (JWT인증)   { :charcterid 의 캐릭터 삭제}
--request PATCH \ --url http://localhost:3018/api/character/money/:charcterid \로그인한 유저에 대해서 캐릭터에 돈을 추가하는 기능 (JWT인증)   { :charcterid 에 돈 추가}
--request POST \  --url http://localhost:3018/api/item/create \ 아이템 생성
--request PATCH \  --url http://localhost:3018/api/item/:itemId \ 아이템 수정 
--request GET \  --url http://localhost:3018/api/item/items \ 아이템 전체 조회
--request GET \   --url http://localhost:3018/api/item/:itemId \ 아이템 상세 조회
--request POST \  --url http://localhost:3018/api/itemshop/buy/:charcterId \로그인한 유저의 캐릭터의 아이템 구매  (JWT인증)   { :charcterid 의 인벤토리에서 아이템 구매  body 안에 itemId: 가 필요 숫자만  }
--request PATCH \  --url http://localhost:3018/api/itemshop/sell/:charcterId \로그인한 유저의 캐릭터의 아이템 판매 (JWT인증)  { :charcterid 의 인벤토리에서 아이템 판매  body 안에 itemId: 가 필요 숫자만 }
--request GET \--url http://localhost:3018/api/inventory/:charcterId \캐릭터의 아이템 조회   (JWT인증)   { :charcterid 의 인벤토리 조회 캐릭터 주인이 아니면 돈은 조회 불가 }
--request GET \  --url http://localhost:3018/api/equippedItem/:charcterId  \캐릭터의 장착된 장비 조회 (JWT인증) { :charcterid 의 장착된 장비 조회  }
--request POST \  --url http://localhost:3018/equippedItem/equip/:characterid  \ 로그인한 유저의 캐릭터 장비 장착하기 (JWT인증) { :charcterid 의 인벤토리에서 장착  body 안에 itemId: 가 필요 숫자만 }
--request POST \  --url http://localhost:3018/equippedItem/unequip/:characterid \  로그인한 유저의 캐릭터 장비 해제하기 (JWT인증) { :charcterid 의 장비된 장비에서 탈착  body 안에 itemId: 가 필요 숫자만}




