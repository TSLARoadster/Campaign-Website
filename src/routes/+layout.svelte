<script lang="ts">
    let navbar;

    // scrollTo action
    function scrollTo(node, options) {
        const handleScroll = (event) => {
            event.preventDefault();
            const target = document.querySelector(event.currentTarget.getAttribute("href"));
            const navbarHeight = navbar.offsetHeight + 20;

            if (target) {
                // Offset the scroll position by the navbar height
                const targetPosition = target.getBoundingClientRect().top + window.scrollY - navbarHeight;
                window.scrollTo({ top: targetPosition, behavior: "smooth", ...options });
            }
        };

        node.addEventListener("click", handleScroll);
        return {
            destroy() {
                node.removeEventListener("click", handleScroll);
            },
        };
    }
</script>



<nav bind:this={navbar}>
    <div class="nav-container">
        <a class="title" href="#top" use:scrollTo={{ navbar }}><b>VOTE FOR <span>STARS</span></b></a>
        <div class="options">
            <a class="lesser-button option" href="#mission" use:scrollTo={{ navbar }}>Our Mission</a>
            <a class="lesser-button option" href="#about" use:scrollTo={{ navbar }}>About Us</a>
            <a class="feedback-button option" href="#feedback" use:scrollTo={{ navbar }}>Send Feedback</a>
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
        text-align: center;
        transition: background-color 0.3s, color 0.2s;
    }

    .feedback-button:hover {
        background-color: var(--blue-500);
        color: #ffffff;
    }

    @media only screen and (max-width: 800px) {
        .nav-container {
            height: 5vh;
            padding: 0.5em 1em;
        }

        .lesser-button {
            display: none;
        }

        .feedback-button {
            width: 100%;
            text-align: center;
            font-size: 1.5vh;
        }
    }

</style>