## Tables

### Firebase Auth

| field | type | description |
|:--------:|:----:|:-----------:|
| display_name | String | User display name |
| email | String |  |
| photo_url | Uri |  | 

### FireStore

#### CoffeeBean(/v1/coffee_beans)

| field | type | description |
|:--------:|:----:|:-----------:|
| roasted_at | Date | Coffee Bean roasted date (format: 'yyyy-mm-dd') |
| memo | String | Bean memo |
| link | String | Bean link |
| image | FirebaseStorageImage | Picture storage in FirebaseStorage |
| rating | Int | Number of rating 1 ~ 5. |
| shop_reference | DocumentReference | Shop table record id |

#### Shop(/v1/shops)

| field | type | description |
|:--------:|:----:|:-----------:|
| name | String | Shop name |
| link | String | Shop link |
| location | GeoPoint |

#### Relations

- CoffeeBean: 1 - n: Shop

### Storage
