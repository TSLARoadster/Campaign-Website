<div id="landing">
    <p><b>S</b>UPPORTING<br>
        <b>T</b>EAMWORK<br>
        <b>A</b>CHIEVEMENT AND<br>
        <b>R</b>ESPONSIBILITY FOR<br>
        <b>S</b>UCCESS
    </p>
    <div class="image-container">
        <img src="static/images/Group Photo.png" alt="Group">
        <div class="name-container">
            <span class="name"><a href="/analee">Analee T</a></span>
            <span class="name"><a href="/javion">Javion L</a></span>
            <span class="name"><a href="/alan">Alan A</a></span>
            <span class="name"><a href="/evie">Eviem'ree M</a></span>
            <span class="name"><a href="/jimia">Jimia L</a></span>
        </div>
        <span class="name">Click on the names above!</span>
    </div>
</div>

<style>
    #landing {
        color: var(--red-200);
        font-size: 4.5vw;
        margin: 3vh 1vw;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
        flex-wrap: wrap;
    }

    b {
        font-weight: bolder;
    }

    #landing p {
        margin: 2vw 2vw;
        padding: 0;
    }

    img {
        margin: 2vw 2vw 0.5vh 2vw;
        width: 35vw;
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.5);
    }

    .image-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .name-container {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-evenly;
        width: 100%;
    }

    .name {
        font-size: 2vw;
        font-weight: bold;
    }

    .name a {
        color: var(--blue-500)
    }

    @media only screen and (max-width: 800px) {
        img {
            width: 80%;
        }

        #landing p {
            font-size: 5vh;
        }

        .name {
            font-size: 2vh;
        }
    }
</style>