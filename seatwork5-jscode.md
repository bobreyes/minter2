Greeting Card Messages Array

1. Think about how you could test whether the message in each case is a Christmas message. What string is present in all of those messages, and what method could you use to test whether it is present?

2. You'll then need to write a conditional test of the form operand1 operator operand2. Is the thing on the left equal to the thing on the right? Or in this case, does the method call on the left return the result on the right?

Hint: In this case it is probably more useful to test whether the method call isn't equal to a certain result.


-=-=-=-=-=-=-=-=-=-=-=-= JavaScript Code Begin -=-=-=-=-=-=-=-=-=-=-=-=

var list = document.querySelector('.output ul');
list.innerHTML = '';
var greetings = ['Happy Birthday!',
                 'Merry Christmas my love',
                 'A happy Christmas to all the family',
                 'You\'re all I want for Christmas',
                 'Get well soon'];

for (var i = 0; i < greetings.length; i++) {
  var input = greetings[i];
  // Your conditional test needs to go inside the parentheses
  // in the line below, replacing what's currently there
  if (greetings[i]) {
    var result = input;
    var listItem = document.createElement('li');
    listItem.textContent = result;
    list.appendChild(listItem);
  }
}

-=-=-=-=-=-=-=-=-=-=-=-= JavaScript Code End -=-=-=-=-=-=-=-=-=-=-=-=

3. Upload the solution (code) to your GitHub account under /minter2/seatwork5
