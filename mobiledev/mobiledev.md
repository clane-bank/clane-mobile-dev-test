![alt text](https://avatars3.githubusercontent.com/u/17319994?s=200&v=4)
## Clane Mobile Software Engineer Challenge

### Requirements
- You will be provided a set of simple news API to work with.
- Your assignment would require you to create a simple react-native app using the API given to you.
- A simple landing page that would display all the news (Paginated) with a `next` and `back` links
- Clicking on any of the news would display a single news in a separate page with the images and comments. Also add a form to add a new comment to the news. Also ability to edit/delete any comment on the news.
- We'd also like you to display the images on the news view page as a slider.
- A form to Create and update news. 

### API Endpoints
  > BaseUrl for the api: `https://5e4bfc87a641ed0014b02740.mockapi.io/api/clane/`

  |Method|Endpoint|Description|
  |------|--------|-----------|
  |`GET` |`/news`| Get all news|
  |`GET` |`/news?page=1&limit=10`| Get paginated news|
  |`GET`| `/news/:id`| Get news by id|
  |`POST`| `/news`| Add news item|
  |`PUT`| `/news/:id`| Update news item|
  |`DELETE`| `/news/:id`| Delete news item|
  |`GET`| `/news/:id/images`| Get Images for news|
  |`POST`| `/news/:id/images`| Add Image to News|
  |`DELETE`| `/news/:id/images/:id`| Delete image from news|
  |`GET`| `/news/:id/comments`| Get comments on a news|
  |`POST`| `/news/:id/comments`| Add Comment to news|
  |`PUT`| `/news/:id/comments/:id`| Edit comment on a news|
  |`DELETE`| `/news/:id/comments/:id`| Delete comment on news item|

  Sample Data from Creating a news news
  ```json
  {
      "author": "Seun Matt",
      "title": "This is a title"
  }
  ```
  Sample Data for Creating Comment
  ```json
  {
      "newsId": 1,
      "name": "Jan Wuckert",
      "avatar": "http://lorempixel.com/640/480/fashion",
      "comment": "This is me saying you're bluffing!"
  }
  ```

  Sample Data for adding Image
  ```json
  {
      "newsId": 1,
      "image": "http://lorempixel.com/640/480/fashion"
  }
  ```

### Notes
- This is a test of your knowledge of react-native, therefore
  - You are expected to provide your solution in using react-native components
  - Do not worry about the security.
  - Handle validation properly for `POST/PUT` requests 
- Source code must be stored in a git repository (you can send us a link to a github or bitbucket repo)
  - For public repos:
	  - Avoid words like `clane` and `challenge`.
	  - This is needed to prevent other candidates from finding your solution.
- Your repo should be easy to setup with clear instruction.
- The Postman collection for the APIs [is located here](Clane%20Mobile%20Test%20Scripts.postman_collection.json)

### Libraries Suggestion for ReactNative
- Please use `Axios` for APIs consumption (https://github.com/axios/axios)
- Please use `rematch` for redux implementation (https://rematch.github.io/rematch/#/README?id=rematch)
- Please use `react-native-elements` https://react-native-training.github.io/react-native-elements/

### Expection
- This challenge should take around 2 days to complete.
- You are allowed to use libraries that can make your work standout and that you are most convenient with.
- You can work on it at your own schedule, but a complete solution is expected within 7 days.
- Your code should be modular, each module should focus on doing one thing and do it well.
- Please, over-engineering is allowed.
- Error handling and retry if backend is busy.
- We frown at code repetitions and we expect a more clean code.
- We value code re-usability.
- We value offline first where necessary.
- We love well documented codebase with good naming conventions.
- We favour good code structure.

**Questions? We love to answer: <careers@clane.com>**
