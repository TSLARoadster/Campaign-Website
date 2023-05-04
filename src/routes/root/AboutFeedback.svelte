<div class="about-feedback-container">
    <div id="about" class="info-container">
        <div class="header">
            <h1>ABOUT US</h1>
            <img class="icon" src="images/About Icon.png" alt="About Icon" />
        </div>
        <p class="body">
            We are all extremely dedicated Stanton students. Together we participate in a wide variety of Stanton activities, including numerous clubs and sports. We feel that across our wide variety of experiences and connections with a wide variety of people, we are well equipped to represent the class of 2026. We share the goal of wanting to make sophomore year the best yet, and we have many awesome ideas about socials and fun events! Last of all, we want more opportunities for volunteering, academic success, and more DUBS at pep rallies.
        </p>
    </div>
    <div id="feedback" class="info-container">
        <div class="header">
            <h1>FEEDBACK</h1>
            <img class="icon" src="images/Feedback Icon.png" alt="Feedback Icon" />
        </div>
        <p class="body">
            We represent <b>YOU</b>! If you have any questions, comments, concerns, or any other feedback, please fill out the below form and we will get back to you as soon as possible!
            <br><br>
            No time to fill out the form? No problem! Instead of filling it out, you can also directly message any of us on our Instagrams.
        </p>
        <a class="form" href="https://forms.office.com/Pages/ResponsePage.aspx?id=TR3rjaTQBE2JrvcHbLqp-50hh3jXAelGujHrVrKaHU1UQUtPV05ERzM5T1dTQ1JNNkM2RTVOMUNCRS4u" target="_blank" rel="noopener noreferrer">MICROSOFT FORMS</a>
    </div>
</div>

<style>
    .about-feedback-container {
        margin: 15vh 4vw 0 4vw;
        display: -webkit-flex;
        display: flex;
        flex-wrap: wrap;
        align-items: flex-start;
        justify-content: space-evenly;
    }

    .info-container {
        display: -webkit-flex;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 40%;
        margin: 2vw;
    }

    .header {
        display: -webkit-flex;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .header h1 {
        font-size: 5vw;
        color: var(--blue-500);
        margin: 0;
    }

    .icon {
        width: 5vw;
        margin-left: 2vw;
    }

    .body {
        margin: 0;
        color: var(--red-300);
        font-size: 2vw;
    }

    .form {
        margin: 4vh 2vw;
        border: 0.2em solid var(--blue-300);
        padding: 1em 1em;
        font-size: 2vw;
        width: 90%;
        transition: background-color 0.3s, color 0.2s;
        text-align: center;
        color: var(--gray-200);
    }

    .form:hover {
        background-color: var(--blue-300);
        color: #ffffff;
    }

    @media only screen and (max-width: 800px) {
        .info-container {
            width: 100%;
        }

        .header h1 {
            font-size: 13vw;
        }

        .icon {
            width: 13vw;
        }

        .body {
            font-size: 5vw;
            text-align: center;
        }

        .form {
            width: 50%;
            font-size: 5vw;
            margin: 1vh;
        }
    }
</style>