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

        mounted() {
            console.log('Component mounted.')
        }
    }
</script>