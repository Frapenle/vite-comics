<template lang="">
    <main>
        <div class="container">
            <div class="current-series">
                <h4>current series</h4>
            </div>
            <div class="cards-wrapper">
                <CardComponent v-for="card in cardsList"
                :imgPath="card.thumb"
                :price="card.price"
                :serie="card.series"
                :type="card.type"/>
            </div>
            <div class="flex">
                <button>Load more</button>
            </div>
        </div>
        <div class="banner">
            <div class="container">
                <div class="banner-items" v-for="element in bannersList">
                    <img :src="getImageName(element.imageName)" :alt="element.text">
                    <div class="banner-text">{{element.text}}</div>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import CardComponent from "./CardComponent.vue";

export default {
    name: 'MainVue',
    components: { CardComponent },
    data() {
        return {
            bannersList: [
                {
                    text: 'digital comics',
                    imageName: "comics-digital-comics.png"
                },
                {
                    text: 'dc merchandise',
                    imageName: "comics-merchandise.png"
                },
                {
                    text: 'subscription',
                    imageName: "comics-subscriptions.png"
                },
                {
                    text: 'comic shop locator',
                    imageName: 'comics-shop-locator.png'
                },
                {
                    text: 'dc power visa',
                    imageName: "dc-power-visa.svg"
                }
            ],
            cardsList: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },

    methods: {
        getImageName: function (imgName) {
            return new URL(`../assets/img/buy-${imgName}`, import.meta.url).href;
        }
    },

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

main {
    width: 100%;
    background-color: black;
    padding-top: 3rem;
    color: white;
}

.current-series {
    line-height: 0;
    padding: 1.4rem 1rem;
    color: white;
    background-color: $main-color;
    position: absolute;
    top: calc(-3rem - 1.4rem);
    left: 0;
    text-transform: uppercase;
}

.container {
    position: relative;
}


.cards-wrapper {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    font-size: .9rem;
    font-family: 'Roboto', sans-serif;
}

.flex {
    display: flex;
    justify-content: center;
}

button {
    margin: 1rem 0;
    background-color: $main-color;
    text-transform: uppercase;
}

.banner {
    width: 100%;
    background-color: $main-color;

    .container {
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    img {
        width: 30px;
    }

}

.banner-items {
    padding: 1rem 0;
    display: flex;
    align-items: center;

    .banner-text {
        margin-left: .6rem;
        text-transform: uppercase;
        font-weight: 300;
        font-size: .7rem;
    }
}
</style>