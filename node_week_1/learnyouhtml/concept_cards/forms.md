# Forms

The HTML `<form>` element creates a form that collects input from the user. A website may require a user's name and credit card information. It asks the user for this information through a form.

Within the form tag, the two main attributes that are used are **action** and **method**.

Action holds the URL of a program that processes the form information.

Method specifies how the form data will be sent. Possible values for method are get and post. Get is used to request data from a source, and Post is used to send data to create or update a resource.

Forms are created with input elements. The tag for input elements is `<input>`. `<input>` has a value `type` that indicates which specific input method is used. Here is a list of commonly used `type` values:

* text: a single-line text field. This is the default value for `type` if one is not specified.

  ```markup
  <form>
      <label for="fname">First name:</label><br>
      <input type="text" id="fname" name="fname"><br>
      <label for="lname">Last name:</label><br>
      <input type="text" id="lname" name="lname">
  </form>
  ```

   First name:  
   
   Last name:  
 

* button: a clickable button

  ```markup
  <input type="button" value="Click Me!">
  ```

* checkbox: a box that can be checked off by the user

  ```markup
  <form>
      <input type="checkbox" id="item1" name="item1" value="Sandwiches">
      <label for="item1">Sandwiches</label><br>
      <input type="checkbox" id="item2" name="item2" value="Pizza">
      <label for="item2">Pizza</label><br>
      <input type="checkbox" id="item3" name="item3" value="Burritos">
      <label for="item3">Burritos</label>
  </form>
  ```

    Sandwiches  
    Pizza  
    Burritos

* **file** - a control that allows the user to select a file

  ```markup
  <form>
      <label for="myfile">Select a file:</label>
      <input type="file" id="myfile" name="myfile">
  </form>
  ```

   Select a file: 

* **password** - a single-line text field whose value is obscured

  ```markup
  <form>
      <label for="username">Username:</label><br>
      <input type="text" id="username" name="username"><br>
      <label for="pwd">Password:</label><br>
      <input type="password" id="pwd" name="pwd">
  </form>
  ```

   Username:  
   
   Password:  
 

* **radio** - a "radio button". Similar to checkboxes in that you are given multiple options, but you can only check off one radio button.

  ```markup
  <form>
      <input type="radio" id="male" name="gender" value="male">
      <label for="male">Male</label><br>
      <input type="radio" id="female" name="gender" value="female">
      <label for="female">Female</label><br>
      <input type="radio" id="other" name="gender" value="other">
      <label for="other">Other</label>
  </form>
  ```

    Male  
    Female  
    Other

* **submit** - a button that submits the form

  ```markup
  <form action="/action_page.php">
      <input type="submit" value="Submit">
  </form>
  ```

