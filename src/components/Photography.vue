
<template>
    <v-carousel hide-delimiters>
        <v-carousel-item
            v-for="(image, i) in images"
            :src="image.src"
            lazy-src="../assets/loading_image.png"
            :key="i"
            aspect-ratio="1"
            eager
        >
        <template v-slot:placeholder>
            <div class="d-flex align-center justify-center fill-height">
                <v-progress-circular
                color="grey-lighten-4"
                indeterminate
                ></v-progress-circular>
            </div>
        </template>
    </v-carousel-item>
    </v-carousel>
</template>
  
<script>
    export default {
        data() {
            return {
                images: [
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172834&authkey=%21ADc1-JcELitHxek&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172830&authkey=%21AKFAgzIIuTvVDgo&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172796&authkey=%21AAmGZy9gjTzHcpk&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172788&authkey=%21ANqdJj2mIV8yF_M&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172798&authkey=%21ABldjRZP8kIQtI0&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172801&authkey=%21AMtS6PJHY30Ghwc&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172803&authkey=%21AISOgErLjHIvVqk&width=3456&height=5184'
                },
                {
                    src: "https://onedrive.live.com/embed?resid=E241B47466E9E170%2172804&authkey=%21AJIEFBP-JwnlreI&width=3456&height=5184"
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172805&authkey=%21APt-0CK-5W-RPNw&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172809&authkey=%21AKfwJCJ2WumkAJ0&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172812&authkey=%21AOX_-ElvmU9yo6A&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172820&authkey=%21AC-te61L72sssfw&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172828&authkey=%21AF37kEpkZya5G90&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172832&authkey=%21AN30IrInB2v58zU&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172841&authkey=%21AKbtiBaB2ijpdnY&width=3456&height=5184'
                },
                {
                    src: 'https://onedrive.live.com/embed?resid=E241B47466E9E170%2172843&authkey=%21AJqfujf7LSwHNQs&width=5184&height=3456'
                },
                ]
            }
        },
    }
</script>
  