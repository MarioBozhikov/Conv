<template>
    <div class="Explain container">
        <div class="text-container">
            <h1 class="header">Convert your Youtube video</h1>
            <p class="snippet">Download your favorite music and clips from Youtube so you can lisent on anything anywhere!</p>
            <button class="start">Let's go</button>
        </div>
        <img src="~assets/img/logo.png" alt="Logo" class="image">
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Russo+One&display=swap");
* {
  font-family: "Russo One", sans-serif;
}
.Explain {
    height: 50vh;
        position: relative;
        display: flex;
        padding: 2rem 0;
        align-items: flex-start;
        justify-content: space-between;
        margin-right: 0rem;
    }
    .text-container {
        width: 50%;
        margin-top: 1rem;
    }
    .header {
        font-weight: 900;
        font-size: 4rem;
    }
    .snippet {
        color: rgb(85, 84, 84);
        font-size: 1.25rem;
    }
    .image {
        width: 19rem;
        margin-top: 1rem;
        margin-right: 15rem;
    }
    .start {
        --c:#4d7ea8;
        padding: 1rem 4rem;
        background: linear-gradient(to bottom right, #272932, #475b5a);
        color:var(--c);
        outline: none;
        width: 20rem;
        font-weight: 700;
        border-radius: 50px;
        z-index: 2;
        cursor: pointer;
        display: inline-block;
        font-size: 20px;
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
        border: none;
    }
    .start:hover {
        color: whitesmoke;
    }
    @media (max-width: 500px) {
        .Explain {
            height: 40vh;
        }
    }
</style>