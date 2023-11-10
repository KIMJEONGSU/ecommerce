# Fashion Campus의 매출 증가를 위한 인사이트 도출과 이탈 예측 모델 구현

<br>

### 프로젝트 기간
2023.06.07 - 2023.07.04

### 기술 스택
- Python: pandas, sklearn, matplotlib, seaborn을 활용한 분석 및 시각화, 코드 리팩토링
- Google Drive

### 데이터 소개 _ [kaggle](https://www.kaggle.com/datasets/latifahhukma/fashion-campus?select=customer.csv)
<details>
<summary>고객 데이터</summary>
<div markdown="1">

1. Data shape : 100,000 rows X 15 columns
2. 컬럼 소개
    
    
    | 컬럼 | 소개 | 컬럼 | 소개 |
    | --- | --- | --- | --- |
    | customer_id | 고객아이디 | gender | 성별 |
    | first_name | 성 | birthdate | 생년원일 |
    | last_name | 이름 | device_type | 디바이스 타입 |
    | username | 닉네임 | device_id | 디바이스 아이디 |
    | email | 이메일 | device_version | 디바이스 버전 |

</div>
</details>

<details>
<summary>제품 데이터</summary>
<div markdown="1">

1. Data shape : 44,424 rows X 10 columns
2. 컬럼소개
    
    
    | 컬럼 | 소개 | 컬럼 | 소개 |
    | --- | --- | --- | --- |
    | id | 제품 아이디 | baseColor | 컬러 |
    | gender | 성별 | season | 계절 |
    | masterCategory | 큰 카테고리 | year | 연도 |
    | subCategory | 작은 카테고리 | usage | 의류분야 |
    | articleType | 의류종류 | productDisplayName | 제품이름 |

</div>
</details>

<details>
<summary>로그 데이터</summary>
<div markdown="1">

1. Data shape : 12,833,602 rows X 12 columns
2. 컬럼소개
    
    
    | 컬럼 | 소개 | 컬럼 | 소개 |
    | --- | --- | --- | --- |
    | session_id | 세션 아이디 | product_id | 제품 아이디 |
    | event_name | 페이지 이름 | quantity | 개수 |
    | event_time | 이벤트 타임 | item_price | 가격 |
    | event_id | 이벤트 아이디 | payment_status | 결제 성공 여부 |
    | traffic_source | 사용기기 | search_keywords | 검색 키워드 |

</div>
</details>

<details>
<summary>구매 데이터</summary>
<div markdown="1">

1. Data shape : 1,254,585 rows X 16 columns
2. 컬럼소개
    
    
    | 컬럼 | 소개 | 컬럼 | 소개 |
    | --- | --- | --- | --- |
    | created_at | 주문 일자 | payment_status | 결제 성공 여부 |
    | customer_id | 고객 아이디 | promo_amount | 할인된 가격 |
    | booking_id | 예약 아이디 | promo_code | 프로모션 코드 |
    | session_id | 세션 아이디 | shipment_fee | 배송비 |
    | payment_method | 결제 수단 | shipment_date_limit | 배송제한 날짜 |
</div>
</details>
