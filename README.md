<!DOCTYPE html>
<html lang="en">
<head>
 <link rel="shortcut icon" href="favicon.ico" type="image/x-icon" />
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>N-CO OS 1.0 Beta</title>
 <style>
 body {
   font-family: Arial, sans-serif;
   color: black; /* Default text color */
 }

 .container {
   max-width: 400px;
   margin: 0 auto;
   padding: 20px;
   border: 1px solid #ccc;
   border-radius: 5px;
 }

 .btn {
   display: block;
   width: 100%;
   padding: 10px;
   margin-top: 10px;
   text-align: center;
   background-color: #007bff;
   color: #fff;
   border: none;
   border-radius: 5px;
   cursor: pointer;
 }

 .btn:hover {
   background-color: #0056b3;
 }

 h2 {
   color: grey;
   display: inline;
 }

 .popup {
   display: none;
   position: absolute;
   border: 1px solid #ccc;
   border-radius: 5px;
   background-color: #f9f9f9;
   padding: 10px;
   z-index: 1000;
   cursor: grab;
 }

 .dropdown {
   position: relative;
   display: inline-block;
 }

 .dropdown-select {
   background-color: #007bff;
   color: #fff;
   padding: 10px;
   border: none;
   border-radius: 5px;
   cursor: pointer;
 }

 .dropdown-content {
   display: none;
   position: absolute;
   background-color: #f9f9f9;
   min-width: 160px;
   box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
   z-index: 1000;
 }

 .dropdown-content button {
   display: block;
   width: 100%;
   padding: 10px;
   text-align: left;
   background-color: transparent;
   color: black;
   border: none;
   cursor: pointer;
 }

 .dropdown-content button:hover {
   background-color: #ddd;
 }

 .dropdown:hover .dropdown-content {
   display: block;
 }
 </style>
</head>
<body>
  <div class="container">
    <h2>Welcome to N-CO OS 1.0 Beta</h2>
    <button class="btn">Click Me</button>

    <div class="dropdown">
      <button class="dropdown-select">Select Option</button>
      <div class="dropdown-content">
        <button>Option 1</button>
        <button>Option 2</button>
        <button>Option 3</button>
      </div>
    </div>
  </div>

  <div class="popup">
    <p>This is a popup!</p>
  </div>

  <script>
    // Example JavaScript for toggling popup visibility
    document.querySelector('.btn').addEventListener('click', function() {
      let popup = document.querySelector('.popup');
      popup.style.display = popup.style.display === 'none' ? 'block' : 'none';
    });
  </script>
</body>
</html>
