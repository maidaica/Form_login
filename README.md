# Form_login
// html 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- css -->
    <!-- <link rel="stylesheet" href="main.css"> -->
    <link rel="stylesheet" href="css/login.css">
    <!-- boxIcons -->
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>

</head>
<body>
    <div class="login-box">
        <h2>Please Login</h2>
        <p>Enter your details</p>
        
        <form action="">
            <div class="form-group">
                <label for="email">
                    Email
                </label>
                <i class="bx bxs-user"></i>
                <input type="email" name="" id="" placeholder="Your email">
            </div>
            <!--  -->
            <div class="form-group">
                <label for="password">
                    Password
                </label>
                <i class="bx bxs-lock"></i>
                <input type="password" name="" id="" placeholder="Your password">
            </div>
            <!--  -->

            <a href="#" class="forgot">
                Forgot your password?
            </a> <br>

            <input type="submit" value="Log In">
        </form>

    </div>
</body>
</html>

-------------------------------------------------------------------------------css--------------------------------------------------------------------------------
*{
    margin: 0;
    padding: 0;
    /* border: 0; */
    /* outline: 0; */
    /* box-sizing: border-box; */
    font-family: Arial, Helvetica, sans-serif;
}
body{
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background-image: url('../images/low-poly-grid-haikei.svg');
    background-size: cover;
    animation: move 15s linear alternate infinite;
}
@keyframes move{
    50%{
        background-position: 50%;
    }
}

.login-box{
    width: 400px;
    /* height: min-content; */
    padding: 40px;
    background-color: #fff;
    text-align: center;
    border-radius: 16px;
  
}
.login-box h2{
    font-size: 40px;

}
.login-box p{
    color: #404040;
    margin-top: 5px;
}

form{
    text-align: left;
    margin-top: 30px;
}

form .form-group{
    margin: 18px 0;
}
form .form-group label{
    display: block;
    font-size: 20px;
    
}
form .form-group input{
    width: 100%;
    height: 40px;
    margin-top: 6px;
    padding: 0 0 0 34px;
    border-radius: 10px;   
    font-size: 18px;
    color: #404040;
    
}

form .form-group input:focus{
    border-color: red;
    box-shadow: 0 0 10px red ;
}

form .form-group input:valid{
    border-color: red;
    background-color: #fff;
}

form .form-group i {
    position: absolute;
    color: #404040;
    font-size: 20px;
    transform: translateX(2px) translateY(17px);
}
form .form-group input{
    padding-left: 20px;
}

form .forgot{
    text-decoration: none;
    font-size: 18px;
}

form input[type="submit"]{
    width: 100%;
    margin-top: 15px;
    height: 46px;
    border-radius: 20px;
    color: white;
    background-color: red;
}
