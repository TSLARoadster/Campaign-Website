<nav>
    <div class="nav-container">
        <a class="title" href="/"><b>VOTE FOR <span>STARS</span></b></a>
        <div class="options">
            <a class="lesser-button option" href="#mission">Our Mission</a>
            <a class="lesser-button option" href="#about">About Us</a>
            <a class="feedback-button option" href="#feedback">Send Feedback</a>
        </div>
    </div>
</nav>

<slot></slot>

<style>
    nav {
        background-color: var(--blue-200);
        position: sticky;
        top: 0
    }

    .nav-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        padding: 0.5em 2em;
    }

    .title {
        font-size: clamp(12pt, 7vw, 60pt);
        width: 100%;
        color: var(--blue-500)
    }

    .title span {
        color: var(--red-200);
        text-shadow: 0 0.07em var(--blue-500)
    }

    .options {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 100%;
        list-style: none;
        position: relative;
    }

    .option {
        color: var(--gray-200);
        font-family: "Montserrat Thin",sans-serif;
        font-size: clamp(1pt, 2vw, 16pt);
    }

    .lesser-button {
        transition: all 0.2s;
        padding: 0.5em;
        border-bottom: 0 solid;
    }

    .lesser-button:hover {
        color: var(--blue-400);
        border-bottom: 0.2em solid var(--blue-400);
        transition: all 0.2s;
    }


    .feedback-button {
        border: 0.2em solid var(--blue-500);
        border-radius: 50px;
        padding: 1em 1em;
        display: flex;
        align-items: center;
        transition: background-color 0.3s, color 0.2s;
    }

    .feedback-button:hover {
        background-color: var(--blue-500);
        color: #ffffff;
    }
</style>