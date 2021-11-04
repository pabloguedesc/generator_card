<template>
  <div id="Navbar">
    <div class="links">
      <li><a class="btn-link" href="">Sobre</a></li>
      <li><a class="btn-link" href="">Ajuda</a></li>
      <li><a class="btn-link" id="login" href="">Log in</a></li>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#Navbar {
  display: flex;
  flex-direction: row-reverse;
  position: absolute;
  width: 100vw;
  padding: 1rem;
}

.links {
  display: flex;
  margin: 0 5rem;
  width: 300px;
  justify-content: space-between;
}

li {
  list-style: none;
}

.btn-link {
  text-decoration: none;
  color: #ffffff9c;
  padding: 5px;
  border-radius: 8px;
  transition: .3s;
}

.btn-link:hover {
  color: var(--white);
  /* box-shadow: rgba(255, 255, 255, 0.664) 0px 1px 2px 0px, rgba(255, 255, 255, 0.404) 0px 1px 3px 1px; */
}

#login{
  border: .5px solid rgb(130, 111, 173, 0.623);
  box-shadow: rgba(255, 255, 255, 0.178) 0px 1px 2px 0px, rgba(255, 255, 255, 0.185) 0px 1px 3px 1px;
  transition: 0.5s;
}

#login:hover{
  border: 1px solid var(--white);
  box-shadow: rgba(255, 255, 255, 0.664) 0px 1px 2px 0px, rgba(255, 255, 255, 0.911) 0px 1px 3px 1px;
}
</style>