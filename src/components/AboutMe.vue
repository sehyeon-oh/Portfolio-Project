<template>
    <section id="aboutme_section">
        <LazyLoad class="lazy_picture">
            <div class="picture_container">
                <img src="../assets/profile_pic.jpg" alt="Se Hyeon's Profile Picture">
            </div>
        </LazyLoad>
        <LazyLoad class="lazy_text">
            <div class="aboutme_content">
                <h3>&emsp;"As a lifelong technology enthusiast, my journey has been marked by continuous exploration and learning in the ever-evolving world of technology. Since embarking on my IT career in 2017, my primary passions have centered around Front-End and Web Development. My academic achievements include a Bachelor's degree in System Information from São Paulo University (USP, Brazil) and a Postgraduate Diploma in Web & Mobile Development from Langara College in Vancouver, BC."</h3>
            </div>
        </LazyLoad>
    </section>
</template>

<script>
import LazyLoad from './Global Functions/LazyLoad.vue'

export default {
    components: {
        LazyLoad,
    },

    name: 'AboutMe',
}
</script>

<style scoped>

#aboutme_section {
    position: relative;
    background-color: #030303;
    width: 100%;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

#aboutme_section > .lazy-load-wrapper {
    width: 100%;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

#aboutme_section > .lazy_picture {
    padding: 3em 5% 2rem;
}

#aboutme_section > .lazy_text {
    padding: 0 5% 2rem;
}


#aboutme_section > .lazy-load-wrapper > .picture_container {
    width: 80%;
}

#aboutme_section > .lazy-load-wrapper > .picture_container > img {
    width: 100%;
    border-radius: 50%;
}

#aboutme_section > .lazy-load-wrapper > .aboutme_content {
    padding: 0;
}

#aboutme_section > .lazy-load-wrapper > .aboutme_content > h3 {
    color: #B5B6B7;
    font-weight: lighter;
    font-size: 1rem;
    letter-spacing: .3px;
    line-height: 150%;
}

@media screen and (min-width: 769px) {
    #aboutme_section {
        flex-direction: row;
        padding: 5rem 5%;
    }
    
    #aboutme_section > .lazy-load-wrapper > .picture_container {
        width: 100%;
    }

    #aboutme_section > .lazy-load-wrapper > .picture_container > img {
        width: 100%;
    }

    #aboutme_section > .lazy-load-wrapper > .aboutme_content {
        padding: 0;
    }

    #aboutme_section > .lazy-load-wrapper > .aboutme_content > h3 {
        font-size: 1.2rem;
    }
}

</style>