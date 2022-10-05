<script setup>
    
</script>
<template>
    <div id="uploaded-panel" class="visible">
        <p>Uploaded</p>
        <div class="copy-text">
            <div class="text-group">
                <input id='uploaded-url' type='text' class='readonly-text' readonly>
            </div>
            <div class="button-group">
                <button id="copy-button" class='button'>Copy</button>
            </div>
        </div>
        <label>Url</label>
        <input id='expr-time' type='text' class='readonly-text' readonly>
        <label>Expiration time(secs)</label>
    </div>
</template>
<style scoped>
p{
    padding: 5px;
    font-size: 40px;
    margin:10px 0 10px 0;
    padding-bottom:10px;
    border-bottom: 2px solid black;
}
#uploaded-panel.invisible{
    display: none;
}
#uploaded-panel.visible{
    display: flex;
    flex-direction: column;
    align-items: left;

    width: 70%;
    margin:10px;
    padding:10px;
    padding-bottom: 10px;
    padding-top: 10px;

    box-sizing: border-box;
    border: 1px solid black;   
}
#uploaded-panel label{
    height: 15px;
    margin: 10px 0 10px 0;
    
    font-size: 10px;
    font-weight: 100;
    font-family:Arial, Helvetica, sans-serif;
    text-align: left;
}
#uploaded-panel input{
    height:30px;
    
    box-sizing: border-box;
    outline-style: none;
}

.copy-text{
    display: flex;
    flex-direction: row;
    align-items: left;
    justify-content: center;

    margin:0;

    box-sizing: border-box;
}
.copy-text .text-group{
    display: flex;
    flex-direction: column;
    justify-content: center;

    width: calc(100% - 60px);
    margin: 0;
}
.copy-text .button-group{
    display: flex;
    flex-direction: column;
    justify-content: center;

    margin: 0;
}
.copy-text input{
    height: 30px;
    box-sizing: border-box;
}
.copy-text button{
    height: 30px;
    width: 60px;
}

.button{
    width: 60px;
    height: 30px;

    font-size:10px;
    font-weight: 600;
    font-family: Arial, Helvetica, sans-serif;

    box-sizing: border-box;
    border: 2px solid balck;
    margin: 0;

    background-color: rgb(14, 201, 129);   
}
.button:hover{
    cursor: pointer;
    background-color: rgb(43, 234, 160);
}
.button:active{
    background-color: rgb(14, 144, 94);
}
.button:disabled{
    background-color: rgb(14, 144, 94);
    cursor: not-allowed;
}
.readonly-text{
    background-color: rgb(235, 231, 231);

    border: 1px solid black;
    cursor:default;
}

.labelbutton{
    height: 30px;
    width: 100px;

    display: flex;
    flex-direction: column;
    justify-content: center;

    font-size:15px;
    font-family: sans-serif;
    font-weight: 400;
    text-align: center;
    
    box-sizing: border-box;
    background-color: white;
}
.labelbutton.hoverenable:hover,
.labelbutton.hoverenable>label:hover{
    cursor: pointer;
}

</style>

