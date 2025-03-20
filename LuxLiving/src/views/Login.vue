<template>
    <nav></nav>
    <form method="post">
        <div class="container">
            <img class="avatar" src="../assets/Profile.jpg" alt="Avatar">
        </div>
        <div class="container">
            <label for="username"></label>
            <input type="text" name="name" placeholder="Enter Username">
            <br>
            <label for="password"></label>
            <input type="password" name="password" placeholder="Enter Password">
            <br>
            <button type="submit">Login</button>
            <label>
                <input checked="checked" type="checkbox">Remember me
            </label>
        </div>
        <div class="container">
            <RouterLink to="/signup"><button class="signupbtn" type="button">Signup</button></RouterLink>
            <RouterLink to="recoveryaccount"><span class="password"><a href="#">Forgot password?</a></span></RouterLink>
        </div>
    </form>
</template>

<script>

</script>

<style>
input[type=text], input[type=password] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

button {
  background-color: #7293bf;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

button:hover {
  opacity: 0.8;
}

.signupbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #04AA6D;
}

.imgcontainer {
  text-align: center;
  margin: 24px 0 12px 0;
}

img.avatar {
  width: 40%;
  border-radius: 50%;
  display: block;
}

.container {
  padding: 16px;
}

span.password {
  float: right;
  padding-top: 16px;
}

@media screen and (max-width: 1395px) {
  span.password {
    display: block;
    float: none;
  }
  .signupbtn {
    width: 100%;
  }
}
</style>