# beitlist API Documentation

## ContactUs
### ReviewAllMessages
- **Method**: `GET`
- **URL**: `http://127.0.0.1:8000/api/contacts/list`
---
### CreateMessage
- **Method**: `POST`
- **URL**: `http://127.0.0.1:8000/api/contacts/create`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
        "name": "andrew",
        "phone": "01234567890",
        "email": "andrew@gmail.com",
        "message": "violance"
    }
```
---
### UpdateMessage
- **Method**: `POST`
- **URL**: `http://127.0.0.1:8000/api/contacts/update/900`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
        "name": "kero",
        "phone": "01234567890",
        "email": "andrew@gmail.com",
        "message": "violance"
    }
```
---
### ReviewOneMessage
- **Method**: `GET`
- **URL**: `http://127.0.0.1:8000/api/contacts/show/5000`
#### Headers
- `Accept`: `application/json`
---
### DeleteMessage
- **Method**: `DELETE`
- **URL**: `http://127.0.0.1:8000/api/contacts/delete/1000`
---
## Reasons
### ShowReason
- **Method**: `GET`
- **URL**: `http://127.0.0.1:8000/api/reasons/show/2`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json

```
---
### AddReason
- **Method**: `POST`
- **URL**: `http://127.0.0.1:8000/api/reasons/add`
#### Body (raw JSON)
```json
{
    "name":"other"
}
```
---
## AboutUs
### ReviewAboutUs
- **Method**: `GET`
- **URL**: `http://127.0.0.1:8000/api/statics/about-us`
#### Headers
- `Accept`: `application/json`
---
### CreateAboutUs
- **Method**: `POST`
- **URL**: `http://127.0.0.1:8000/api/statics/about-us/create`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `title`: `title 2`
- `title_ar`: `سيبسيبسيب`
- `pre_title`: `dfsdfa`
- `pre_title_ar`: `شيبسيبسيبسبسيبسيبسيبسيب`
- `description`: `ssdfghjklkjhgfdsdfghjklkjhgf`
- `description_ar`: `fddfgdfgdfgdfgd`
- `image`: ``
---
### UpdateAboutUs
- **Method**: `POST`
- **URL**: `http://127.0.0.1:8000/api/statics/about-us/update/1`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `title`: `cvb`
- `title_ar`: `dsdcsd`
- `pre_title`: `sdcsdc`
- `pre_title_ar`: `dc`
- `description`: `sdc`
- `description_ar`: `xcvxcv`
- `image`: ``
---
## UserReview
### GetAllReviews
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/reviews/list`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json

```
---
### ShowAReview
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/reviews/show/1333`
---
### AddReview
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/reviews/create`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "comment": "tst",
    "rating": 2,
    "user_to_id": 13
}
```
---
### UpdateReview
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/reviews/update/1`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "comment": "tst",
    "rating": 1,
    "user_to_id": 12
}
```
---
### Myreviews
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/users/reviews`
#### Headers
- `Accept`: `application/json`
---
### DeleteReview
- **Method**: `DELETE`
- **URL**: `{{apiUrl}}/api/reviews/1/delete`
#### Headers
- `Accept`: `application/json`
---
## Auth
### register
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/register`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "fullname": "kyrillos",
    "email": "kkk@gmail.com",
    "phonenumber": "012025502657525",
    "password": 123456789,
    "usertype" : 1,
    "email_contact":0,
    "phone_contact":0,
    "whatsapp_contact":0
}
```
---
### login
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/login`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "email": "kkk@gmail.com",
    "password": "123456789"
}
```
---
### Profile
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/users/profile`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json

```
---
### UpdateProfile
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/users/update/profile`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `subscribtion_id`: `3`
---
### Logout
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/logout`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    
}
```
---
### changepassword
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/users/change-password`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `currentPassword`: `123456789`
- `password`: `123456789K`
---
## User
### ListUsers
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/users/list`
---
## Listing
### showListing
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/properties/list?page=1&perPage=2`
#### Headers
- `Accept`: `application/json`
#### Query Parameters
- `page`: `1`
- `perPage`: `2`
---
### AddListing
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/properties/create`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `name`: `hjfgh`
- `name_ar`: `fghfgh`
- `description`: `fgfg`
- `description_ar`: `fghf`
- `type`: `1`
- `bathrooms`: `1`
- `bedrooms`: `1`
- `location_id`: `1`
- `size`: `21`
- `propertytype_id`: `1`
- `view`: `asda`
- `price`: `10000`
- `thumbnail`: ``
- `cover`: ``
- `images[]`: ``
---
### UpdateList
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/properties/update`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `name`: `andy`
- `name_ar`: `slkdhskdl`
- `description`: `kjbkjnbkj`
- `description_ar`: `dsfsdf`
- `bedrooms`: `1`
- `bathrooms`: `2`
- `location_id`: `2`
- `size`: `35`
- `view`: `asfasd`
- `price`: `20020`
- `map`: `fsdfhjk`
- `propertytype_id`: `1`
- `thumbnail`: ``
- `cover`: ``
- `images[]`: ``
- `id`: `94`
---
### SortList
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/properties/sort?sortBy=price_asc&pagenumber=3`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
#### Query Parameters
- `sortBy`: `price_asc`
- `pagenumber`: `3`
---
### DeleteImages
- **Method**: `DELETE`
- **URL**: `{{apiUrl}}/api/properties/1/delete-images`
#### Headers
- `Accept`: `application/json`
#### Query Parameters
- `offset`: `0`
- `limit`: `10`
---
### PendingList
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/properties/list/pending?offset=1&limit=2`
#### Query Parameters
- `offset`: `1`
- `limit`: `2`
---
### ListingSearch
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/properties/search?propertytype=1&minPrice=0&maxPrice=100000&minArea=20&maxArea=22&bathrooms=1&type=2&location_id=1&compound_id=1&description=fgfg&outdoors=garden&features=1&perPage=1&sortBy=price_desc`
#### Headers
- `Accept`: `application/json`
#### Query Parameters
- `propertytype`: `1`
- `minPrice`: `0`
- `maxPrice`: `100000`
- `minArea`: `20`
- `maxArea`: `22`
- `bathrooms`: `1`
- `type`: `2`
- `location_id`: `1`
- `compound_id`: `1`
- `description`: `fgfg`
- `outdoors`: `garden`
- `features`: `1`
- `perPage`: `1`
- `sortBy`: `price_desc`
---
### MyListing
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/users/properties`
#### Headers
- `Accept`: `application/json`
---
## Subscribtion
### GetAllSubscribtions
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/subscribtions/list`
#### Headers
- `Accept`: `application/json`
---
### CreateSubscribtion
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/subscribtions/create`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "name": "five",
    "name_ar": "five",
    "price": 200,
    "listsno" :5
}
```
---
### DeleteSubscribtion
- **Method**: `DELETE`
- **URL**: `{{apiUrl}}/api/subscribtions/delete/1`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "id": 2,
    "name": "kero",
    "name_ar": "keero",
    "price": 200
}
```
---
### ShowOneSubscribtion
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/subscibtions/show/1`
#### Headers
- `Accept`: `application/json`
---
### UpdateSubscribtion
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/subscribtions/update/1`
#### Headers
- `Accept`: `application/json`
#### Body (raw JSON)
```json
{
    "name": "kero",
    "name_ar": "keero",
    "listsno": 1,
    "price": 200
}
```
---
## Reports
### AllReports
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/property/reports`
#### Headers
- `Accept`: `application/json`
---
### CreateReport
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/proerty/reports/create`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `body`: `test body`
- `property_id`: `1`
---
### UpdateReport
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/proerty/reports/update/1`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `body`: `1`
- `property_id`: `1`
---
## Company
### DeleteACompany
- **Method**: `DELETE`
- **URL**: `{{apiUrl}}/api/companies/delete/100`
#### Headers
- `Accept`: `application/json`
---
### ShowACompany
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/companies/show/20`
#### Headers
- `Accept`: `application/json`
---
### GetAllCompanies
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/companies/list`
#### Headers
- `Accept`: `application/json`
---
### CreateCompany
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/companies/create?name=facebook&name_ar=fa&description=asdas&description_ar=asdasd`
#### Headers
- `Accept`: `application/json`
#### Query Parameters
- `name`: `facebook`
- `name_ar`: `fa`
- `description`: `asdas`
- `description_ar`: `asdasd`
---
### UpdateCompany
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/companies/update/200`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `name`: `12`
- `name_ar`: `asd`
- `description`: `asd`
- `description_ar`: `asdasda`
---
## Slideshow
### GetAllslides
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/slides/list`
---
### CreateSlideshow
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/slides/create`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `name`: `k`
- `name_ar`: `k`
- `shortdesc`: `ss`
- `shortdesc_ar`: `fad`
- `customorder`: `2`
- `image`: ``
---
### GetASlide
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/slides/show/100`
#### Headers
- `Accept`: `application/json`
---
### DeleteASlide
- **Method**: `DELETE`
- **URL**: `{{apiUrl}}/api/slides/delete/600`
#### Headers
- `Accept`: `application/json`
---
### UpdateSlideshow
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/slides/update/2`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
- `name`: `as`
- `name_ar`: `asd`
- `shortdesc`: `asdas`
- `shortdesc_ar`: `asdasd`
- `customorder`: `3`
- `image`: ``
---
## Favourite
### GetMyFavListings
- **Method**: `GET`
- **URL**: `{{apiUrl}}/api/properties/favorites`
#### Headers
- `Accept`: `application/json`
#### Body (form-data)
---
### AddFavListing
- **Method**: `POST`
- **URL**: `{{apiUrl}}/api/properties/add-to-favorite/100`
#### Headers
- `Accept`: `application/json`
#### Query Parameters
- `id`: `1`
---