## building ***Models*** to work with and also the docs of the api
### ***CRUD*** operation
1. **C** -> **Create**: make new record like (POST)
2. **R** -> **Read**: bring data to read them (GET)
3. **U** -> **Update**: modify data (POST)
4. **D** -> **Delete**: to remove record (DELETE)

### ***ERD***: Entity Relationship Diagram to build database design models

---
#### *Categories*
- id
- title

> `GET /~/api/categories` -> return all categories

> `GET /~/api/category/{id}` -> return the  given category by id

> `GET /~/api/category/{id}/posts` -> return the posts for given category

> `POST /~/api/categories` -> add a new category

> `POST /~/api/category/{id}` -> update the  given category by id

> `DELETE /~/api/category/{id}` -> delete the  given category by id
---
#### *Author*
- id
- name
- avatar
> `GET /~/api/authors` -> returns all authors

> `GET /~/api/author/{id}` -> return the given author by id

> `GET /~/api/posts/author/{id}` -> return all posts for the given author id
 
> `POST /~/api/authors` -> add a new author

> `POST /~/api/author/{id}` -> update the given author by id

> `DELETE /~/api/author/{id}` -> delete the given author by id
---
#### *Post*
- id
- title
- author
- Date Time
- content
- [comments]
- featuredImage
- vote up
- vote down

> `GET ~/api/posts` -> return all posts

> `GET ~/api/post/{id}` -> return the given post by id

> `POST ~/api/posts` -> create new post

> `POST ~/api/post/{id}` -> update the given post by id

> `DELETE ~/api/post/{id}` -> delete the given post by id
---
#### *comment*
- id
- author
- datetime (the calculated time from the time that written in until now)
- content

> `GET ~/api/post/{id}/comments` -> return all comments for the given post

> `GET ~/api/comment/{id}` -> return the given comment by id

> `POST ~/api/post/{id}/comments` -> create new comment for the given post

> `POST ~/api/comment/{id}` -> update the given comment by id

> `DELETE ~/api/comment/{id}` -> delete the given comment by id