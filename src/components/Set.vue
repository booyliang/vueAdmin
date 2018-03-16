<template>
  <div>Set</div>
</template>
<script>
export default{
    methods: {
      set() {
          const set = new Set([1, 2, 3, 4, 4]);
          console.log([...set]); // 去重
      },

      // class
      newClass(value) {
          class Bar {
              doStuff() {
                  console.log('sthff');
              };
              getName(value) {
                  console.log(value)
              }
          }
          let b = new Bar();
          b.doStuff();
          b.getName(value);
      } 
      
      
    },
    mounted () { 
        this.newClass('ject');
        
    }

}
    
</script>