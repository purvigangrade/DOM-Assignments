# DOM Assignment 1
---
## Task1 
-------
Adding "Hire Me" at the last of Menu and replacing "Projects" with "Contacts"
## Output Image
---
![Output Image](./DOM%20Assignment%202.0%201%2C2%2C3/firstAssignmentImage/task1Output.png)

```JavaScript
//To add "HIRE ME" to the list
const element = document.querySelector("ul") 
const list = document.createElement("li")
list.textContent = "Hire Me"
element.appendChild(list);

//To replace "Contacts" with "Projects"
const element = document.querySelector("ul").children[2]
const l1 = document.createElement("li")
l1.textContent = "Projects"
element.replaceWith(l1);
```
----
## Task2 
-------
Replacing the placeholder with "Search My Project" text"
## Output Image
---
![Output Image]([./firstAssignmentImage/task2Output.png](https://github.com/purvigangrade/DOM-Assignments/blob/main/DOM%20Assignment%202.0%201,2,3/firstAssignmentImage/task2Output.png?raw=true))

```JavaScript
let select = document.querySelector(".search-field input");
select.placeholder = "Search My project"
```
----
## Task3
-------
Changing the span elements
## Output Image
---
![Output Image](./firstAssignmentImage/task3Output.png)

```JavaScript
let element = document.querySelector("ul").children[2];
element.innerHTML = "<a>Projects</a>";

let spanElement = document.querySelector(".hero-left-section p");
let freelancer = spanElement.children[2];
freelancer.innerHTML = "<span>an Employee</span"

spanElement.children[4].innerHTML = "<span>iNeuron Intelligence Pvt Ltd.</span>"
```
---
## Task4
-------
Add the Image
## Output Image
---
![Output Image](./firstAssignmentImage/task4Output.png)

```JavaScript
let image = document.querySelector(".hero-right-section img")
image.innerHTML = "<img src="https://hiteshchoudhary.com/static/a8d73d1aac4c79e9bb689640e6090367/2eaab/person-image.jpg"/>
```
---
## Task5
-------
Add the support me button
## Output Image
---
![Output Image](./firstAssignmentImage/task5Output.png)

```JavaScript
let element = document.querySelector("ul").children[2];
element.innerHTML = "<a>Projects</a>";

let element = document.querySelector(".hero-right-section-btns")
let btn = document.createElement("button")
btn2.textContent = "Support Me"
element.appendChild(btn2)
```
---
# DOM Assignment 2
---
## Task1
-------
Add the background color to all H3
## Output Image
---
![Output Image](./secondAssignmentImage/task1Output.png)

```JavaScript
let element1 = document.querySelectorAll(".accordian")
let h3array = Array.from(element4);
for (let i=0; i<= h3array.length; i++){
    h3array[i].style.backgroundColor = "#b4d3d6"
}
```
## Task2 
-------
Add one more column of skills
## Output Image
---
![Output Image](./secondAssignmentImage/task2Output.png)

```JavaScript
const tag = `
<h3>Skills</h3>
<p>I posses a very good command over the Full Stack Development technologies like MERN which can be seen in my work over the Github</p>
`

const newDiv = document.createElement("div")
newDiv.className = "accordian"
newDiv.innerHTML = tag
let select = document.querySelector(".accordian-wrapper")
select.appendChild(newDiv);
```
----
# DOM Assignment 3
---
## Task1
-------
Add the placeholders
## Output Image
---
![Output Image](./thirdAssignmentImage/task1Output.png)

```JavaScript
//User Output Board
let element = document.querySelector(".enterName")
element.placeholder = "FSJS 2.0"
let eMail = document.querySelector(".enterMail")
eMail.placeholder = "fsjs@ineuron.ai"
let Message = document.querySelector(".enterMessage")
Message.placeholder = "Hello World"

//User Input Board
let UserName = document.querySelector(".userName")
UserName.placeholder = "FSJS 2.0"
let Useremail = document.querySelector(".userEmail")
Useremail.placeholder = "fsjs@ineuron.ai"
let UserMessage = document.querySelector(".userMessage")
UserMessage.placeholder = "Hello World"
```
---
# DOM Assignment 4
---
## Task1
-------
Change the CSS as per the output image
## Output Image
---
![Output Image](./04_DOM%20Project/04_DOM%20Project/Output/DOM%20P1%20SS.png)

```JavaScript
let select = document.querySelector(".slide-container");
select.style.flexWrap = "nowrap"


let clash = document.querySelectorAll(".clash-card");
clash.forEach(function(hold){hold.style.width = "240px"});

let clashs = document.querySelectorAll(".clash-card__image");
clashs.forEach(function(holds){holds.style.height = "180px"});

let font = document.querySelectorAll(".stat");
font.forEach(function(ls){ls.style.fontSize = "15px"});

let padd = document.querySelectorAll(".one-third");
padd.forEach(function(ls){
    ls.style.padding = "12px 8px"
    ls.style.color = "White"
});

document.querySelector(".clash-card__unit-stats--barbarian").style.backgroundColor = "#ec9b3b";
document.querySelector(".clash-card__unit-stats--archer").style.backgroundColor = "#ee5487";
document.querySelector(".clash-card__unit-stats--giant").style.backgroundColor = "#f6901a";
document.querySelector(".clash-card__unit-stats--goblin").style.backgroundColor = "#82bb30";
document.querySelector(".clash-card__unit-stats--wizard").style.backgroundColor = "#4facff";

let size = document.querySelectorAll(".clash-card__unit-description");
size.forEach(function(ls){
    ls.style.padding = "12px 8px"
    ls.style.fontSize = "12px"
});

let sele = document.querySelectorAll(".clash-card div:nth-child(3)");
sele.forEach(function(sos){sos.style.fontSize = "20px"})

document.querySelector(".archer div:nth-child(3)").innerHTML = "The Archer";
document.querySelector(".goblin div:nth-child(3)").innerHTML = "The Goblin";

document.querySelector(".clash-card__image--barbarian img").style.width = "320px";
document.querySelector(".clash-card__image--archer img").style.width = "320px";
document.querySelector(".clash-card__image--giant img").style.width = "280px";
document.querySelector(".clash-card__image--goblin img").style.width = "300px";
document.querySelector(".clash-card__image--wizard img").style.width = "280px";
```
----
# DOM Assignment 5
-------
Add the Button in the navbar, Add one more card, Change the color of text in all the cards
## Output Image
---
![Output Image](./05_DOM%20Project/05_DOM%20Project/Output/DOM%20P2%20SS.png)

```JavaScript
//Add the Button in the navbar
let element = document.querySelector(".nav-center").children[2]
let btn = document.createElement("a")
btn.className = "btn"
btn.textContent = "Pro Subscription"
element.appendChild(btn)

//Add one more card
let reciepes = document.querySelector(".recipe-gallery")
let element = document.createElement("div")
element.className="card"
reciepes.appendChild(element)
element.innerText = "add 6th card here"
element.style.fontSize="25px"
element.style.fontWeight="Bold"

//Change the color of text in all the cards
let textcolor1 = document.querySelectorAll(".recipe-text");
    for(let i=0; i<textcolor1.length;i++)
    {
        textcolor1[i].style.color = "#8a2be2"
    }
```
# DOM Assignment 6
-------
## Task1
---
Change the logo
## Output Image
---
![Output Image](./06_DOM%20Project/06_DOM%20Project/Output/DOM%20P3%20SS-1.png)

```JavaScript
//Add the Button in the navbar
let logoheader = document.querySelector("header");
let logo = `
<img src="https://ineuron.ai/images/ineuron-logo.png">
`
logoheader.innerHTML = logo;

//OR

document.querySelector("header img").src = "https://ineuron.ai/images/ineuron-logo.png"
```
---
## Task2
---
Change the dollar amount from 4 to 10
## Output Image
---
![Output Image](./06_DOM%20Project/06_DOM%20Project/Output/DOM%20P3%20SS-2.png)

```JavaScript
document.querySelector(".app_price span").innerText = "$10"
```
---
# DOM Assignment 7
-------
## Task1
---
Remove the languages that have 2.0 in their name
## Output Image
---
![Output Image](./DOM%20P7/DOM%20P7/ass7.1-after.png)

```JavaScript
let courses = document.querySelector(".main__languages").getElementsByTagName("a")
courses[1].remove();
courses[2].remove();
courses[3].remove();
courses[4].remove();
courses[5].remove();
```
---
## Task2
---
Adding new element as warning and replacing the placeholder
## Output Image
---
![Output Image](./DOM%20P7/DOM%20P7/ass7.2-after.png)

```JavaScript
document.querySelector(".main__form-input").placeholder = "iNeuron"

let newElement = document.createElement("div")
newElement.textContent = "After Writing the text submit the form"
newElement.style.fontSize = "22px"
newElement.style.backgroundColor = "red"
newElement.style.marginBlock = "20px"
newElement.style.paddingBlock = "20px"
newElement.style.marginInline = "20px"
newElement.style.color = "white"
newElement.style.fontWeight = "Bold"
newElement.style.fontFamily = "Poppins"
newElement.style.borderRadius = "5px"

document.querySelector(".main__form").appendChild(newElement);
```
---
# DOM Assignment 8
-------
## Task1
---
Add the scroll bar at the side
## Output Image
---
![Output Image](./DOM%20P8/DOM%20P8/ass8.1-after.png)

```JavaScript
let element = document.querySelector(".col-lg-4")
element.style.overflow = "scroll"
element.style.border = "2px solid red"
```
-------
## Task2
---
Change in background Color
## Output Image
---
![Output Image](./DOM%20P8/DOM%20P8/ass8.2-after.png)

```JavaScript
document.body.style.background =  "white"
```
---
## Task2
---
Add Hamburger
## Output Image
---
![Output Image](./DOM%20P8/DOM%20P8/ass8.3-after.png)

```JavaScript
let accordian = document.querySelector(".navbar-toggler");
  accordian.addEventListener("click", () => {
    let select = document.querySelector(".collapse");
    if (select.style.display === "block") {
      select.style.display = "none";
    } else {
      select.style.display = "block";
    }
  });
```
---
# DOM Assignment 9
-------
## Task1
---
Chane the color of H1
## Output Image
---
![Output Image](./DOM%20P9/DOM%20P9/ass9.1-after.png)

```JavaScript
let element = document.querySelector(".caption .title")
element.style.color = "red"
```
---
## Task2
---
Chane the color of Add to card button
## Output Image
---
![Output Image](./DOM%20P9/DOM%20P9/ass9.2-after.png)

```JavaScript
document.querySelector(".add-to-cart").style.backgroundColor = "red"
```
