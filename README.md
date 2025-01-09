# JS-Chapter5
JavaScript Chapter 5 Programming Assignment

In this project you will create an app that allows users to rank photos by clicking the images in a “photo bucket” to move them from the bucket to an ordered list of images. Clicking an image in the list returns the photo to the bucket while automatically renumbering the list. A preview of the completed project is shown in Figure 5-39.

![image](https://github.com/user-attachments/assets/6bfe706b-9958-4ac5-8347-3d9cc5b1ab17)

Figure 5-39

Do the following:

Use your code editor to open the index.html and script.js files. Enter your name and the date in the comment section of each file and commit.

Go to the index.html file in your code editor and in the head section add a script element to load the script.js file, deferring the app until the page is loaded. Review the contents and structure of the web document and then close the file, saving your changes.

Return to the script.js file in your code editor. Below the initial comment section declare the following variables:

The images variable containing an HTML collection of all elements with the tag name “img”.

The photoBucket variable referencing the element with the id “photo_bucket”.

The photoList variable referencing the element with the id “photo_list”.

Create a for loop that iterates through all of the items in the images collection.

Within the for loop insert an onclick event handler that runs an anonymous function when an image is clicked.

When an image is clicked it is either moved from the photo bucket to the photo list or from the photo list back to the photo bucket. To determine which action to perform, add the following if else statement to the anonymous function:

If the parent element of the clicked image has an id equal to “photo_bucket” then do the following:

Create an element node named newItem for the li element,

append newItem to the photoList object, and

append the image to the newItem object using the appendChild() method.

Note: Use the this object to reference the image that was clicked by the user.

Otherwise, do the following:

Declare a variable named oldItem equal to the parent element of the clicked image,

append the clicked image to photoBucket object, and

remove oldItem from the parent element of oldItem using the removeChild() method.

Commit your changes to the file and then load index.html in your web browser.

Verify that you can move items between the photo bucket and the photo list by clicking the image within either location.
