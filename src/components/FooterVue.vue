<template lang="">
    <footer>
        <div class="container">

        
            <section class="footer-top">
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
            </section>
            <section class="footer-down"></section>
        </div>
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

footer {
    background-color: grey;
    padding: 2rem 0;
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
</style>