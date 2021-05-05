

<template>
  <div class="hello">
    <button class="main__btn">Launch Octopy</button>
    <button class="main__btn2">Launch Octopy</button>
  </div>
</template>


<script>
export default {
  name: 'Button',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/* Knap1 */

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

/* Knap2 */

.main__btn2 {background-image: linear-gradient(to right, #FF512F 0%, #F09819  51%, #FF512F  100%)}
.main__btn2 {


   text-align: center;
   text-transform: uppercase;
   transition: 0.5s;
   background-size: 200% auto;
   color: white;
   box-shadow: 0px 4px 5px 0px rgba(0, 0, 0, 0.10),
   0px 5px 20px 0px rgba(0, 0, 0, 0.10);
   display: block;
   text-decoration: none;
   display: inline-block;
   padding: 0.7375em 0.99em;
   border-radius: 2em;
   font-size: 14px;
   margin: 0.5em 0;
   padding-bottom: 0.7375em;
   box-shadow: 0px 4px 5px 0px rgba(0, 0, 0, 0.10),
   0px 1px 20px 0px rgba(0, 0, 0, 0.10);
   border: none;
   cursor: pointer;
 }

 .main__btn2:hover {
   background-position: right center; /* changes the direction of the grad on button */
   color: #fff;
   text-decoration: none;
   box-shadow: 0px 0px #888888;
   }

/* Styles */

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