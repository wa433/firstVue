<template>
  <div>
    <input type="text" v-model="message"><br>
    <p>{{message | capitalize}}</p>
  </div>
</template>

<script>
export default {
  filters:{
          capitalize:function(string){
            if(!string) return '';
            string=string.toString();
            var arrs=string.split(" ");
            return arrs.map(function(arr){
              arr=arr.toString();
              return arr.charAt(0).toUpperCase()+arr.slice(1);
            }).join(" ");
          }
        },
  data:function(){
    return {
      message:"hello world nihao ya"
    }
  }
}
</script>