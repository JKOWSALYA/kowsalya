//# kowsalya
(function () {
var names = ["Yaakov", "John", "Jen", "Jason", "Paul", "Frank", "Larry", "Paula", "Laura", "Jim"];

  // STEP 10:
  for (var i =0; i < names.lenght; i++) {

  // STEP 11:
  var firstLetter = names[i].charAt(0).toLowerCase();

  // STEP 12:
  if (firstLetter === 'j') {
    byeSpeaker.speak(names[i]);
  } else {
    helloSpeaker.speak(names[i]);
  }
}

})();
// STEP 2:
(function (window) {
	// STEP 3:
	var helloSpeaker = {};
	var speakWord = "Hello";
	// STEP 4:
	helloSpeaker.speakWord = function () {
	  console.log(speakWord + " " + name);
	}
	// STEP 5: 
	window.helloSpeaker = helloSpeaker;
})(window);
// STEP 6:
(function (window) {
	// STEP 7: 
	var byeSpeaker = {};
	var speakWord = "Good Bye";
	// STEP 8:
	byeSpeaker.speakWord = function () {
	  console.log(speakWord + " " + name);
	}
	// STEP 9:
	window.byeSpeaker = byeSpeaker;
})(window);
