<script setup>
    
</script>
<template>
    <div id="setting-panel">
        <p>Settings</p>
        <!-- expiration-time-input -->
        <div class="expiration-time">
            <label for="expiration-time-input">Expiration time</label>
            <input id="expiration-time-input" type="number" list="time-choice" min="60" step="1" placeholder="Expiration (secs)" name="expiration-time">
            <datalist id="time-choice">
                <option value="60">1min</option>
                <option value="300">5min</option>
                <option value="3600">1hour</option>
                <option value="86400">1day</option>
                <option value="604800">1week</option>
                <option value="2592000">1month</option>
            </datalist>
        </div>
        <!-- password-input -->
        <div class="password">
            <label for="password-input">Password</label>
            <input id="password-input" placeholder="Password" type="text" name="password">
        </div>
        <!-- max-visited-number-input -->
        <div class="max-visited-numer">
            <label for="password-input">Max visited time</label>
            <input id="max-number-input" type="number" min="1" step="1" placeholder="Max visited number" name="max-number">
        </div>
        <!-- language-select -->
        <div class="language">
            <label for="language-select">Language</label>
            <select name="languages" id="language-select">
                <option value="c" selected>C</option>
                <option value="cpp">C++</option>
                <option value="csharp">C#</option>
                <option value="java">Java</option>
                <option value="python">Python</option>
                <option value="js">JS</option>
                <option value="go">Golang</option>
            </select>
        </div>
    </div>
</template>
<style scoped>
#setting-panel{
    display: flex;
    flex-direction: column;
    align-items: left;

    width: 70%;
    margin:20px;

    box-sizing: border-box;
    /* border: 1px solid black; */
}
#setting-panel>p{
    padding: 5px;
    font-size: 40px;
    margin:10px;
    padding-bottom:10px;
    border-bottom: 2px solid black;
}
#setting-panel>div{
    display: flex;
    flex-direction:column-reverse;

    margin:10px;
    overflow: hidden;
}
#setting-panel>div>label{
    margin-top:10px;
    margin-left: 2px;

    height:15px;

    font-size: 10px;
    font-weight: 100;
    font-family:Arial, Helvetica, sans-serif;
    text-align: left;
}
#setting-panel>div>input,select{
    width: 300px;
    height: 30px;
}
</style>

