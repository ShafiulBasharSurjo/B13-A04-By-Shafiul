1. What is the difference between getElementById, getElementByClassNmae, and querySelector / querySelectorAll?
 Ans : getElementById is used to work with only one element. It selects an element by it's id and returns the said element or null.

 getElementByClassNmae works with classes. It selects all the elements with a certain similar class and retuens a live HTMl collection. Example: document.getElementByClassNmae('btn').

 querySelector returns the first element that matches with the given class. Example : document.querySelector("totalcount").

 querySelectorAll returns all the elements that matches with the given class as a static nodelist. Example : document.querySelectorAll('data-tab').


2. How do you create and insert a new element into the DOM?
  Ans: 
  const pawn = document.createElement('div');

  pawn.textContent = 'Hi';
  pawn.classList.add('pawn');

  document.getElementById('cards').appendChild(pawn);

3. What is Event Bubbling? And how does it work?
   Ans: Event Bubbling is the way that events travel through he DOM.

   When an event happens on an element it not only triggers that sspecific element but also bubbles up through every parent element all the way to the document.

4. What is Event Delegaton in JavaScript? Why is it useful?
 
 Ans: By using Event Bubbling we just need to add one listener in the parent class and let bubbling do the work.

   If we use Event Bubbling we don't have to add an event listener to every element seperately.

5. What is the difference between preventDefault() and stopPropagation() methods?

 Ans: preventDefault: It stops the browser from doing it's usual behaiviour. Like opening a link from URL.

 stopPropagation: This stops the event from bubbling up the DOM tree.