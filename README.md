#### For this exercise, we are using [jsonplaceholder](https://jsonplaceholder.typicode.com/).
- Create a 2-column layout. 
- Left column shows a list of post titles, each of the list items are clickable.
- Right column shows the detail of the clicked item (title and body).
- Body should be editable. To achieve this, you must render the contents into a textarea form element, and when the user hits ‘Enter’, an action is dispatched which calls the following endpoint: https://jsonplaceholder.typicode.com/posts/[POST_ID], where POST_ID is the selected post’s Id. The method of the call should be a ‘PATCH’, and the request body must be the following object: { body: [TEXTAREA_VALUE] }, where TEXTAREA_VALUE is the string that the user entered in the textarea field.

#### UI
https://drive.google.com/file/d/16mCo5g3nirlOI2xjC2qVh4XJgGCq651V/view?usp=sharing

#### get all posts
https://jsonplaceholder.typicode.com/posts

#### more CRUDs
https://jsonplaceholder.typicode.com/guide.html
