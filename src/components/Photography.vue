
<template>
    <v-carousel hide-delimiters>
        <v-carousel-item
            v-for="(image, i) in images"
            :src="image.src"
            :key="i"
            aspect-ratio="1"
        ></v-carousel-item>
        <template v-slot:placeholder>
            <div class="d-flex align-center justify-center fill-height">
                <v-progress-circular
                color="grey-lighten-4"
                indeterminate
                ></v-progress-circular>
            </div>
        </template>
    </v-carousel>
</template>
  
<script>
    export default {
        data() {
            return {
                images: [
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mqPDDYdHuQP8Vu0CFY3Mymuxx29vlPCXQh5p_qgus5LzfSrJ_FxvA1FomfrAux57aM3clDF6twYbmWWCzFo_Zb2JAdf8JisjVYlOarPK6bwNB1BTQYl_mbUP2x8uzlA9OwzlajoTFq1nvj4O0w-4rokgf_HDIZ2e9INkEvN8x6dCKo3a6Ie2gu5tWIqr5Cj9OXnLe4yREpmUvy3mbzOBG-g?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mBKvqCOrITVaGdA_tDuZJgSxjsw8jt9SfkWpoSmY126CPxkPNg81d8E0fdx1qElksTyFf6IyMdUCZGNvUIbs92UpW__h0SWTHId2EtSpy0DvSvZlw1DsoW2XFWxRo0sEJFSNT6wElo7yc9Agndz_Od_SothHG68VQQ9B8NfvzxyjW40FpHUrKNRUY_0tAX5NBoa3PKLIqjDaQ4EfLZ0LrUQ?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mR0SxyBE1eWvrS_t_2A6Ktq6ute20f8p1MSqAXHDXPRvh5OSAWVDaN962BQpfU-cFQHNewPePb8IC2Rc3Y3PckJ_nFFFQQNkqoxeRV5Orhe47FnOvKSgByCUuQmKbQenyDV96MPXDlOMy9f4PYsOC1j6r0aHRJa9G3TNfAZLR2APQVkaUcm0Z0bptaL_GsuyZ4i2k27igXCx6peXOGYmAzQ?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mHM9ivjoFfHjE5dgiaYIxjiQMFokEo9fujwE281n-HaN134T7A6NU0sOz-VPGh8rl8cr2QSe-4N96zQ79sttUPhal3CHgRe7yJcXXK_z07dwZuAr0H34bBKmdAKzF6-j-mJ8aHGZ3fAu6spUws6hUWgGn0Bm93N08m6nXPC7SpQQw5QSRmdv6MnncsB6nLgm5QD0ANLHkGOrMC8fRGjFwJQ?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mQluvt_FGWXyvyAsu4BA9Fc2fCkxohAyC6nnMuPOQZN7EaTSZrks7TvGtUDKENoaOJOWgbzY9KVMe3o3AXp2OMTl4UPuV2AIbWs5Mxq8GXF3MvTmPjE7fryErux10If8Q1nbAtMeQXXxErqX_8cNfzygMPb40QijPMfm80DBm5wWdgMvBnMw8X4_Tfbhn5D5pT4MdxhoDcWPS5X8LdaYwXw?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mvQxZk98rh6N9H8kSsN_Hhm74bZf5txTs5Viz3L8OgkcfmwHk4Nrr1c_HYqWQeYpzLgBdHqk7Vm7hMUXoDrJi0VV1GvP7KT2Em_c1st4_N5sYXpiFw9N3AMWwDA2Mb5Ezzp8_pqKuOy8mNSiLo6QYJiZ6mG77keYupX7rGO1otkoQ7W_OTcxFy5hvjvZg222KxKXCsct_IaE72n0gZghBcA?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mFC0t5VmcMlaK-zH-W5HIjeSM4ZaUcH7KJu7z0cH3FImAj9NZXUV946oDFxAAJ_iYfMhRsmmFDZmG-ySxu5y3RGDITK2Ai-zNIwzFTiOL4l_20iryxA_LHy5kXUW4EymfcvxwKvvYlgVmP6DWezyphHrP0ZR6i3mgRLyKEWf0nUOT7pc6bMknW-VNx77TKDq0b7AydENvxN5jbY_-rrITeQ?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: "https://ams03pap002files.storage.live.com/y4mtrqfZvulUBmy_AzAVrx6kLtAGZAdfbukbsL_PeszGY9nFNZEYnAyYvxjbMSxnTfgGLTL_e8OkML2ON8AhX_4MKB5viB9JutsIsyRoYg4ttbnfpYFHXiqqHfXL0Egnlw04KIoVwsqy3CbKxXW8c5-8GdDGN3jRerW2DkJiGXqjDIzXVChkpPXL5v2i6KXgo-bnvyH_Fc1kfBYaqPTLrbYVw?encodeFailures=1&width=1102&height=1654"
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mEQ8j2ElGJ5dux3x8fXA5CvJMK0jRPO5Ein_uWSGZswLgAUrpojB43CDGd2qGXAWGFHMF4FBffxF-n0B7tk_2s2b_DfNVczMBL2RcXyiPgmglDotNnKRvOhePWmsxnFHM6zDmtS4buDPIOZJkOZCf5uqL-Tg4H8isfCTidbwMQVNrnc2Dz33Zj6dleXFVdJVOVhcj_hiVAe76P23bLqCBXw?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mD4g9IeH0DWrmn5KcRQLhaju93__yrVwolMqKQiTiWUA3g_oungJY8Ib4YN-uu1b8_nx6zOErvcppyCot-4PcGfAzM8mx1vDgSsP0ZTMV2O70zkMUNdGgPFZtM-S6JIn4H5i7Hl4qApKdF2Qkup3QOT3tDXjn5HIl7YWBR1wkXYgthACfmy8zMndJJwmRKDy4minWPrnXhP7bBm058S3gRQ?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mCtYvumUHPTlHzxH5OhFCoOrBk20vFcE-QdEuf2d-EfN55wQnOqXPXCIPJA6BdlNH325xzWmOImdUMPb29uUnQLVuQuXUwHFOLm_TWaeyyJB6yIJKBSXcbMKTtmF-0pX41llx4wDINWJzyixWOCuMjOoVfH8wy-xslF0ELoG4wArfhRfIRdwzvK0dtOKYUHI20VqkuL5aomBn2k657VNBZw?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mbLsZI7D2blyvu2_vBQUA66hUW-8WLdYoSZ7Z-jLzZv8XYdolzAOULEV2MK3mdLLaj3ISfTNlo9iIyI8DRDZASsxNcRoAmcevd2Eg9j5jv18DipZsm70537Y7sBX6-TVqLiA8Njno-o4RE-EV7iWBpIBg561n533JSr4rnKiK80bwCkjK4A7y6IQ3lLdRSldDiss7Ke328OhSahbtmyzBDQ?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mIPI2y9BfMRgq5wH5qa-xEcsZgxplSCJjbOB2iy_KLJ7IIs11dOmnPc5vMqlhoc_KhKUUOvzRFhwGaymYa0hS8QsfegwBFDv8DmEIefDOEmJqllkozTPWH7qCHIqLIS7KqDQjFPRpr12YMmdFTuDElVwBSpgz1Qh1xK2H_nSBImfKd53LA17PhHgmfe8PXaqdLvW9144HBk0q5_ybjYuXgA?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4m0Im1mKD1vhtCec47ONTdgQ-QTsx2B8Nq0xalECistQAnfapEYw5K-qbI_q3urEoPX64d5-kr4efnG2d7-hdpeCGoF9VgdFvZNPqcHWh0LX3Tx2-hWE6L-OHOso4aGHphUySTQWoe5uY1s71mwRuchAcGjRTJqMUXsnzo4ZoADmyiWTfbCkqXCF43zEsqhUkVDY9IP7OnwTyzl7_bnVMZFw?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mTfZyJ4BcQZ8KY5ICv7xv4Gz222v94ZagjT1FVbVWItRkdmZuekb3V1yy6Reheew_oANBpceSU25seMo8YD3KG2pLPMAQi6U06bW4gFaL7IAkOVZaIredP4TVvXso80H-jxT8xkzTRyuAR8OPqcWbiKGTLiuxoihd58wKukBfAHpr0rFScwEaO99C8Z_4vbPsMNHUuKWsgzksoeRffNczyw?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mwTrPF1OXX3gF1kOoGzn0pRhmx_IQ8M5gGDKlEDPc07fJf54v6R2UAVoEwgvkyTqQKGMRG2sEEJi20tBxRXkPK4DsyuC49Wt9-NDf_MyGP9rAJTHtvNALyHBp-Z8AeBHNo_QHpI80HXMuVi8tYXsQScShEKayWujpUA0GgE_qVr87RBtdMup7Jrq0CobaB77bBsX-JN8JE_q1pf2cVzUkbg?encodeFailures=1&width=1102&height=1654'
                },
                {
                    src: 'https://ams03pap002files.storage.live.com/y4mDKNm7CmNAcZa7NWBI_xUHslgSXXe6tgzko0TkRs5fHvMyPUoOzbOWoUQ7BJKcFhR9kB5glXVHOh7zp3-mvHUYtfeDNvdC6R3AGSFSZQw4CNftdXjEQPyHBL2CcKmKR5m68_aMf7l3Ay2LsftXaUyXncM7hQv8bwH78xLQY6gAUkMhAoYXKwocgKUYGO7FDhAuN-nO9ZNyIjVfFtzPSaKnw?encodeFailures=1&width=2481&height=1654'
                }
                ]
            }
        },
    }
</script>
  