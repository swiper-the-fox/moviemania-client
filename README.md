# moviemania-client

**Register User**
----
  Add an User Account

* **URL**

  `/register`

* **Method:**
  
  `POST`
  
*  **URL Params**

   **Required:**
 
   `email=[string]`

   `password=[string]`

   **Optional:**

* **Data Params**

* **Success Response:**
  
  * **Code:** 201 <br />
    **Content:** `{"id": 4, "email": "taufiqgiri@mail.co.id"}`
 
* **Error Response:**

  * **Code:** 400 BAD REQUEST <br />
    **Content:** `{"message": "Email is already taken"}`

  OR

  * **Code:** 400 BAD REQUEST <br />
    **Content:** `{"message": ["User.email cannot be null", "User.password cannot be null"]}`

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._>

---

**User Login**
----
  Log In as an User Account

* **URL**

  `/login`

* **Method:**
  
  `POST`
  
*  **URL Params**

   **Required:**
 
   `email=[string]`

   `password=[string]`

   **Optional:**

* **Data Params**

* **Success Response:**
  
  * **Code:** 201 <br />
    **Content:** `{ "access_token"}`
 
* **Error Response:**

  * **Code:** 500 INTERNAL SERVER ERROR <br />
    **Content:** `{"message": "internal server error"}`

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._>

---

**Get Popular Movie**
----
  Get popular movies

* **URL**

  `/movies`

* **Method:**
  
  `GET`
  
*  **URL Params**

   **Required:**

   **Optional:**

* **Data Params**

    `access_token=[string]`

* **Success Response:**
  
  * **Code:** 200 <br />
    **Content:** `{"movies":[{"id": 682377, "title": "Chick Fight", "poster_path": "https://image.tmdb.org/t/p/w342//4ZocdxnOO6q2UbdKye2wgofLFhB.jpg"}, {"id": 724989, "title": "Hard Kill", "poster_path": "https://image.tmdb.org/t/p/w342//ugZW8ocsrfgI95pnQ7wrmKDxIe.jpg"}, ....`
 
* **Error Response:**

  * **Code:** 500 INTERNAL SERVER ERROR <br />
    **Content:** `{"message": "internal server error"}`

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._>

---

**Get A Movie**
----
  Get a movie by ID

* **URL**

  `/movies/:id`

* **Method:**
  
  `GET`
  
*  **URL Params**

   **Required:**

   **Optional:**

* **Data Params**

    `id=[integer]`

* **Success Response:**
  
  * **Code:** 200 <br />
    **Content:** `{"id": 2, "title": "Ariel", "release_date": "1988-10-21", "overview": "Taisto Kasurinen is a Finnish coal miner whose father has just committed suicide and who is framed for a crime he did not commit. In jail, he starts to dream about leaving the country and starting a new life. He escapes from prison but things don't go as planned...", "rating": 6.8, "genres": [{"id": 18, "name": "Drama"}, { "id": 80, "name": "Crime"}, {"id": 35, "name": "Comedy"}], "poster_path": "https://image.tmdb.org/t/p/w342//ojDg0PGvs6R9xYFodRct2kdI6wC.jpg"}`
 
* **Error Response:**

  * **Code:** 500 INTERNAL SERVER ERROR <br />
    **Content:** `{"message": "internal server error"}`

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._>