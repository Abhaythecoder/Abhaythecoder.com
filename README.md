<!DOCTYPE html>

  <head>
    <meta charset="UTF-8">
    <title>Name and Age Form</title>
  </head>
  <body>
    <h1>Please enter your name and age</h1>
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name"><br><br>
      <label for="age">Age:</label>
      <input type="number" id="age" name="age"><br><br>
      <input type="submit" value="Submit">
    </form>
    <br><br>
    <p id="response"></p>

    <script>
      // Get the form and response element
      const form = document.querySelector("form");
      const response = document.querySelector("#response");

      // Listen for form submission
      form.addEventListener("submit", function(event) {
        event.preventDefault();

        // Get the values of the name and age inputs
        const name = form.elements.name.value;
        const age = form.elements.age.value;

        // Update the response text to thank the user
        response.innerHTML = `Thank you, ${name}! Your age is ${age}.`;
      });
    </script>
  </body>
</html>
