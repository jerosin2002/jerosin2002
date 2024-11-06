<!DOCTYPE html> 
<html lang="en"> 
<head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Signup Form</title> 
    <style>         body {             font-family: Arial, sans-serif;             background-color: lightblue; 
        } 
 
        .container {             max-width: 400px;             margin: 50px auto;             padding: 20px;             background-color: white;             border-radius: 8px;             box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1); 
        } 
         h2 {             text-align: center; 
        } 
         label {             display: block;             margin-top: 10px; 
        } 
 
        input[type="text"],         input[type="password"],         input[type="tel"],         input[type="email"],         input[type="date"],         select {             width: 100%;             padding: 8px;             margin: 5px 0;             box-sizing: border-box;         } 
 
        input[type="radio"] {             margin-right: 5px; 
        } 
 
        .signup-btn {             width: 100%;             padding: 10px;             background-color: orange;             border: none;             color: white;             font-size: 16px;             cursor: pointer;             border-radius: 5px; 
        } 
 
        .signup-btn:hover { 
            background-color: darkorange; 
        } 
    </style> 
</head> 
<body> 
    <div class="container"> 
        <form action="signup.php" method="POST" enctype="multipart/formdata"> 
            <h2>Signup</h2> 
             
            <label for="name">Name:</label> 
            <input type="text" id="name" name="name" required> 
 
            <label for="username">Username:</label> 
            <input type="text" id="username" name="username" required> 
 
            <label for="password">Password:</label> 
            <input type="password" id="password" name="password" required> 
 
            <label for="mobile">Mobile No:</label> 
            <input type="tel" id="mobile" name="mobile" required> 
 
            <label for="email">Email:</label> 
            <input type="email" id="email" name="email" required> 
 
            <label for="country">Country:</label> 
            <select id="country" name="country" required> 
                <option value="">Select Country</option> 
                <option value="India">India</option> 
                <option value="USA">USA</option> 
                <!-- Add more countries as needed --> 
            </select> 
 
            <label for="state">State:</label> 
            <select id="state" name="state" required> 
                <option value="">Select State</option> 
                <option value="Tamil Nadu">Tamil Nadu</option> 
                <option value="California">California</option> 
                <!-- Add more states as needed --> 
            </select> 
 
            <label for="district">District:</label> 
            <input type="text" id="district" name="district" required> 
 
            <label for="address">Address:</label> 
            <input type="text" id="address" name="address" required> 
 
            <label for="dob">Date of Birth:</label>             <input type="date" id="dob" name="dob" required> 
 
            <label>Gender:</label> 
            <input type="radio" id="male" name="gender" value="Male" required> 
            <label for="male">Male</label> 
            <input type="radio" id="female" name="gender" value="Female" required> 
            <label for="female">Female</label> 
 
            <label for="profile_image">Profile Image:</label>             <input type="file" id="profile_image" name="profile_image" required> 
 
            <button type="submit" class="signup-btn">Signup</button> 
        </form> 
    </div> 
</body> 
</html> 
