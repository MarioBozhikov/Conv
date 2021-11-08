<template>
    <div class="Conv">
        <h1 class="h1">Convert any video to mp3/mp4 file.</h1>
            <div class="URL">
              <input class="URL-input" placeholder="Insert your link here..."/>
              <button class="cnvrt-but" id="btn">Start Converting now!</button>
              <select class="opt">
                <option value="mp3">MP3</option>
                <option value="mp4">MP4</option>  
              </select>
        </div>
    </div>
</template>

<script>
    export default function(req, res, next){
      plugins:[
        { src: '~/plugins/script.js', mode: 'client'}
      ]
    }
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Russo+One&display=swap");
* {
  font-family: "Russo One", sans-serif;
}
.Conv{
    width: auto;
    height: 15rem;
    border: none;
    overflow: hidden;
    padding: 0;
    cursor: pointer;
    margin-top: 20px;
}
.h1 {
  text-align: center;
  padding-top: 55px;
  margin-bottom: 1px;
}
.URL {
  position: relative;
  width: 1000px;
  height: 55px;
  padding: 30px 30px 50px 30px;
  align-content: center;
  margin: auto;
}
.URL-input {
  width: 100%;
  border: 2px solid #ccc;
  border-radius: 104px;
  padding: 11px 103px 12px 15px;
  line-height: 1;
  box-sizing: border-box;
  outline: none;
}
.cnvrt-but {
  position: absolute;
  right: 34px;
  top: 34px;
  bottom: 111px;
  border: 0;
  background: linear-gradient(to bottom right, #272932, #475b5a);
  color: #4d7ea8;
  outline: none;
  margin: 0;
  padding: 0 10px;
  border-radius: 50px;
  z-index: 2;
  cursor: pointer;
  display: inline-block;
  font-size: 16px;
  font-weight: 50;
  line-height: 2.5;
  padding: 0 1rem;
  text-align: center;
  text-decoration: none;
  transition: box-shadow 0.2s ease-in-out;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  white-space: nowrap;
}
.cnvrt-but:hover {
  color: rgb(148, 19, 64);
}
.opt{
  position: relative;
  border: 0;
  background: linear-gradient(to bottom right, #272932, #475b5a);
  color: #4d7ea8;
  outline: none;
  margin: 4px 1px;
  padding: 3px 30px 5px;
  border-radius: 50px;
  z-index: 2;
  cursor: pointer;
  font-size: 17px;
  font-weight: 50px;
  text-align: center;
} 
</style>