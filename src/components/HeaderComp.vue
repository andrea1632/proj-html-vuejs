<template>
    <div>
        <header>
            <div class="bgBlue">
                <div class="top w80auto">
                <div>
                    <i class="fa-solid fa-clock"></i>
                    <span>
                        Open Hours: Mon-Sat-9:00 - 18:00
                    </span>
                </div>
                <div class="rightTop">
                    <div>
                        <i class="fa-solid fa-phone"></i>
                        <span>
                            +1(305) 1234-5678
                        </span>                       
                    </div>
                    <div>
                        <i class="fa-solid fa-envelope"></i>
                        <span>
                            hello@example.com
                        </span>
                    </div>
                    <div class="topIcons">
                        <a href="https://www.facebook.com/" target="_blank" class="text-decoration-none"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="https://www.twitter.com/" class="text-decoration-none" target="_blank"><i class="fa-brands fa-twitter mx"></i></a>
                        <a href="https://www.linkedin.com/" target="_blank" class="text-decoration-none"><i class="fa-brands fa-linkedin-in"></i></a>
                        
                        
                    </div>
                </div>
            </div>            
            </div>
            <div class="hero">
              <div class="overlay">  
                <div class="w80auto">
                    <div class="topContentHero">
                        <div class="nexgen">
                            <span class="ps-3">
                                nex
                            </span>
                            gen
                        </div>
                        <nav>
                            <ul>
                                <li v-for="elm, i in links" :key="i">
                                    <a :href="'#' + elm.link">{{elm.title}}</a>
                                </li>
                                <!-- <li>
                                    <a href="#">about</a>
                                </li>
                                <li>
                                    <a href="#">projects</a>
                                </li>
                                <li>
                                    <a href="#">process</a>
                                </li>
                                <li>
                                    <a href="#">testimonials</a>
                                </li> -->
                                <li>
                                    <a href="#"><i class="fa-regular fa-user"></i></a>
                                </li>
                                <li>
                                    <button class="btnGreen">
                                        get in touch
                                    </button>
                                </li>
                            </ul>
                        </nav>
                    </div>
                    <div class="mainContentHero">
                        <h4>
                            human resources
                        </h4>
                        <div class="productivity">
                            Get More
                            <div>
                                Productivity
                            </div>                                
                        </div>
                        <p>
                            Planning, recruitment and selection process and performance evaluation of employees
                        </p>
                        <div>
                            <button class="btnGreen">get in touch</button><button class="btnLight">read more</button>
                        </div>
                    </div>
                </div>
              </div>  
            </div>
        </header>
    </div>
</template>

<script>
export default{
    name: 'HeaderComp',
    props: {
        links : Array
    }
}
</script>

<style lang="scss" scoped>
  .top{
      display: flex;
      justify-content: space-between;
      color: #C0C3D0;
      padding: 15px 0;      
          a{
              color: #C0C3D0;
          }      
  }
  .rightTop{
      display: flex;
      width: 30%;
      justify-content: space-between;
  }
  .bgBlue{
     background-color: #21333E;
  }
  .mx{
      margin: 0 20px;
  }
  .hero{
      background-image: url('./../assets/img/bg-4.jpg');
  }
  .nexgen{
      text-transform: uppercase;
      color: #C0C3D0;
      font-weight: 600;
      font-size: 1.2em;
  }
  .nexgen span{
      background-color: #1F3D3D;
      color: #058887;
      padding: 10px;
      border-top-left-radius: 20px;
      border-bottom-left-radius: 20px;    
  }
  nav ul{
      list-style: none;
      display: flex;
      align-items: center;
  }
  ul li a i{
      margin-right: 10px;
  }
  ul li a{
      text-transform: uppercase;
      text-decoration: none;
      color: white;
      margin: 0 20px;
  }
  ul li a:hover{
      color: #00A6A6;
  }
  .topContentHero{
      display: flex;
      justify-content: space-between;
      padding-top: 30px;
  }
  .mainContentHero{
      margin-top: 200px;
      max-width: 60%;
      h4{
          text-transform: uppercase;
          color: #00A6A6;
      }
      .productivity{
          font-size: 5em;
          font-weight: 900;
          color: white;
          div{
            background-repeat: no-repeat;
            background-image: linear-gradient(120deg, #135454 0%, #135454 100%);
            background-size: 50% 0.4em;
            background-position: 6px 70%;
          }
      }
      p{
          color: #929aa3;
          font-size: 1.1em;
          width: 50%;
          padding: 30px 0;
      }
      padding-bottom: 150px;
  }
</style>