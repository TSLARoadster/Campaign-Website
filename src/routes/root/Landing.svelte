<div id="landing">
    <div id="announcement">
        <span>
            CHECK OUT THE CAMPAIGN VIDEO:
            <a href="https://www.instagram.com/reel/Cr8jsuPutuA/" target="_blank">INSTAGRAM</a> |
            <a href="https://duvalschoolsorg.sharepoint.com/:v:/r/teams/3153_3153_StudentActivitiesOfficeSAO21-22copy230/Shared%20Documents/Campaign%20Central%20-%20SOPHOMORE%20Candidates/ALAN%20A%20PRESIDENT%20CAMPAIGN.mp4?csf=1&web=1&e=RGUacE" target="_blank">ONEDRIVE (DCPS)</a>
        </span>
    </div>
    <p><b>S</b>UPPORTING<br>
        <b>T</b>EAMWORK<br>
        <b>A</b>CHIEVEMENT AND<br>
        <b>R</b>ESPONSIBILITY FOR<br>
        <b>S</b>UCCESS
    </p>
    <div class="image-container">
        <img src="images/Group Photo.webp" alt="Group">
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
        display: -webkit-flex;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        flex-wrap: wrap;
    }

    #landing p {
        margin: 2vw;
        padding: 0;
    }

    img {
        margin: 1vw;
        width: 35vw;
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.5);
    }

    .image-container {
        display: -webkit-flex;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .name-container {
        display: -webkit-flex;
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

    #announcement {
        color: var(--blue-600);
        font-weight: bold;
        background-color: var(--gray-100);
        width: 100%;
        height: 15vh;
        border-radius: 10px;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 4.7vw;
    }

    #announcement a {
        color: var(--red-200);
    }

    @media only screen and (max-width: 800px) {
        img {
            width: 80%;
        }

        #landing p {
            font-size: 8vw;
        }

        .name {
            font-size: 5vw;
        }
    }
</style>