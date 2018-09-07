Panda Exercise 1

//QUESTION 1
Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.

ANSWER 1
var img = document.body.querySelector('img'); img.src = ('https://placebear.com/400/400');

//QUESTION 2
Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

ANSWER 2
var sky_img = document.body.querySelector('#left-image img'); sky_img.src = ('https://placebear.com/325/225');

//QUESTION 3
Select the heading that says "Panda the Bear" and change it to your own name.

ANSWER 3
var h1 = document.body.querySelector('h1'); h1.innerText = 'Tyler';

//QUESTION 4
Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

ANSWER 4
var h3 = document.body.querySelector('#employment h3'); h3.innerText = 'Fuck DOM';

//QUESTION 5
Change the colour of the body.

ANSWER 5  
var body = document.body.style.backgroundColor = "blue";

//QUESTION 6
Change the colour of each element using the highlight class. Use a for loop to do this.

ANSWER 6
var highlights = document.querySelectorAll(".highlight"); highlights.forEach(function(highlight) { highlight.style.backgroundColor = "red"; });

//QUESTION 7
Change the font family of the h1 to 'monospace'.

ANSWER 7
var font = document.body.querySelector('h1'); font.style.fontFamily = "monospace";

//QUESTION 8
Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

ANSWER 8
var placeholder_name =
document.querySelector('#name'); placeholder_name.value = 'Tyler P';

//QUESTION 9
Change the placeholder attribute of the message field to "state your business".

ANSWER 9
var placeholder_msg =
document.querySelector('#message'); placeholder_msg.value = 'state your business';

//QUESTION 10
Give the name field a "value" attribute of "your nemesis".

ANSWER 10
var placeholder_name =
document.querySelector('#name'); placeholder_name.placeholder = 'your nemesis'; placeholder_name.value = 'Tyler P';

//QUESTION 11
Change the value attribute of the email field to "koalathebear@gmail.com".

ANSWER 11
var placeholder_email =
document.querySelector('#email'); placeholder_email.value = 'koalathebear@gmail.com';

//QUESTION 12
Change the value of the submit button on the contact form to "En garde!".

ANSWER 12
var submit =
document.querySelector('#submit'); submit.value = 'en garde';

//QUESTION 13
We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

ANSWER 13
var disable_button = document.querySelector('#submit'); submit.disabled = true;

//QUESTION 14
We should help Panda protect their privacy by erasing their personal details from the sidebar.

ANSWER 14
var bio_hide =
document.querySelector('ul'); var parent = bio_hide.parentElement; parent.removeChild(bio_hide);

//QUESTION 15
Find a way to select the round icons in the sidebar and then change their colour

ANSWER 15
var btn = document.querySelectorAll(".action-icon-bg"); btn.forEach(function(btn) { btn.style.backgroundColor = 'blue'; });

-------------------------------------------------------------------

Panda Exercise 2

//DELETING
QUESTION:
Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a javaScript function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but parentNode might be useful when it comes to selecting the right element)


ANSWER:
var timeTravel = document.querySelector('.bar-default:nth-of-type(4)'); timeTravel.parentNode.removeChild(timeTravel);

//CLONING
var pikachu = document.body.querySelector('#right-image img'); var pikaclone = pikachu.cloneNode(); 
