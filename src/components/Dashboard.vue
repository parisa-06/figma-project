<template>
  <div class="container-fliud">
    <div class="row g-0 contanet">
      <div class="col tab">
        <ul class="tab-ul row g-0">
          <li class="tab-li active col-12 col-md-6 col-lg-2">
            <p>DASHBOARD</p>
            <p>Amaszing Performance</p>
          </li>
          <li class="tab-li col-12 col-md-6 col-lg-2">
            <p>ACCOUNTING</p>
            <p>Cleanest Accounthing Data</p>
          </li>
          <li class="tab-li col-12 col-md-6 col-lg-2">
            <p>REPORTS</p>
            <p>Fluent User Reports</p>
          </li>
          <li class="tab-li col-12 col-md-6 col-lg-2">
            <p>ORDERS</p>
            <p>Detailed Orders</p>
          </li>
          <li class="tab-li col-12 col-md-6 col-lg-2">
            <p>CUSTOMERS</p>
            <p>Each Customer Data</p>
          </li>
        </ul>
      </div>
    </div>
    <div class="row g-0 buttom-menu-dashboard">
      <button class="buttom-menu active">Dashboard</button>
      <button class="buttom-menu">Ui Features</button>
      <button class="buttom-menu">Form Control</button>
      <button class="buttom-menu">Custom Pages</button>
      <button class="buttom-menu">Ui Elements</button>
    </div>

    <div class="row g-0 widget-all">
      <div
        v-for="item in items"
        :key="item"
        class="col-12 col-lg-4 widget"
        :style="item.image"
      >
        <h6 class="title-heder">{{ item.title }}</h6>
        <p class="title-second">{{ item.titleSecond }}</p>
        <p class="text">{{ item.text }}</p>
      </div>
     
    <div class="col-12 col-lg-4 widget multiple-email">
    <h6>{{imgMultipleEmails.title}}</h6> 

    <h5>{{imgMultipleEmails.titleSecond}}</h5>
    <p>{{imgMultipleEmails.text}}</p>
   <div class="img-multiple-email">
     <div v-for="r in imgMultipleEmails.image" :key="r" class="img-email">
     <img    :src="r.img" alt="">
  </div>
    </div>

    </div>
    <div class="col-12 col-lg-4 widget widget-progress ">
  <div class="progress-img">
    <img src="https://th.bing.com/th/id/R25b6f37df5616f86f5b2a78daf21eed6?rik=kn6pGRM1nJdreQ&pid=ImgRaw" alt="">
  </div>
   <div class="widget-progress-text">
     <p>Keen Themes Admin Templates</p>
     <p>Due: 27 Apr 2020</p>
   </div>
    <h4 class="progress-text">progress</h4>
    <div class="progress" >
   <div class="progress-bar" ></div>
  </div>
  

  <h4 class="text-img-multiple-progress">Team</h4>
  <div class="img-multiple-progress">
  <div  v-for="r in imgMultipleEmails.image" :key="r" class="img-multiple">
     <img    :src="r.img" alt="">
  </div>
    </div>

    </div>
   </div>
 
   

    </div>
</template>

<script>


export default {
 
  data() {
    return {
      items: [
        {
          title: "1.header title script",
          titleSecond: "1.title second script",
          text:
            "1.is data: Craft a headline that is informative and will capture readers.",
          image: {backgroundImage:"url(https://th.bing.com/th/id/OIP.S_wYtvETU6t6m1aI8JSdZAHaHb?pid=ImgDet&w=647&h=649&rs=1)" },
        },
        {
          title: "2.header title script",
          titleSecond: "2.title second script",
          text:
            "2.is data: Craft a headline that is informative and will capture readers.",
          image: {backgroundImage:"url(https://th.bing.com/th/id/R2a7036b905a78d6d15420990acae425d?rik=ZUKRRJVMvmM3mA&riu=http%3a%2f%2fclipart-library.com%2fdata_images%2f220590.png&ehk=VrTcgfRlz5uAdrqe8TyGjq3yqO0dBAEh35S1AXyop4Q%3d&risl=&pid=ImgRaw)",
          },
        },
        {
          title: "3.header title script",
          titleSecond: "3.title second script",
          text:
            "3.is data: Craft a headline that is informative and will capture readers.",
          image: {backgroundImage:"url(https://th.bing.com/th/id/R1425acb6f31d3b512aed253d852576a0?rik=cV6RLAoeh5eVdw&pid=ImgRaw)",
          },
        },
      ],
      imgMultipleEmails:{
          title: '7 Hours Ago',
          titleSecond: 'PitStop - Multiple Email Generator',
          text:'Outlines keep you honest. If stop  indulging in poorly thought-out metaphors driving and keep structure',
        image:[
          {
            img:'https://storage.codacambridge.com/files/personnel/icons/boazdaniel.png',
          
          },
           {
            img:'https://image.flaticon.com/icons/png/512/2793/2793595.png'
           },
            {
            img:'https://insynctechnology.com.au/wp-content/uploads/2020/08/Michael-Zanatta-283x300.png'
           }
        ]
        },
        options: {
    color: '#E91E63',
    strokeWidth: 0.9,
}
  
    };
  },
};
</script>


<style scoped>
* {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.title-heder {
  font-style: normal;
  font-weight: 500;
  font-size: 0.95rem;
  line-height: 24px;
  color: #b5b5c3;
  margin-bottom: 30px;
}
.title-second {
  font-style: normal;
  font-weight: 500;
  font-size: 0.85rem;
  line-height: 21px;
  color: #1bc5bd;
  margin: 15px 0;
}
.text {
  font-style: normal;
  font-weight: 200;
  font-size: 1rem;
  line-height: 25px;
  color: #464e5f;
}
.contanet {
  width: calc(100vw - 100px);
  margin: 0 auto;
}
.tab {
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  background-color: #f0f3f5;
}
.tab-ul {
  display: flex;
  flex-direction: row;
  list-style: none;
  padding: 0px;
}
.tab-li {
  width: calc((100vw - 100px) / 5);
  height: 110px;
  border-bottom: 1px solid #dfdfdf;
  background-color: #f0f3f5;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.tab-li:not(:last-child) {
  border-right: 1px solid #dfdfdf;
}
.tab-li:first-child {
  border-top-left-radius: 5px;
}
.tab-li:last-child {
  border-top-right-radius: 5px;
}
.tab-ul .active {
  background-color: #fff;
  border: none !important;
}
.tab-li p {
  font-size: 0.85rem;
  color: #b5b5c3;
  line-height: 30px;
}
.tab-li p:first-child {
  font-weight: bold;
  color: #464e5f;
}
.buttom-menu-dashboard {
  width: calc(100vw - 100px);
  background-color: #fff;
  padding: 30px 70px;
  margin: 0 auto;
}
/* .buttom-menu-dashboard bottom{
    
} */
.buttom-menu {
  width: 117.48px;
  height: 44px;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 21px;
  /* margin-right: 40px; */
  background-color: #fff;
  border: none;
  color: #80808f;
}
.buttom-menu-dashboard .active {
  background-color: #f3f6f9;
  border-radius: 6px;
  color: #464e5f;
}
.widget {
  width: 413px;
  height: 200px;
  border: 1px solid #dfdfdf;
  border-radius: 5px;
  background-color: #fff;
  padding: 20px;
  background-repeat: no-repeat;
  background-size: 30%;
  background-position: 320px -45px;
  margin-bottom: 20px;
  margin-right: 15px;
}
.widget-all {
  width: calc(100vw - 100px);
  margin: 2px auto;
  padding: 45px 70px;
  background-color: #fff;
  display: flex;
  /* justify-content: space-around; */
}
.multiple-email{
  height: auto !important;
}
.img-multiple-email{
display: flex;
align-items: center;
margin-top: 50px;
margin-bottom: 20px;
}

.multiple-email p{
  font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 21px;

color: #80808F;
}
.multiple-email h5{
font-style: normal;
font-weight: 400;
font-size: 22px;
line-height: 33px;
color: #212121;
margin-bottom: 15px;
}
.multiple-email h6{
  font-style: normal;
font-weight: 100;
font-size: 14px;
line-height: 21px;
color: #B5B5C3;
margin-top: 15px;
margin-bottom: 40px;
}

.img-multiple-email img{
  width:40px;
  height: 40px;
    margin: 0 auto;
}
.img-email{
  width: 50px;
  height: 50px;
  background-color: #e5eaee;
  border-radius: 10px;
  margin-right: 10px;
  display: flex;
 align-items: flex-end;

}
.widget-progress{
  height: auto  !important;
}

.progress-img{
  width: 80px;
  height: 80px;
background: #D7F9EF;
border-radius: 12px;
  margin-right: 10px;
  float: left;
  display: flex;
  align-items: center;
  justify-content: center;
}
.progress-img img{
 width:50px;
  height: 50px;
  margin: 0 auto;
}
.widget-progress-text :first-child{
  font-style: normal;
font-weight: 600;
font-size: 17px;
line-height: 25px;
color: #212121;
margin-bottom: 10px;
}
.widget-progress-text :last-child{
  font-style: normal;
font-weight: 500;
font-size: 14px;
line-height: 21px;
margin-bottom: 50px;
color: #B5B5C3;
}
.text-img-multiple-progress{
  font-weight: 600;
font-size: 14px;
line-height: 21px;
color: #212121;
margin-bottom: px;
}
.progress-bar{
width:70%;
height:6px ;
background: #0BB783;
border-radius: 5px;
}
.progress{
  height:6px;
  background: #D7F9EF;
border-radius: 5px;
margin-bottom: 40px;
}
.progress-text{
  font-weight: 600;
font-size: 14px;
line-height: 21px;
color: #212121;
margin-bottom: 15px;
}
.img-multiple-progress img{
  width: 50px;
  height: 50px;
}
.img-multiple{
 background-color: #D7F9EF;
  border-radius: 10px;
   margin-right: 10px;
}
.img-multiple-progress{
width: 50px;
  height: 50px;
display: flex;
  
}

@media only screen and (max-width: 800px) {
  .tab-li {
    width: calc(100% / 2);
    /*border-right: 1px solid #dfdfdf; */
    border-left: 1px solid #dfdfdf;
  }
  .tab-li:last-child {
    border-right: 1px solid #dfdfdf;
    border-top-right-radius: 0px !important;
    border-bottom-right-radius: 5px;
    border-bottom-left-radius: 5px;
  }
  .widget{
    background-position: 330px -37px;
    margin: 15px auto;
  }
}
@media only screen and (max-width: 500px) {
  .contanet {
    width: 100vw;
    padding: 10px;
  }
  .tab-li {
    width: 100vw;
    border-right: 1px solid #dfdfdf;
    border-left: 1px solid #dfdfdf;
  }
  .tab-li:first-child {
    border-top: 1px solid #dfdfdf;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
  }
  .tab-li:last-child {
    border-top-right-radius: 0px !important;
    border-bottom-right-radius: 5px;
    border-bottom-left-radius: 5px;
  }
  .buttom-menu-dashboard {
    width: 90vw;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .buttom-menu {
    margin: 0 auto;
  }
  .widget-all {
    width: 90vw;
      padding: 45px 10px;
  }
  .widget{
    height: auto;
    margin: 15px auto;
    background-position: 240px -27px;
  }
}
</style>