

<template>
  <div class="hello">
    <button class="main__btn">Launch Octopy</button>
  </div>
</template>


<script>
export default {
  name: 'Button',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.main__btn {
    font-family: var(--font-family);
    font-size: 1.3rem;
    font-weight: 700;
    color: var(--offdark);
    background: #a1a1a1;
    background: -webkit-linear-gradient(to right, #44c1ed, #4479ed, #3185df);
    background: linear-gradient(to right, #44c1ed, #4479ed, #3185df);
    padding: 12px 24px;
    border: none;
    border-radius: 2px;
    margin-top: 2rem;
    cursor: pointer;
    position: relative;
    transition: all 0.35s;
    outline: none;
    text-transform: uppercase;
  }

.main__btn a {
    position: relative;
    z-index: 2;
    color: #fff;
    text-decoration: none;
}

.main__btn:after {
    position: absolute;
    content: '';
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: #4479ed;
    transition: all 0.35s;
    border-radius: 4px;
}

.main__btn:hover {
    color: #fff;
}

.main__btn:hover:after {
    width: 100%;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>