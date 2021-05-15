<template>
 <header >
        <div class="container-fluid ">
     <div class="row header-row ">
        <div class="col-2 logo">
        <img src="../assets/Logo.png" />
      </div>
      <div class="col-10 col-lg-3 Right">
        <div class="search">
          <i class="fas fa-search"></i>
          <input label="search" placeholder="search" />
        </div>
        <div class="serch-responsive" @click=" stateSearch =! stateSearch">
          <a href="#" class="nav-item nav-link">
            <i class="fas fa-search"></i>
          </a>
          </div>
        <div class="navbar-nav">
          <ul class="navbar-nav-ul">
            <li>
              <a href="#" class="nav-item nav-link"
                ><i class="fa fa-th-large"></i
              ></a>
            </li>
            <li>
              <a href="#" class="nav-item nav-link"
                ><i class="fa fa-signal"></i>
              </a>
            </li>
            <li>
              <a href="#" class="nav-item nav-link"
                ><i class="fa fa-user"></i
              ></a>
            </li>
            <li>
              <a href="#" class="nav-item nav-link"
                ><i class="fa fa-pause"></i
              ></a>
            </li>
          </ul>
        </div>
      </div>
     </div>
  
       <div class="search-responsive-show" v-if=" !stateSearch">
      <input type="text" class="searchTerm" placeholder="search">
      <button type="submit" class="searchButton">
        <i class="fa fa-search"></i>
     </button>
       </div>
   
     </div>

    </header>
</template>
<script>
export default ({
 data() {
    return{
      stateSearch :'true',
    }
  }
})
</script>


<style scoped>
.header-row {
  /* background-color: aqua; */
    display: flex;
  justify-content: space-between;
  align-items: center;
}
header {
  width: calc(100vw - 100px);
  /* height: 40px; */
  margin: 50px auto;

  /* background-color: red; */
}
.logo{
  /* background-color: yellow; */
  padding: 0px !important;
}
.logo img {
  width: 50px;
  height: 31px;
 
  /*background-color: lightpink;*/
}
.Right {
  /* background-color: rebeccapurple; */
  height: 40px;
  display: flex;
  justify-content: end;
}
.search {
  height: 40px;
  background: #e5eaee;
  border-radius: 10px;
  float: left;
}
.search i {
  width: 19px;
  height: 19px;
  color: #dadada;
  margin: 8px;
  /* background-color: lightpink; */
}
.search input {
  height: 40px;
  width: 115px;
  border: none;
  outline: none;
  background: #e5eaee;
  border-radius: 6px;
  color: #b5b5c3;
  font-size: 0.85em;
}
.serch-responsive {
  display: none;
  width: 35px;
  height: 35px;
  height: 35px;
  background: #e5eaee;
  color: #b5b5c3;
  margin-left: 6px;
  align-items: center;
  justify-content: center;
  float: right;
  border-radius: 6px;
}
.serch-responsive i {
  color: #80808f;
}
.search-responsive-show{
  display: none;
  width: calc(100vw - 100px);
  margin: 5px auto;
  padding: 15px ;
  background-color: #fafbfd;
  border-radius:5px;
  box-shadow:-2px 1px 5px 1px  #e5eaee;
 z-index: 10px;
 position: absolute;
 top:50px;
 left:50px;
}
.searchTerm {
  width: calc(100vw - 30px);
  border: 1px solid #e5eaee;
  padding: 5px;
  border-radius: 5px 0 0 5px;
  outline: none;
  color: #9DBFAF;
}
.searchTerm:focus{
  color: #b5b5c3;
}
.searchButton {
  width: 40px;
  height: 36px;
  border: 1px solid #e5eaee;
  background: #e5eaee;
  text-align: center;
  color: #80808f;
  border-radius: 0 5px 5px 0;
  cursor: pointer;
  font-size: 20px;
}
.nav {
  /* background-color: violet; */
  height: 40px;
}
.navbar-nav-ul {
  display: flex;
  flex-direction: row;
  list-style: none;
  padding: 0 !important ;
  /* background-color: seagreen; */
}
.navbar-nav a {
  width: 40px;
  height: 40px;
  background: #e5eaee;
  border-radius: 6px;
  margin-left: 6px;
  display: flex;
  align-items: center;
  justify-content: center;
  float: right;
}
.navbar-nav i {
  color: #80808f;
  font-size: 19px;
}

@media only screen and (max-width: 800px) {
  .search input {
    width: 100px;
  }
}
@media only screen and (max-width: 500px) {
  header {
    width: 100vw ;
     margin:10px 0 ;
  }
  
  .logo{
  /* background-color: yellow; */
  padding: 10px !important;
}
  .logo img {
    width: 34px;
    height: 25px;
   
  }
  .Right,
  .nav {
    height: 35px;
  }
  .navbar-nav a {
    height: 35px;
    width: 35px;
    margin-left: 4px;
  }
  .search {
    /* height: 35px; */
    display: none;
  }
  .serch-responsive {
    display: flex;
    /* justify-content: end; */
    float: left;
  }
  .search-responsive-show{
  display: flex;
  justify-content: center;
  
}
}
</style>