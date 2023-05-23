<template>
    <!-- Don't need "action" as we use JS to handle the action -->
  <form >
    <label>Email</label>
    <input type="email" required>
  </form>
</template>

<script>
export default {

}
</script>

<style>

form {
    max-width: 400px;
    margin: 20px auto;
    background-color: #DDEDFF;
    text-align: left;
    padding: 5rem;
    border-radius: 10px;
    margin: auto;

}

label {
font-family: Arial, Helvetica, sans-serif;
font-size: 1em;
margin: 25px 0 15px;
text-transform: uppercase;
display: inline-block;
}

input {
display: block;
padding: 10px 6px;
width: 100%;
box-sizing: border-box; /*Sizing takes into consideration the borer and  padding*/
border: none;
border-bottom: 3px solid #cfcfcf ;
color: rgb(192, 192, 192);
}


</style>