<div class="container">
    <div class="left">
        <div class="goals">
            <h3>my goals:</h3>
            <ul>
                <li>create a fun and better sophomore year</li>
                <li>first place in pep rallies</li>
                <li>volunteer hours</li>
            </ul>
        </div>
        <div class="ideas">
            <h3>my ideas!</h3>
            <ul>
                <li>end of year class film</li>
                <li>time capsule</li>
                <li>candy gram fundraising</li>
                <li>beach social/cleanup</li>
            </ul>
        </div>
    </div>
    <div class="main">
        <h2>VOTE FOR</h2>
        <h1>ANALEE TAPNIO</h1>
        <span class="subtitle">check out @analee.souchai on instagram and teams for my platform information</span>
        <p>As a prior class officer, I'm experienced!
            Learning skills from this year, I can turn
            our next year as sophomores
            into an unforgettable one.</p>
        <div class="about-me">
            <h3>abt me:</h3>
            <ul>
                <li>my favorite color is pink</li>
                <li>i have a wiener dog named Winnie</li>
                <li>i'm best friends w blackpink</li>
            </ul>
        </div>
    </div>
    <img src="images/Analee.png" alt="Analee">
</div>

<style>
    .container {
        display: flex;
        flex-direction: row;
        align-content: space-between;
        justify-content: center;
    }

    .left {
        display: flex;
        flex-direction: column;
        align-content: space-between;
        justify-content: flex-end;
        width: 60%;
        margin: 5vw;
    }

    .ideas {
        margin: 8vh 0 0 0;
    }

    h3 {
        font-size: 2vw;
        margin: 0;
        padding: 0;
        text-align: center;
    }

    ul {
        font-size: 1.5vw;
        margin: 0;
        padding: 0;
        width: 100%;
        text-align: center;
    }

    .main {
        display: flex;
        flex-direction: column;
        align-content: space-between;
        justify-content: center;
        width: 100%;
        text-align: center;
    }

    .main h2 {
        color: var(--blue-500);
        font-size: 3vw;
        margin: 0;
        padding: 0;
    }

    .main h1 {
        font-size: 6vw;
        margin: 0;
        padding: 0;
        color: var(--red-200);
        text-shadow: 0 0.05em var(--blue-500);
    }

    .subtitle {
        color: var(--red-200);
        font-size: 1.8vw;
    }

    .main p {
        font-size: 2.2vw;
        margin: 5vh;
        padding: 0;
    }

    .about-me {
        margin: 0 0 0 50%;
    }

    img {
        width: 100%;
        margin: 5vw;
    }

    @media only screen and (max-width: 800px) {
        .container {
            flex-direction: column;
            align-content: space-evenly;
            justify-content: center;
        }

        .left {
            width: 100%;
            margin: 0;
            order: 2;
        }

        .main {
            width: 100%;
            margin: 0;
            order: 1;
        }

        .about-me, .goals, .ideas {
            margin: 1vh auto;
            width: 40%;
        }

        img {
            width: 80%;
            margin: 5vh auto;
            order: 3;
        }

        .main h2 {
            font-size: 8vw;
        }

        .main h1 {
            font-size: 12vw;
        }

        .subtitle {
            font-size: 6vw;
            margin: auto;
            width: 70%;
        }

        .main p {
            font-size: 7vw;
        }

        h3 {
            font-size: 6vw;
        }

        ul {
            font-size: 4vw;
        }
    }
</style>