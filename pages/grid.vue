<template>
    <div class="grid-container">
        <!-- <div class="grid-item grid-item-1">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro, officiis! Corrupti, molestiae? Dignissimos suscipit alias nemo id voluptates earum in optio repellendus. Laboriosam sit molestias, iusto placeat aliquam error illum blanditiis quod voluptate, nam, minus sunt. Saepe in repellat veniam quo eligendi officiis eveniet vel, quasi dolor voluptatum illo numquam.
        </div>
        <div class="grid-item grid-item-2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore minus labore atque tempore. Reiciendis dolores quibusdam asperiores cupiditate autem possimus incidunt necessitatibus maxime velit iusto!
        </div> -->
                <div class="grid-item grid-item-1"> </div>
        <div class="grid-item grid-item-2"></div>
        <div class="grid-item grid-item-3"></div>
    </div>
</template> 


<style lang="scss" scoped>

.grid-container {
    display: grid;
    grid-template-columns: 200px 250px;
    // grid-template-columns: 2fr 1fr;
    // grid-template-columns: repeat(4, 100px);
    grid-auto-rows: minmax(150px auto);
    grid-gap: 20px;

    // grid-template-rows: 200px 150px;
    // grid-template-areas: 
    // "header header"
    // "sidebar content" 
    // "sidebar content";
    .grid-item-1 {
            // grid-area: header;
            grid-column-start: 1; 
            grid-column-end: -1; 
            // grid-column: 1 / -1;
    } 

    .grid-item-2 {
        // grid-row-start: 2;
        // grid-row-end: 4;
        grid-row: span 4;
    }
}















/* Background Styles Only */

@import url('https://fonts.googleapis.com/css?family=Raleway');

* {
    font-family: Raleway;
}

*, *::before, *::after {
  box-sizing: border-box;
}

html, body {
  background-color: #333;
  height: 100%;
  margin: 0;
}

.grid-container {
  position: relative;
  padding: 20px;
  width: 100%;
}

.grid-item {
  position: relative;
  font-size: 25px;
  padding: 20px;
  padding-top: 50px;
  background-color: #379AD6;
  color: #222;
  border: 1px solid white;
}

.grid-item:nth-child(odd) {
  background-color: #5bbdfa;
}

.grid-item::before {
  content: 'Grid Item';
  position: absolute;
  font-size: 25px;
  font-weight: bold;
  top: 10px;
  left: 15px;
}

.grid-item::after {
  position: absolute;
  font-size: 25px;
  top: 10px;
  right: 15px;
  font-weight: bold;
}

.grid-item-1::after {
  content: '1';
}

.grid-item-2::after {
  content: '2';
}

.grid-item-3::after {
  content: '3';
}

.grid-item-4::after {
  content: '4';
}

.grid-item-5::after {
  content: '5';
}

.grid-item-6::after {
  content: '6';
}

.grid-item-7::after {
  content: '7';
}

.grid-item-8::after {
  content: '8';
}

.grid-item-9::after {
  content: '9';
}

.grid-item-10::after {
  content: '10';
}

.grid-item-11::after {
  content: '11';
}

.side-links {
  position: absolute;
  top: 15px;
  right: 15px;
}

.side-link {
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  margin-bottom: 10px;
  color: white;
  width: 180px;
  padding: 10px 0;
  border-radius: 10px;
}

.side-link-youtube {
  background-color: red;
}

.side-link-twitter {
  background-color: #1DA1F2;
}

.side-link-github {
  background-color: #6e5494;
}

.side-link-text {
  margin-left: 10px;
  font-size: 18px;
}

.side-link-icon {
  color: white;
  font-size: 30px;
}
</style>