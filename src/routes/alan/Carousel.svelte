<script>
    import { onMount } from "svelte";
    import { writable } from "svelte/store";

    let currentIndex = writable(0);
    let infoCards = [];

    onMount(() => {
        infoCards = [
            {
                title: "WIN PEP RALLIES!",
                text: "To win more Pep Rallies, there needs to be better collaboration and communication within the entire sophomore class. One thing would be a <b>PEP RALLY HYPE committee</b>, which will be a group of students distributed among everyone else to make sure everyone is excited during the pep rally. For communication, I will also establish more lines of communication such as a <b>Remind group</b> for our class and more <b>active Instagram</b> and <b>Teams updates</b>. On top of this, I will delegate my officers with managing and organizing the class as a whole, to ensure that we are all organized and unified in pep rally spirit!",
            },
            {
                title: "MOTIVATE SUCCESS",
                text: "To promote more success at Stanton, there needs to be <b>more available class resources</b>, such as tutoring and study materials, along with better <b>time management strategies</b>. To achieve this, <b>I will make a website</b> that will act as a hub for the class, allowing people to meet up with other students for tutoring <b>(earn volunteer hours!)</b>, as well as other study tools and resources for all classes The website will also have tools to help you manage your time successfully to ensure that you never miss an assignment.",
            },
            {
                title: "HAVE FUN!",
                text: "Through frequent events and activites, I will work with our class officers to create more fun opportunities for sophomores that didn't exist during freshman year. Sadly, it is unlikely that having more field trips for sophomores will be accepted by admin, but I will work to create other fun activities outside of school such as <b>Sophomore Socials</b>. On top of this, I will work to create more opportunities for fun ways to earn <b>volunteer hours</b> while spending time with your friends. One of these opportunities that I want to start is a <b>Class of '26 Legacy Project</b>, which will have every sophomores' name printed in a new area that will be near the benches and gazebo. Through this, every student will be memorialized on campus.",
            },
        ];
    });

    function previous() {
        currentIndex.update((n) => (n === 0 ? infoCards.length - 1 : n - 1));
    }

    function next() {
        currentIndex.update((n) => (n === infoCards.length - 1 ? 0 : n + 1));
    }
</script>

<div class="carousel">
    <button on:click={previous}>&lt;</button>
    {#each infoCards as infoCard, i}
        {#if $currentIndex === i}
            <div class="info-card">
                <h3 class="info-card-title">{@html infoCard.title}</h3>
                <p class="info-card-text">{@html infoCard.text}</p>
            </div>
        {/if}
    {/each}
    <button on:click={next}>&gt;</button>
</div>

<style>
    .carousel {
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 5vw;
        height: 100%;
    }

    button {
        background-color: transparent;
        border: none;
        font-size: 3vw;
        cursor: pointer;
        padding: 1vw;
        transition: all 0.2s;
    }

    button:hover {
        color: var(--red-100);
        transition: all 0.2s;
    }

    .info-card {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: var(--blue-200);
        border-radius: 30px;
        margin: 5vw;
        padding: 2vw;
    }

    .info-card-title {
        margin: 0;
        padding: 0;
        font-size: 5vw;
        color: var(--red-100);
    }

    .info-card-text {
        margin: 0;
        padding: 0;
        font-size: 2vw;
        color: var(--red-300);
        text-align: center;
    }

    @media only screen and (max-width: 800px) {
        .info-card-title {
            font-size: 8vw;
        }

        .info-card-text {
            font-size: 4vw;
        }
    }
</style>
