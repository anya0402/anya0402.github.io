---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<style>
    .headertext {
        font-size: 60px;
        padding-bottom: 90px;
        text-align: center;
    }

    .button {
        padding: 16px 32px;
        text-align: center;
        /* text-decoration: none; */
        /* display: inline-block; */
        /* font-size: 16px; */
        margin: 4px 2px;
        transition-duration: 0.4s;
        cursor: pointer;
        background-color: white; 
        color: black; 
        border: 2px solid #000000;
        border-radius: 20px;
    }

    .button:hover {
        background-color: #4178db;
        color: white;
    }
</style>

<div class="headertext">Welcome to my website!</div>

<p style="text-align: center;">Click on the following buttons to learn more about me:</p>

<div style="display: flex; align-items: center; justify-content: space-evenly; padding-top: 10px">
    <a href="https://anya0402.github.io/about/">
    <button class="button">About Me</button>
    </a>

    <a href="https://anya0402.github.io/projects/">
    <button class="button">My Projects</button>
    </a>

    <a href="https://anya0402.github.io/resume/">
    <button class="button">My Resume</button>
    </a>
</div>