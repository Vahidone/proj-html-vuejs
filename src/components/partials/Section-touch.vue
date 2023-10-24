
<script>
import store from '../../data/store'
export default {
  name: 'SectionTouch',
  data() {
    return {
      store
    }
  }

}
</script>

<template>
  <section>
    <div class="container">
      <div class="left">
        <h6>SEND A MESSAGE</h6>

        <h1>Get in</h1>
        <h1 class="h1-b">Touch</h1>

        <p>We will respond to your messsage as soon as possible</p>

        <div class="my-form">
          <div class="row">
            <div class="col-6">
              <div class="mb-3">
                <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="Name">
              </div>
            </div>

            <div class="col-6">
              <div class="mb-3">
                <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Email">
              </div>
            </div>

            <div class="col-6">
              <div class="mb-3">
                <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="Phone">
              </div>
            </div>

            <div class="col-6">
              <select class="form-select" aria-label="Default select example">
                <option selected>More Info</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
            </div>
          </div>
        </div>


        <div class="mb-3">
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3" placeholder="Message"></textarea>
        </div>

        <button class="btn_green">SEND</button>
      </div>

      <div class="right">
        <h4 class="fw-bold">Example Inc.</h4>
      
        <ul>
          <li v-for="(item, index) in store.listArrExampleTouch" :key="index"><p v-if="item.text">{{ item.text }}</p><a :href="item.href"><i v-if="item.icon" :class="item.icon"></i>{{ item.info }}</a></li>
         
        </ul>

        <button class="btn_white bg-white">VIEW MAP</button>
      </div>
    </div>

  </section>
  
</template>


<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
section {
  height: 850px;
  background-color: white;
    .container {
      display: flex;
      height: $h-100;
      .left {
        width: 60%;
        height: $h-100;
        padding: 100px 0;
        h6 {
          color: #068283;
          margin-bottom: 20px;
        }
        h1 {
          font-weight: bold;
          display: inline-block;
        }
        
        .h1-b {
          color: #068283;
          margin-left: 10px;
          font-size: 3rem;
          font-weight: bold;
          background-color: #D9EBED;
          padding: 4px 8px;
        }
        p {
          color: gray;
          padding: 20px 0 50px 0;
        }
        .my-form {
          div {
            input {
              background-color: #ECECEC;
              height: 50px;
                &::placeholder {
                  color: gray;
                }
            }
            select {
              background-color: #ECECEC;
              color: gray;
              height: 50px;
            }
          }
        }

        textarea {
          background-color: #ECECEC;
          height: 150px;
            &::placeholder {
              color: gray;
            }
          
        }

          
      }
      .right {
        text-align: start;
        width: 40%;
        height: $h-100;
        padding: 100px 50px;
          p {
            color: gray;
            margin: 30px 0;
          }
          ul {
            padding-left: 0;
            li {
              margin: 30px 0;
              a {
                color: #508d8d;
                  i {
                    color: #068283;
                    margin-right: 10px;
                    background-color: #D9EBED;
                    font-size: 1.2rem;
                    padding: 13px;
                    border-radius: 50%;
                  }
              }
            }

          }
          
      }

    }
 
}


</style>