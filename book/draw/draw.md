
## connect info

[설계화면 바로가기](https://excalidraw.com/#json=4901323535286272,gsFj20UUbLiwjpXscIpIkA)


```elixir

[ 철수가 영희에게 '에어팟 프로' 상품을 추천하는 상황을 설계 ]

철수가 쿠팡 상품 페이지 접속
|> 리워드 링크 URL 생성 
|> 친구에게 카톡으로 추천 상품에 대한 URL 전달
|> 친구가 해당 URL 접속
|> 상품 주문 

```

```js

// 김철수의 개인 
{
    "추천인_ID" : "김철수"
    "상품명": "에어팟 프로",
    "품번": "MWP22KH/A",
    "공유링크" : "https://www.coupang.com/vp/products/332473915?itemId=1062243893&vendorItemId=5541656862&src=1191000&spec=10999999&addtag=400&ctag=332473915&lptag=CFM99390563&itime=20210904112532&pageType=PRODUCT&pageValue=332473915&wPcid=16306633054774387853578&wRef=&wTime=20210904112532&redirect=landing&isAddedCart="
}

// 김철수가 추천한 에어팟프로 페이지
{
    "방문자" : 322,
    "구매신청" : 4,
    "구매완료" : 3,
    "환불신청" : 1,
    "누적판매 금액" : 49299
}

// 김철수
{
    "user_ID": "김철수",
    "공유한 상품목록": ["에어팟프로","아이폰","엘지그램노트북"]
    "생성된 URL 목록" : ["에어팟프로url","에어팟프로url","에어팟프로url"]
}


// 김철수의 리워드 페이지
{
    "user_ID" : "김철수",
    "누적 리워드 " : SUM(["에어팟프로","아이폰","엘지그램노트북"].map(p=>p.rewards)) 
    "누적 방문자 " : SUM(["에어팟프로","아이폰","엘지그램노트북"].map(p=>p.visitors)) 
}
```
