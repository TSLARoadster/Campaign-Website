<script lang="ts">
    import Carousel from "./Carousel.svelte";
</script>

<div class="container">
    <div class="top-container">
        <div class="portrait-container">
            <img class="portrait" src="images/Alan.webp" alt="Alan Alwakeel">
        </div>
        <div class="info-container">
            <h2 class="title">CLASS PRESIDENT</h2>
            <h1 class="name">ALAN ALWAKEEL</h1>
            <span class="subtitle">INITIATIVE. ATTENTIVE. CREATIVE.</span>
            <div class="social-container">
                <a href="https://instagram.com/alan.alwakeel" target="_blank">
                    <div class="social">
                            <img src="images/Instagram.webp" alt="Instagram">
                            <span class="username">@ALAN.ALWAKEEL</span>
                    </div>
                </a>
                <div class="social">
                    <img src="images/Snapchat.webp" alt="Snapchat">
                    <span class="username">@ALAN.ALWAKEEL07</span>
                </div>
            </div>
            <div class="goals">
                <h2 class="goals-title">MY GOALS:</h2>
                <ul class="goals-list">
                    <li class="goal">
                        <img src="images/Checkmark.webp" alt="Checkmark">
                        <span class="goal-title">Win Pep Rallies</span>
                        <span class="goal-text"> - Better collaboration + communication</span>
                    </li>
                    <li class="goal">
                        <img src="images/Checkmark.webp" alt="Checkmark">
                        <span class="goal-title">Motivate Success</span>
                        <span class="goal-text"> - Class website + volunteering</span>
                    </li>
                    <li class="goal">
                        <img src="images/Checkmark.webp" alt="Checkmark">
                        <span class="goal-title">Have Fun!</span>
                        <span class="goal-text"> - Sophomore Socials + Legacy Project</span>
                    </li>
                </ul>
            </div>
            <h3 class="slogan">Shoot for the Stars! Vote the stellar way for Alan A!</h3>
            <span class="details">SCROLL FOR MORE DETAILS</span>
        </div>
    </div>
    <Carousel />
</div>


<style>
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        height: 100%;
    }

    .top-container {
        display: flex;
        align-items: flex-start;
        justify-content: space-evenly;
        height: 70%;
        margin: 0 5vw;
    }

    .portrait-container {
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
        margin: 5vh 0 0 10vw;
        width: 20%
    }

    .portrait {
        width: 100%;
    }

    .info-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;
        width: 80%;
    }

    .title {
        font-size: 3vw;
        color: var(--blue-500);
        text-shadow: 0 0 0.1em rgba(0, 0, 0, 0.2);
        margin: 5vh 0 0 0;
    }

    .name {
        font-size: 7vw;
        color: var(--red-200);
        margin: 0;
        text-shadow: 0 0.05em var(--blue-500);
    }

    .subtitle {
        font-size: 1.5vw;
        color: var(--blue-600);
        font-weight: bold;
        margin: 0 0 1vh 0;
    }

    .social-container {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
        margin: 1vh;
    }

    .social {
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0.5vh;
    }

    .social img {
        width: 3vw;
        margin: 0 1vw 0 0;
    }

    .username {
        font-size: 1.5vw;
        color: var(--blue-300);
        font-weight: bold;
        margin: 0;
    }

    .goals {
        display: flex;
        flex-direction: column;
    }

    .goals-title {
        font-size: 5vw;
        color: var(--blue-500);
        margin: 0;
        text-align: center;
    }

    .goals-list {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
        margin: 0;
        padding: 0;
        list-style: none;
        font-family: "Raleway", sans-serif;
        color: var(--red-300);
    }

    .goal {
        display: flex;
        align-items: center;
    }

    .goal img {
        width: 3vw;
        margin: 0 1vw;
    }

    .goal-title {
        margin: 0;
        padding: 0;
        font-size: 2vw;
    }

    .goal-text {
        margin: 0 0.3vw;
        padding: 0;
        font-size: 1.2vw;
    }

    .slogan {
        font-size: 3vw;
        color: var(--blue-500);
        margin: 0;
        text-align: center;
        font-weight: bold;
    }

    .details {
        font-size: 2vw;
        color: var(--gray-200);
    }

    @media only screen and (max-width: 800px) {
        .title {
            font-size: 7vw;
        }

        .name {
            font-size: 10vw;
        }

        .subtitle {
            font-size: 4vw;
        }

        .social img {
            width: 6vw;
        }

        .username {
            font-size: 4vw;
        }

        .goals {
            width: 100%;
        }

        .goals-title {
            font-size: 8vw;
        }

        .goal img {
            width: 7vw;
        }

        .goal-title {
            font-size: 5vw;
        }

        .goal-text {
            font-size: 2.6vw;
        }

        .slogan {
            font-size: 4vw;
        }

        .details {
            display: none
        }
    }
</style>