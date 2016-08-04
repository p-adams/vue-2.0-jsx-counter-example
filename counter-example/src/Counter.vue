<script>
    export default{
        name: 'Counter',
        props: ['count'],
        data(){
            return{
                c : this.count
            }
        },
        methods: {
            inc(){
                this.c++
            },
            dec(){
                this.c--
            }
        },
        render(h){
            return(
                <div>
                    <h2>Count: {this.c}</h2>
                    <button on-click={this.dec}>-</button>
                    <button on-click={this.inc}>+</button>
                </div>
            )
        }
    }
</script>