<template>
    <nav></nav>
    <form>
        <div class="container">
            <h1>Signup</h1>
            <p>Create an account</p>
            <br>
            <label for="email"><b>Email: </b></label>
            <input name="email" type="text" placeholder="Enter Email">
            <br>
            <label for="password"><b>Password: </b></label>
            <input name="password" type="password" placeholder="Enter Password">
            <br>
            <label for="confirmPassword"><b>Confirm password: </b></label>
            <input name="confirmPassword" type="password" placeholder="Confirm Password">
            <br>
            <label>
                <input checked="checked" type="checkbox" style="margin-bottom: 15px;">Remember me
            </label>
            <p>By creating an account you agree to our<a href="#" style="color: dodgerblue;">Terms & Privacy</a>.</p>

            <div>
                <RouterLink to="/login"><button class="loginbtn" type="submit">Log in</button></RouterLink>
                <button class="signupbtn" type="submit">Sign up</button>
            </div>
        </div>
    </form>
</template>

<script>
import Footer from './Footer.vue';
export default {
    name: 'Signup'
}
</script>

<style>
body {font-family: Arial, Helvetica, sans-serif;}
* {box-sizing: border-box}

input[type=text], input[type=password] {
  width: 100%;
  padding: 7px;
  margin: 2px;
  display: inline-block;
  border: none;
  background: #f1f1f1;
}

input[type=text]:focus, input[type=password]:focus {
  background-color: #ddd;
  outline: none;
}

hr {
  border: 1px solid;
  margin-bottom: 25px;
}

button {
  background-color: #04AA6D;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
  opacity: 0.9;
}

button:hover {
  opacity:1;
}

.loginbtn {
  padding: 14px 20px;
  background-color: #7293bf;
}

.loginbtn, .signupbtn {
  float: left;
  width: 50%;
}

.container {
  padding: 16px;
}

@media screen and (max-width: 300px) {
  .cancelbtn, .signupbtn {
     width: 100%;
  }
}
</style>