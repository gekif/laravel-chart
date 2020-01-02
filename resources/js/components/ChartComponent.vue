<script>

    import {Line} from 'vue-chartjs';

    export default {
        extends: Line,

        data() {
            return {
                url: 'http://chart.dev/products',
                years: [],
                labels: [],
                prices: [],
                data: ''
            }
        },

        methods: {
            getProducts() {
                axios.get(this.url).then((response) => {
                    console.log(response.data);
                });
            }
        },

        mounted() {
            this.getProducts();
        }
    }
</script>