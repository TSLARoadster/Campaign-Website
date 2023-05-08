<div class="container">
    <div class="goals">
        <h3>
            GOALS
        </h3>
        <ul class="goals-list">
            <li class="goal">More socials to help connect and build friendships with the class as a whole</li>
            <li class="goal">Aim for first place for all the pep rallies</li>
            <li class="goal">Make sophomore year the most memorable and academically the best</li>
        </ul>
    </div>
    <div class="main">
        <h3>CLASS OF 2026</h3>
        <h2>VOTE FOR</h2>
        <h1>JAVION LIU</h1>
        <span class="position">FOR CLASS OFFICER</span>
        <span class="subtitle">A FRESH FACE, A FRESH START</span>
        <a class="redirect" href="https://instagram.com/javionliu4officer" target="_blank">For more info, check out my campaign on Instagram! @javionliu4officer</a>
    </div>
    <div class="about">
        <img src="images/Javion.webp" alt="Javion Liu" />
        <div class="about-text">
            <h3>A LITTLE ABOUT ME</h3>
            <ul class="about-me-list">
                <li class="about-me-point">My favorite color is green</li>
                <li class="about-me-point">I do community service to my church</li>
                <li class="about-me-point">Pizza on top as my favorite food</li>
            </ul>
        </div>
    </div>
</div>

<style>
    .container {
        display: flex;
        align-items: flex-start;
        justify-content: space-evenly;
    }

    .goals {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: 5vw;
        width: 100%;
    }

    .goals h3 {
        font-size: 5vw;
        margin: 0;
        padding: 0;
        color: var(--blue-600);
    }

    .goals-list {
        margin: 0;
        padding: 0;
        color: var(--blue-600);
        font-size: 2vw;
        text-align: center;
        width: 100%;
    }

    .main {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: flex-start;
        margin: 1vw;
        width: 100%;
    }

    .main h3 {
        font-size: 2vw;
        margin: 0;
        padding: 0;
        color: var(--blue-300);
        font-weight: normal;
    }

    .main h2 {
        font-size: 3.5vw;
        margin: 0;
        padding: 0;
        color: var(--blue-600);
    }

    .main h1 {
        font-size: 6vw;
        margin: 0;
        padding: 0;
        color: var(--red-200);
        text-shadow: 0 0.05em var(--blue-500);
        letter-spacing: 0.1em;
    }

    .position {
        font-size: 3vw;
        margin: 0;
        padding: 0;
        color: var(--blue-300);
        font-weight: normal;
    }

    .subtitle {
        font-size: 1.5vw;
        margin: 0;
        padding: 0;
        color: var(--blue-600);
        font-weight: normal;
    }

    .redirect {
        font-size: 1.5vw;
        margin: 2vh 0 0 0;
        padding: 0;
        width: 40%;
        color: var(--red-300);
        font-weight: normal;
    }

    .about {
        display: flex;
        flex-direction: column;
        align-items: flex-end;
        justify-content: space-evenly;
        margin: 1vw;
        width: 100%;
    }

    .about img {
        width: 15vw;
        margin: 2vh 8vw 0 0;
    }

    .about-text {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: 3vh;
        width: 100%;
    }

    .about-text h3 {
        font-size: 3vw;
        margin: 0;
        padding: 0;
        color: var(--red-200);
        text-align: center;
    }

    .about-me-list {
        margin: 0;
        color: var(--blue-500);
        font-size: 1.5vw;
        text-align: center;
        width: 70%;
        padding: 0;
    }

    @media only screen and (max-width: 800px) {
        .container {
            flex-wrap: wrap;
        }

        .main {
            order: 1;
            align-items: center;
            text-align: center;
        }

        .main h3 {
            font-size: 6vw;
        }

        .main h2 {
            font-size: 6vw;
        }

        .main h1 {
            font-size: 10vw;
        }

        .position {
            font-size: 5vw;
        }

        .subtitle {
            font-size: 4vw;
        }

        .redirect {
            font-size: 5vw;
            width: 100%;
        }

        .about {
            order: 2;
            align-items: center;
        }

        .about img {
            width: 40vw;
            margin: 2vh 0 ;
        }

        .about-text h3 {
            font-size: 7vw;
        }

        .about-me-list {
            font-size: 5vw;
        }

        .goals {
            order: 3;
        }

        .goals h3 {
            font-size: 8vw;
        }

        .goals-list {
            font-size: 5vw;
            width: 76%;
        }
    }
</style>