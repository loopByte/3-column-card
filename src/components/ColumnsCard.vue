<template>
    <div class="columns">
        <div class="column borange">
            <div class="column__icon">
                <img src="images/icon-sedans.svg" alt="">
            </div>
            <div class="column__title">
                <h1 class="column__title__text">Sedans</h1>
            </div>
            <div class="column__content">
                <p class="column__content__text">
                    Take an SUV for its spacious interior, power, and versatility. Perfect for your next family vacation and off-road adventures.
                </p>
            </div>
            <div class="column__action">
                <a href="#" class="button orange">Learn More</a>
            </div>
        </div>
        <div class="column dcyan">
            <div class="column__icon">
                <img src="images/icon-suvs.svg" alt="">
            </div>
            <div class="column__title">
                <h1 class="column__title__text">SUVs</h1>
            </div>
            <div class="column__content">
                <p class="column__content__text">
                    Take an SUV for its spacious interior, power, and versatility. Perfect for your next family vacation and off-road adventures.</p>
            </div>
            <div class="column__action">
                <a href="#" class="button d-cyan">Learn More</a>
            </div>
        </div>
        <div class="column vdcyan">
            <div class="column__icon">
                <img src="images/icon-luxury.svg" alt="">
            </div>
            <div class="column__title">
                <h1 class="column__title__text">Luxury</h1>
            </div>
            <div class="column__content">
                <p class="column__content__text">
                    Cruise in the best car brands without the bloated prices. Enjoy the enhanced comfort of a luxury rental and arrive in style.
                </p>
            </div>
            <div class="column__action">
                <a href="#" class="button v-d-cyan">Learn More</a>
            </div>
        </div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@700&family=Lexend+Deca&display=swap');

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

/* Columns wrapper */
.columns {
    width: 1440px;
    height: auto;
    display: flex;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    border-radius: 10px;
    overflow: hidden;
}

/* Background Colors */
.borange { background: hsl(31, 77%, 52%); } /* bright orange */
.dcyan { background: hsl(184, 100%, 22%); } /* dark cyan */
.vdcyan { background: hsl(179, 100%, 13%); } /* very dark cyan */

/* Column wrappers */
.column__icon,
.column__title,
.column__content,
.column__action {
    width: 100%;
    height: auto;
    padding: 10px 50px;
    margin-top: 20px;
}
.column__icon { margin-top: 50px; }
.column__action {
    margin: 100px 0px 50px 0px;
}

/* Column title */
.column__title__text {
    color: hsl(0, 0%, 95%);
    text-transform: uppercase;
    font-family: 'Big Shoulders Display', cursive;
}

/* Column text */
.column__content__text {
    font-size: 15px;
    font-family: 'Lexend Deca', sans-serif;
    color: hsla(0, 0%, 100%, 0.75);
}

/* Column Button */
.button {
    width: auto;
    height: auto;
    padding: 10px 20px;
    border-radius: 20px;
    text-decoration: none;
    border: 2px solid hsl(0, 0%, 95%);
    color: hsl(0, 0%, 95%);
    font-family: 'Lexend Deca', sans-serif;
}
.button:hover {
    background: hsl(0, 0%, 95%);
}
.button.orange:hover { color:hsl(31, 77%, 52%); }
.button.d-cyan:hover { color:hsl(184, 100%, 22%); }
.button.v-d-cyan:hover { color:hsl(179, 100%, 13%); }

/* Mobile layout */
@media screen and (max-width: 500px) {
    .columns {
        width: 375px;
        position: relative;
        top: 0;
        left: 0;
        transform: translate(0, 0);
        flex-direction: column;
    }
}
</style>