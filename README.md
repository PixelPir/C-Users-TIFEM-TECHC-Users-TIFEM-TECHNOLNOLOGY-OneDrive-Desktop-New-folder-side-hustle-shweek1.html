<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Simple FOrm</title>
    <link rel="stylesheet" href="style.css">
    <script>
        function validateForm() {
            var x = document.forms ["myForm"] ["nname", "email", "phone", 
            "password", "select" ] . value;
            if (x == "") {
                alert("Fill the empty block");
                return false;
            }

        }
    </script>
</head>
<body>
    
    <div class="center">
        <h1>Input Your Details</h1>
        <form action="" form name="myForm"
        onsubmit="return validateForm()"
        method="post" required>
            <label for="name">Name</label>
            <input type="text" id="fullname" name="name" placeholder="Your Full Name..." required>

            <label for="email">Email Address</label>
            <input type="email"  id="email" name="email" placeholder="Your Email..." required>

            <label for="Phone">Phone Number</label>
            <input type="tel" id="Phone" name="Phone" placeholder="Your Phone Number..." required>

            
            <label for="gender">Gender</label>
            <select name="gender" id="gender" required>
                <option value="">select Gender</option>
                <option value="Male">Male</option>
                <option value="Female">Female</option>
                <option value="Other">Other</option>
            </select>

            <label for="password">Password</label>
            <input type="password" id="password" name="Password" placeholder="Your Password..." required>

            <button > Submit</button>


        </form>
    </div>

</body>
