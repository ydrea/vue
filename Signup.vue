<template>
<form @submit.prevent="handleSubmit"> 
    <label> email: </label>
    <input type="email" required
    v-model="email"
    >

    <label>Password:</label>
    <input type="password" required
    v-model="password"
    >

    <label>Gender</label>
    <select v-model="gender"> 
        <option value="null">   </option>
        <option value="female"> F </option>
        <option value="male"> M </option>
    </select>

    <div class="terms"> 
    <label>Accept terms and conditions</label>
        <input type="checkbox" required
        v-model="terms"
        >
    </div>

<div class="submit"> 
    <button>Create an account</button>
</div>

</form>
</template>

<script>
export default {
    data () {
        return {
            email: '',
            password: '',
            gender: '',
            terms: false,
        }
    }

}
</script>

<style>
  form {
    max-width: 420px;
    margin: 30px auto;
    background: white;
    text-align: left;
    padding: 40px;
    border-radius: 10px;
  }
  label {
    color: #aaa;
    display: inline-block;
    margin: 25px 0 15px;
    font-size: 1.6em;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: bold;
  }
  input, select {
    display: block;
    padding: 10px 6px;
    width: 100%;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    color: #555;
  }
    .terms {
    display: inline;
    width: 146px;
    margin: 0 10px 0 0;
    position: relative;
    top: 2px;
    text-transform: lowercase; 
    font-size: 0.6em;
  }
  button {
    background: #0b6dff;
    border: 0;
    padding: 10px 20px;
    margin-top: 20px;
    color: white;
    border-radius: 20px;
  }
  .submit {
    text-align: center;
  }
  .error {
    color: #ff0062;
    margin-top: 10px;
    font-size: 0.8em;
    font-weight: bold;
  }
</style>