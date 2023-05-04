<div id="mission">
    <img class="pep-rally" src="images/Pep Rally.png" alt="Pep rally">
    <div class="text-container">
        <span class="heading">Our Mission:</span>
        <span class="subheading">S.O.P.H.O.M.O.R.E.S.</span>
        <p class="body">Our goal as your class government is: <b>Striving for Optimal Performance, Harnessing Opportunities, Mastering Objectives, Representing Excellence, and Success</b>. In other words, our goal is to make sure our <b>2023-24</b> school year is the best year we've ever had!</p>
        <img class="star-graphic" src="images/Stars Graphic.png" alt="Stars graphic">
    </div>
</div>


<style>
    #mission {
        margin: 15vh 1vw 0 1vw;
        display: flex;
        justify-items: flex-start;
        align-items: center;
        flex-wrap: wrap;
        width: auto;
    }

    .text-container {
        display: flex;
        flex-direction: column;
        width: 40%;
    }

    .pep-rally {
        width: 60%;
    }

    .heading {
        color: var(--blue-500);
        font-size: 5vw;
        font-weight: bold;
    }

    .subheading {
        color: var(--red-200);
        font-size: 5vw;
        text-shadow: 0 0.07em var(--blue-500);
        font-weight: bold;
    }

    .body {
        font-family: "Raleway Thin", sans-serif;
        color: var(--red-300);
        font-size: 1.2vw;
    }

    .star-graphic {
        margin: 5vh 0
    }

    @media only screen and (max-width: 800px) {
        .pep-rally {
            width: 100%;
        }

        .text-container {
            width: 100%;
        }

        .heading, .subheading {
            text-align: center;
            font-size: 13vw;
        }

        .body {
            font-size: 5vw;
            text-align: center;
        }

        .star-graphic {
            width: 50%;
            margin: auto
        }
    }
</style>