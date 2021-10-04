<template>
<div class="container">
    <form @submit.prevent="formSubmit">
        <select name="type" id="type" v-model="type" required>
            <option value="buy">ON SALE</option>
            <option value="rent">FOR RENT</option>
        </select>

        
        <select name="bed" id="bed" v-model="bed" required>
            <option value="" disabled selected hidden>Bedrooms</option>
            <option value="1">One</option>
            <option value="2">Two</option>
            <option value="3">Three</option>
            <option value="4">Four or more</option>
        </select>

        <select name="bath" id="bath" v-model="bath" required>
            <option value="" disabled selected  hidden>Bathrooms</option>
            <option value="1">One</option>
            <option value="2">Two</option>
            <option value="3">Three</option>
        </select>

        <input type="number" name="min" min="0" id="min" placeholder="Minimum price ($K)" v-model="min" required>
        <input type="number" name="max" min="0" id="max" placeholder="Maximum price ($K)" v-model="max" required>


    <div class="message"><p>I want to {{type || '__'}} a house with {{bed || '__'}} bedrooms and {{bath || '__'}} bathrooms. My budget is between {{min || '__'}} and {{max || '__'}} thousand dollors.</p></div>
        <button type="submit" class="search-btn">Search</button>

        <p v-if="error" class="error">Bro wtf? you minimum budget can not be more than your maximum</p>
    </form>
</div>
</template>

<script>
export default {
    name: "Searchform",
    data(){
        return {
            type: 'buy',
            min: '',
            max:'',
            bed:'',
            bath:'',
            error: false,
        }
    },
    methods: {
        formSubmit(){
            if(this.min > this.max){
                this.error = true;
            }else{
                this.error = false
                alert('idk how to do backend so just pretend i submitted this shit.')
            }
        }
    }
}
</script>

<style>
    .container {
        background-color: #fff;
        padding: 20px 50px;

    }
    select, input, button, .message {
        background-color: #FFF0CB;
        padding: 20px;
        margin: 10px;
        border: 2px solid rgba(2, 55, 135, 0.5);
        outline: none;
        font-size: 16px;
    }
    select:focus, input:focus, button:focus{
        border:  2px solid rgb(2, 55, 135);
    }
    .search-btn {
        padding: 20px 50px;
        background-color: #FFC839;
        
    }
    div.message{
        background-color: #fff;
        border:  2px solid rgba(2, 55, 135, 0.3);
    }
    .error{
        color: red;
        font-size: 20px;
        display: inline-block;
        margin-left: 20px;
    }
</style>