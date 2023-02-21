Hi Alisiia!

Nice choice for the assignment! And it'sintersting you went old scoll with the XMLHttpRequest - it's what I studied at school!

Unfortunately I'm getting an error on page load and nothing happens when I click the button. I'm 100% sure that what is happening is the JS is executing before the html has finished loading, so on line 4 of the JS:

  btn.addEventListener("click", function() {

it crashes because "btn" does not exist yet.

The quick fix is to add "defer" to link in the html where you import the JS file on line 12. Defer means the JS will run AFTER everything else. Read about it here: https://www.w3schools.com/tags/att_script_defer.asp

Fixing that will fix these problems:
  User fired event to launch the fetch
  Multiple calls to the API

And will get you a Godkänt grade.

However, to get the VG grade you'll need to show multiple properties of the returned data and add something to the API call - unfortunatley the API you have chosen doesn't seem to have multiple properties. You could look at using an API like https://developers.thecatapi.com/view-account/ylX4blBYT9FaoVd6OhvR?report=bOoHBz-8t whic is a little more complex and requires a key, but will return more info to display to the user.


So it's your choice - if you are happy with a G grade please fix the error and resubmit. If you want a VG grade you'll have to extend your code a bit. Please let me know what you will like to do!

*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

Connect to an API ✅

User fired event to launch the fetch ❌

Data is returned and handled efficiently ✅

Display more than one property of the returned data ❌
  In the code only the image is shown

RWD
  Desktop ✅
  Mobile ✅

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Error handling when fetching the data ❌

Append arguments to the request ❌

Multiple calls to the API ❌

Code style ✅
  A few empty lines but nice!