<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: black;
}

* {
  box-sizing: border-box;
}

/* Add padding to containers */
.container {
  padding: 16px;
  text-align: center;
  
}

/* Full-width input fields */
input[type=text], input[type=password] {
  width: 50%;
  padding: 15px;
  margin: 2px 0 5px 0;
  display: inline-block;
  border: none;
  background: #f1f1f1;
}

input[type=text]:focus, input[type=password]:focus {
  background-color: #ddd;
  outline: none;
}

/* Overwrite default styles of hr */
hr {
  border: 1px solid skyblue;
  margin-bottom: 25px;
  color: skyblue;
}

/* Set a style for the submit button */
.registerbtn {
  background-color: rgb(0,128,255);
  color: white;
  padding: 16px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
  opacity: 0.9;
}

.registerbtn:hover {
  opacity: 1;
}

/* Add a blue text color to links */
a {
  color: dodgerblue;
}

/* Set a grey background color and center the text of the "sign in" section */
.signin {
  background-color: #f1f1f1;
  text-align: center;
}
</style>
</head>
<body>

<form action="/action_page.php">
  <div class="container">
    <h1 style="color: white;">COVID 19 VACCINE REGISTRATION</h1>
    <p>Please fill in this form to create an account.</p>
    <hr style="margin-top: -20px;">

    <label for="email"><b>Name</b></label><br>
    <input type="text" placeholder="Enter Name as in Aadhaar Card" name="email" id="email" required><br>

    <label for="psw"><b>Aadhar Number</b></label><br>
    <input type="password" placeholder="Enter 12 digit Aadhaar Number" name="psw" id="psw" required><br>

    <label for="psw-repeat"><b>Create Password</b></label><br>
    <input type="password" placeholder="Enter Password" name="psw-repeat" id="psw-repeat" required><br>
     <label for="psw-repeat"><b>Repeat Password</b></label><br>
    <input type="password" placeholder="Repeat Password" name="psw-repeat" id="psw-repeat" required>
    <hr>

    <button type="submit" class="registerbtn">Register</button>
  </div>
  
  <div class="container signin">
    <p>Already have an account? <a href="#">Log IN</a>.</p>
  </div>
</form>

</body>
</html>
