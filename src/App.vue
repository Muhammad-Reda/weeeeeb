<script>
    import { RouterLink, RouterView } from "vue-router";
</script>

<template>
    <head>
        <link
            rel="stylesheet"
            href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
        />
        <link
            rel="stylesheet"
            href="../src/assets/fontawesome-free-6.1.1-web/css/all.min.css"
            type="text/css"
        />
    </head>
    <nav class="navbar">
        <div class="title">Muhammad Reda</div>
        <input type="checkbox" id="toggler" />
        <label for="toggler"><i class="fa fa-bars"></i></label>
        <div class="menu">
            <ul class="nav-sub">
                <li class="list-item">
                    <RouterLink to="/" class="nav-link">Home</RouterLink>
                </li>
                <li class="list-item">
                    <RouterLink to="/Android" class="nav-link"
                        >Android</RouterLink
                    >
                </li>
                <li class="list-item">
                    <RouterLink to="/About" class="nav-link">About</RouterLink>
                </li>
                <li class="list-item">
                    <RouterLink to="/Contact" class="nav-link"
                        >Contact</RouterLink
                    >
                </li>
            </ul>
        </div>
    </nav>
    <router-view />

    <footer class="text-center text-white" id="bawah">
        <div id="copyright">
            © 2022 Copyright: <strong>Muhammad Reda</strong>
        </div>
        <div class="icon" id="icon">
            <ul>
                <li>
                    <a
                        href="https://www.facebook.com/profile.php?id=100009677568934"
                        target="_blank"
                        ><i class="fab fa-facebook-f" id="facebook"></i
                    ></a>
                </li>
                <li>
                    <a
                        href="https://instagram.com/1xredha?igshid=YmMyMTA2M2Y="
                        target="_blank"
                        ><i class="fab fa-instagram" id="instagram"></i
                    ></a>
                </li>
                <li>
                    <a
                        href="https://www.facebook.com/profile.php?id=100009677568934"
                        target="_blank"
                        ><i class="fab fa-twitter" id="twitter"></i
                    ></a>
                </li>
                <li>
                    <a
                        href="https://www.facebook.com/profile.php?id=100009677568934"
                        target="_blank"
                        ><i class="fab fa-github" id="github"></i
                    ></a>
                </li>
            </ul>
        </div>
    </footer>
</template>

<style>
    #bawah {
        text-align: center;
        padding-top: 40px;
    }

    #copyright {
        text-align: center;
    }
    .title {
        cursor: pointer;
        color: white;
    }
    .navbar {
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        justify-content: space-between;
    }
    #app {
        margin: 0 auto;
        width: 100%;
        height: 100%;
        min-height: 100vh;
        padding: 2rem;
        font-weight: normal;
        background-color: #272c31;
        font-family: "montserrat", sans-serif;
    }
    .navbar .nav-link {
        text-decoration: none;
        color: white;
    }
    .navbar .nav-link:hover {
        color: inherit;
    }
    .nav-sub {
        list-style: none;
        display: flex;
        gap: 25px;
    }
    #toggler,
    .navbar label {
        display: none;
    }

    @media screen and (max-width: 768px) {
        .menu {
            width: 100%;
            max-height: 0;
            overflow: hidden;
        }

        .nav-sub {
            padding-left: 0;
            margin: 0;
            flex-direction: row;
            align-items: center;
            display: flex;
        }

        .navbar label {
            display: inline-flex;
            align-items: center;
            cursor: pointer;
            padding: 5px;
        }

        #toggler:checked ~ .menu {
            max-height: 100%;
        }
    }
    .navbar i {
        color: white;
    }
    .icon {
        text-align: center;
    }
    #facebook {
        color: #0028b9;
    }
    #instagram {
        color: #c13584;
    }
    #github {
        color: aliceblue;
    }
    .icon ul li {
        display: inline-block;
        margin-left: 15px;
        margin-right: 15px;
        font-size: 35px;
        color: #333;
        cursor: pointer;
        transition: 0.3s;
    }

    .icon ul li:nth-child(1):hover {
        border-radius: 20%;
        font-size: 28px;
        width: 28px;
        height: 28px;
    }

    .icon ul li:nth-child(2):hover {
        border-radius: 20%;
        font-size: 28px;
        width: 28px;
        height: 28px;
    }

    .icon ul li:nth-child(3):hover {
        border-radius: 20%;
        font-size: 28px;
        width: 28px;
        height: 28px;
    }

    .icon ul li:nth-child(4):hover {
        border-radius: 20%;
        font-size: 28px;
        width: 28px;
        height: 28px;
    }
</style>
