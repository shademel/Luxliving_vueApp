<template>
    <div class="carousel-view">
        <transition-group class="carousel">
            <div class="slide">
                <h2>{{ slide.title }}</h2>
            </div>
        </transition-group>
        <div class="carousel-controls">
            <button class="carousel-controls_button" @click="previous">Prev</button>
            <button class="carousel-controls_button" @click="next">Next</button>
        </div>
    </div>
</template>

<script>


export default {
    data() {
        return {
            slides: [
                {
                    title: 'Table',
                    id: 1,
                    url: '../assests/Table-1.jpg'
                },
                {
                    title: 'Cabinet',
                    id: 2,
                    url: '../assets/Cabinet-1.jpg'
                },
                {
                    title: 'Sofa',
                    id: 3,
                    url: '../assets/Sofa-1.jpg'
                },
                {
                    title: 'Chair',
                    id: 4,
                    url: '../assets/Chair-1.jpg'
                }
            ]
        }
    },

    methods: {
        next() {
            const first = this.slides.shift()
            this.slides = this.slides.concat(first)
        },
        previous () {
            const last = thhis.slides.pop()
            this.slides = [last].concat(this.slides)
        }
    }
}
</script>

<style>
.carousel {
    width: 24em;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    display: flex;
}

.carousel-view {
    align-items: center;
    display: flex;
    flex-direction: column;
}

.slide {
    display: flex;
    align-items: center;
    justify-content: center;
    border: 0.1em;
    transition: transform 0.3s ease-in-out;
}

.slide:first-of-type {
    opacity: 0;
}

.slide:last-of-type {
    opacity: 0;
}
</style>