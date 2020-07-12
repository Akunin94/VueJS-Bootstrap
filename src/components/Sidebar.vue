<template>
   <aside class="sidebar col-lg-3">
    <ul class="nav flex-column mb-4">
        <li class="nav-item" v-for="nav in navigation" :key="nav.index">
            <a class="nav-link" :href="nav.link" :class="{ active: nav.active, disabled: nav.disabled }">{{ nav.title }}</a>
        </li>
    </ul>
    <form class="border border-primary p-3 mb-4">
        <div class="form-group">
            <label for="exampleInputEmail1">Email address</label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">  
        </div>
        <button type="submit" class="btn btn-primary">Submit</button>
    </form>
    <div class="text-hide">
        <iframe width="100%" height="200" hspace="0" vspace="0" src="https://autoa.lv/informer/fuel240ru.html" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>
    </div>
   </aside>
</template>

<script>
export default {
  data() {
      return {
          navigation: [
              {
                  title: 'Link1',
                  link: '/test',
                  active: true,
                  disabled: false
              },
              {
                  title: 'Link2',
                  link: '/test1',
                  active: false,
                  disabled: false
              },
              {
                  title: 'Link3',
                  link: '/test2',
                  active: false,
                  disabled: true
              }
          ]
      }
  }
}
</script>

<style>
</style>
