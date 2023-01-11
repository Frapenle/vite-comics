<template lang="">
    <footer>
        <section class="footer-top">
            <div class="container">
                <nav>
                    <!-- first column list -->
                    <ul>
                        <li><h3>DC Comics</h3></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                        <!--  -->
                        <li><h3>Shop</h3></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Characters</a></li>
                    </ul>

                    <!-- second column list -->
                    <ul>
                        <li><h3>DC Comics</h3></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                        <li><a href="#">News</a></li>
                        <li><a href="#">News</a></li>
                        <li><a href="#">News</a></li>
                        <li><a href="#">News</a></li>
                    </ul>

                    <!-- third column list -->
                    <ul>
                        <li><h3>DC Comics</h3></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                </nav>
            </div>
        </section>
        <section class="footer-bottom">
            <div class="container">
                <div class="footer-left">
                    <button><a href="#">Sign up now!</a></button>
                </div>
                <div class="footer-right">
                    <div class="social-network">
                        <h3>Follow us</h3>
                        <a href="#" class=""><img src="../assets/img/footer-facebook.png" alt="Facebook"></a>
                        <a href="#" class=""><img src="../assets/img/footer-twitter.png" alt="Twitter"></a>
                        <a href="#" class=""><img src="../assets/img/footer-youtube.png" alt="YouTube"></a>
                        <a href="#" class=""><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></a>
                        <a href="#" class=""><img src="../assets/img/footer-periscope.png" alt="Periscope"></a>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);
    padding: 1.5rem 0;
}

li {
    color: white;

    h3 {
        padding: .8rem 0 .2rem;
    }

    & a {
        color: white;
        font-size: .8rem;
        font-weight: 300;
    }
}

nav {
    display: flex;
    gap: 4rem;
}

.footer-bottom {
    height: 80px;
    display: flex;
    background-color: $footer-bottom-bg;
}

.footer-left>button {
    background-color: transparent;
    border: 2px solid $main-color;

    a {
        color: white;
    }
}

.container {
    width: 100%;
    display: flex;
    height: 100%;
    justify-content: space-between;
    align-items: center;
}

img {
    height: 30px;
}

.social-network {
    display: flex;
    gap: 1rem;

    h3 {
        color: $main-color;
    }
}
</style>