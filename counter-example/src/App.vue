
<script>
import Counter from './Counter.vue'
export default {
  data(){
    return{
    }
  },
  render(h){
    const data = {
      props:{
        count: 0
      }
    }
    return(
      <div>
        <Counter {...data}/>
      </div>
    )
  }
}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
}
</style>
