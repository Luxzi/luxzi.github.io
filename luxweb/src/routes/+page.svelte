<script lang="ts">
    import Navbar from "../components/navbar.svelte";
</script>

<svelte:head>
    <title>Homepage</title>
</svelte:head>

<Navbar />
<div class="section">
    <h1>Hello! I'm Luxzi (they/them)</h1><br/>
    I've been writing software since 2016, which means I've accumulated 8 years of experience. 
    My main areas of interest are systems programming (C, C++, and Rust), game modding, utility software, containerization, and CTFs.
    My programming journey began well before I even owned a computer.
    As a kid, I spent hours disassembling and reassembling electronics, driven by a fascination with how things worked. This innate curiosity about complex systems has shaped my path as an engineer.
    If you’d like to get in touch, please visit the <a data-sveltekit-preload-data href="/contact">Contact</a> page.<br/><br/>

    <h2>Projects I've created or worked on</h2>
    <div class="project-grid">
        <div class="project-card">
            <ul>
                <div class="project-image"><img src="/chunklim-icon.png" width="auto" height="50vh" alt="Project preview"/></div>
                <li><h1>ChunkLim</h1><br/>
                <p>Server-side Minecraft Forge chunklimiter mod.</p></li>
            </ul>
        </div>


        <div class="project-card">
            <ul>
                <div class="project-image"><img src="/chunklim-icon.png" width="auto" height="50vh" alt="Project preview"/></div>
                <li><h1>lthoerner/rush</h1><br/>
                <p>A user-focused shell, implemented in Rust.</p></li>
            </ul>
        </div>

        <div class="project-card">
            <ul>
                <div class="project-image"><img src="/chunklim-icon.png" width="auto" height="50vh" alt="Project preview"/></div>
                <li><h1>knewsnotifd</h1><br/>
                <p>Kernel news RSS notifier daemon for Discord webhooks.</p></li>
            </ul>
        </div>

        <div class="project-card">
            <ul>
                <div class="project-image"><img src="/chunklim-icon.png" width="auto" height="50vh" alt="Project preview"/></div>
                <li><h1>ChunkLim</h1><br/>
                <p>Server-side Minecraft Forge chunklimiter mod</p></li>
            </ul>
        </div>

        <div class="project-card" style="grid-column: 1 / 3; max-width: 100vw; padding: 1.1rem;">
            <ul>
                <li><h1>View all...</h1><br/>
                <p>This will redirect you to GitHub</p></li>
            </ul>
        </div>
    </div>
</div>

<style>
    .project-grid {
        display: grid;
        margin-top: 10px;
        grid-template-columns: auto auto;
        gap: 5px;
    }

    .project-card {
        background: #111111;
        transition: all 0.3s ease-in-out;
        padding: 1rem;
        max-width: 50vw;
    }

    .project-image {
        float: right;
        transform: scale(171%) translateY(0.25vh) translateX(-0.07vw);
    }

    .project-card li {
        display: inline;
        list-style: none;
    }

    .project-card h1,p {
        display:contents;
    }

    @media only screen and (max-width: 800px) {
        .project-card h1 {
            font-size: 12pt;
        }
    }

    @media only screen and (max-width: 600px) {
        .project-card {
            max-width: 35vw;
        }
    }

    @media only screen and (max-width: 1300px) {
        .project-image {
            display: none;
        }
    }

    .project-card:hover {
        background: #eeeeee;
        color: #111111;
        cursor: pointer;
        transform: scale(110%);
        filter: drop-shadow(0px 0px 20px white);
    }
</style>