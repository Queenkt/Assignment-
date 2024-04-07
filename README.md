
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Web Page</title> <style> /* CSS Styles */ body {font-family: Arial, sans-serif; margin: 0;padding: 20px;}h1, h2, h3 {color: green;}p { color: purple; }
container{ max-width: 800px; margin: 0 auto; background-color: blue;padding: 20px; border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0,0.1)}
calculator {display: grid;grid-template-columns: repeat(4, 1fr); grid-gap: 10px;
  } calculator button {padding: 15px; font-size: 20px; background-color: white;
color: white; border: none; border-radius: 5px; cursor: pointer;} calculator button:hover {background-color: blue;}result{grid-column: span 4;
padding: 10px; text-align: right; background-color: blue; border: 1px solid ;border-radius: 5px;}
</style>
</head>
<body>
  <div class="container">
  <h1>Hi I am Oyewole Kofoworola</h1>
  <p>I am a future Backend developer and a future lawyer.</p>

  <h2>Summary</h2>
  <p>My goal for this diploma course is to learn and and to be able to incorporate what i have learnt to my field of study to inprove it.</p>

  <h2>Education</h2>
  <p>I have a WASSCE Certificate.<p>
  <p> I am currently doing my undergraduate studies.<p>

  <h2>Job Experiences</h2>
  <p>I am currently unemployed <p>

  <h2>Hobby</h2>
  <p>My hobbies are reading, sleeping, watching movies and playing board games<p>

  <h2>Other Skills</h2>
  <p>Proficiency in Microsoft word <p>
  <h2>Calculator</h2>
<table class="calculator" >
    <tr>
      <td colspan="3"> <input class="display-box" type="text" id="result" disabled /> </td>
      <td> <input type="button" value="C" onclick="clearScreen()" id="btn" /> </td>
    </tr>
    <tr>
      <td> <input type="button" value="1" onclick="display('1')" /> </td>
      <td> <input type="button" value="2" onclick="display('2')" /> </td>
      <td> <input type="button" value="3" onclick="display('3')" /> </td>
      <td> <input type="button" value="/" onclick="display('/')" /> </td>
    </tr>
    <tr>
      <td> <input type="button" value="4" onclick="display('4')" /> </td>
      <td> <input type="button" value="5" onclick="display('5')" /> </td>
      <td> <input type="button" value="6" onclick="display('6')" /> </td>
      <td> <input type="button" value="-" onclick="display('-')" /> </td>
    </tr>
    <tr>
      <td> <input type="button" value="7" onclick="display('7')" /> </td>
      <td> <input type="button" value="8" onclick="display('8')" /> </td>
      <td> <input type="button" value="9" onclick="display('9')" /> </td>
      <td> <input type="button" value="+" onclick="display('+')" /> </td>
    </tr> <tr>
      <td> <input type="button" value="0" onclick="display('0')" /> </td>
      <td> <input type="button" value="=" onclick="calculate()" id="btn" /> </td>
      <td> <input type="button" value="%" onclick="display('%')" /> </td>
      <td> <input type="button" value="*" onclick="display('*')" /> </td>
    </tr>
</table>
<form>

  <h2>Contact Me</h2>
  <form id="contactForm" action="#" method="post" onsubmit="return validateForm()">
    <label for="name">Name:</label><br>
    <input type="text" id="name" name="name" required><br>

   <label for="email">Email:</label><br>
    <input type="email" id="email" name="email" required><br>

  <label for="message">Message:</label><br>
    <textarea id="message" name="message" required></textarea><br>

   <label for="priority">Priority:</label><br>
    <select id="priority" name="priority" required>
          <option value="" disabled selected>Select Priority</option>
      <option value="low">Low</option>
      <option value="medium">Medium</option>
      <option value="high">High</option>
    </select><br>

 <input type="submit" value="Submit">
  </form>
</div>
<script>
function validateForm() {
  var name = document.getElementById("name").value;
  var email = document.getElementById("email").value;
  var message = document.getElementById("message").value;
  var priority = document.getElementById("priority").value;
  if (name == "" || email == "" || message == "" || priority == "") {
    alert("All fields must be filled out");
    return false;
  }
}
</script>
