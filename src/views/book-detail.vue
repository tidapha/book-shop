<template>
  <div class="three">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <h1><a class="navbar-brand" href="#">Book</a></h1>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >สินค้าใหม่</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">สินค้าขายดี</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">สินค้าขายดี</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">สินค้าลดราคา</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">สินค้าแนะนำ</a>
            </li>
          </ul>
          <form class="d-flex pr-50">
            <div class="row">
              <div class="col-4 mt-auto mb-auto">
                <img src="../assets/img-shipping/search.png" width="15" />
              </div>
              <div class="col-4 mt-auto mb-auto">
                <img src="../assets/img-shipping/cart.png" width="15" />
              </div>
              <div class="col-4">
                <img src="../assets/img-shipping/user.png" width="50" />
              </div>
            </div>
          </form>
        </div>
      </div>
    </nav>
    <div class="container py-5">
      <div class="row">
        <div class="col-5">
          <img :src="image" width="90%" />
        </div>
        <div class="col-7" align="left">
          <h2>รสชาติของผลไม้ที่ยังไม่สุกงอม</h2>
          <p class="py-2">
            ผู้เขียน : โชนัมจู<br />
            สำนักพิมพ์ : Piccolo<br />
            หมวดหมู่ : วรรณกรรม เรื่องสั้น<br />
            ประเภทของสินค้า : Books<br />
            บาร์โค้ด : 9786161840488
          </p>

          <div class="py-4">
            <span>ราคา</span>
            <h3 class="d-inline px-3">THB499.00</h3>
            <h5 class="d-inline text-muted">THB599.00</h5>
          </div>

          <div class="row py-3">
            <div class="col-md-2">
              <input class="form-control" value="1" type="number" />
            </div>
            <div class="col">
              <button class="btn btn-add">Add</button>
            </div>
            <div class="col">
              <button class="btn btn-wishlist">
                <font-awesome-icon :icon="['fas', 'heart']" />
                <span class="px-2">wishlist</span>
              </button>
            </div>
          </div>

          <div class="row py-2">
            <div class="col-12">
              แชร์ :
              <img src="../assets/img-shipping/social-share.png" width="150" />
            </div>
          </div>
        </div>

        <div class="col-12" align="left">
          <img
            class="px-2 py-2 item-link"
            v-on:click="showImage('book')"
            src="../assets/img-shipping/book.png"
            height="170"
          />

          <img
            class="px-2 py-2 item-link"
            v-on:click="showImage('book-detail')"
            src="../assets/img-shipping/book-detail.png"
            height="170"
          />
        </div>
      </div>

      <ul class="nav nav-tabs py-3" id="myTab" role="tablist">
        <li class="nav-item" role="presentation">
          <button
            class="nav-link active"
            id="home-tab"
            data-bs-toggle="tab"
            data-bs-target="#home"
            type="button"
            role="tab"
            aria-controls="home"
            aria-selected="true"
          >
            เกี่ยวกับสินค้า
          </button>
        </li>

        <li class="nav-item" role="presentation">
          <button
            class="nav-link"
            id="profile-tab"
            data-bs-toggle="tab"
            data-bs-target="#profile"
            type="button"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
          >
            รายละเอียด
          </button>
        </li>
      </ul>
      <div class="tab-content py-3" align="left" id="myTabContent">
        <div
          class="tab-pane fade show active container"
          id="home"
          role="tabpanel"
          aria-labelledby="home-tab"
        >
          <p><b>เกี่ยวกับสินค้า :</b> รสชาติของผลไม้ที่ยังไม่สุกงอม</p>
          <p>
            ก่อนที่ชีวิตของเด็กสาววัยย่างสิบหกปีทั้งสี่คนจะได้สัมผัสกับความหวานหอมจากผลไม้รสชาติที่สุดในชีวิต
            พวกเธอจะต้องต่อสู้กับความจริงปวดที่ค่อยๆ
            กัดเซาะจิตใจและผ่านพ้นช่วงชีวิตซึ่งเต็มไปด้วยความยากลำบากนานา
            ทั้งความคิดที่ว่าตัวเองโดดเดี่ยว
            แม้อยู่ในกลุ่มเพื่อนที่เหมือนจะรักกันดี
            หรือแม้จะมีครอบครัวที่พร้อมหน้า
          </p>
        </div>
        <div
          class="tab-pane fade container"
          id="profile"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <p><b>รายละเอียด :</b> รสชาติของผลไม้ที่ยังไม่สุกงอม</p>
          <p>
            ก่อนที่ชีวิตของเด็กสาววัยย่างสิบหกปีทั้งสี่คนจะได้สัมผัสกับความหวานหอมจากผลไม้รสชาติที่สุดในชีวิต
            พวกเธอจะต้องต่อสู้กับความจริงปวดที่ค่อยๆ
            กัดเซาะจิตใจและผ่านพ้นช่วงชีวิตซึ่งเต็มไปด้วยความยากลำบากนานา
            ทั้งความคิดที่ว่าตัวเองโดดเดี่ยว
            แม้อยู่ในกลุ่มเพื่อนที่เหมือนจะรักกันดี
            หรือแม้จะมีครอบครัวที่พร้อมหน้า
          </p>
          <p>
            ความรู้สึกที่ว่าไม่มีใครจริงใจสักคนนั้นกัดกินจิตใจทีละน้อยจนก่อเกิดความหวาดระแวงขึ้น
            ตอนนี้พวกเธอจึงทำได้เพียงพยายามในแบบของตนเอง
            เพื่อผ่านพ้นความไม่คุ้นเคยที่ยากเข็ญไปให้ได้
            ไม่ว่าวิธีเหล่านั้นจะถูกหรือผิด...
            แล้ววันหนึ่งเมื่อถึงเวลาอาจจะไม่ทั้งหมด
            แต่อย่างน้อยก็จะมีหนึ่งคนที่พูดออกมาได้อย่างเต็มปากเต็มคำว่า
            "นี่เป็นผลไม้อร่อยที่สุดเท่าที่ฉันเคยกินมาตั้งแต่เกิดเลย"
          </p>
        </div>
      </div>

      <div class="row mt-5">
        <div class="col-6" align="left">
          <h5>สินค้าแนะนำ</h5>
        </div>
        <div class="col-6" align="right">
          <small> <a href=""> ดูสินค้าแนะนำทั้งหมด </a> </small>
        </div>
        <div class="col" style="position: relative">
          <carousel
            :nav="false"
            :dots="false"
            :responsive="{
              0: { items: 2 },
              700: { items: 5 },
            }"
          >
            <template class="owl-prev" slot="prev">
              <img
                class="prev"
                src="../assets/img-shipping/owl-left-arrow.png"
              />
            </template>

            <template class="owl-next" slot="next">
              <img
                class="next"
                src="../assets/img-shipping/owl-right-arrow.png"
              />
            </template>
            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>

            <router-link to="/book-detail">
              <div class="card m-1 border-0">
                <div class="card-body">
                  <div class="row">
                    <div class="col-md-12 text-success" align="left">
                      <font-awesome-icon :icon="['fas', 'check-circle']" />
                      มีสินค้า
                    </div>
                  </div>
                  <img
                    class="px-4 py-1"
                    src="../assets/img-shipping/book.png"
                  />
                  <button class="btn btn-add-card mx-auto">
                    <font-awesome-icon :icon="['fas', 'shopping-cart']" />
                    Add To Cart
                  </button>
                  <div class="row">
                    <div class="col-6 small text-warning">
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                      <small
                        ><font-awesome-icon :icon="['fas', 'star']"
                      /></small>
                    </div>
                    <div class="col-6 small text-muted">
                      <small>Reviews (4)</small>
                    </div>
                    <div class="col-12" align="left">
                      <span class="text-title-card">
                        รสชาติของผลไม้ที่ยังไม่สุกงอม</span
                      >
                    </div>
                    <div
                      class="col-12 text-decoration-line-through text-muted small"
                      align="left"
                    >
                      <small>THB599.00</small>
                    </div>
                    <div class="col-12" align="left"><b>THB499.00</b></div>
                  </div>
                </div>
              </div>
            </router-link>
          </carousel>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import carousel from "vue-owl-carousel";
import { library } from "@fortawesome/fontawesome-svg-core";
import { faUserSecret } from "@fortawesome/free-solid-svg-icons";

library.add(faUserSecret);

export default {
  components: { carousel },
  name: "BookDetail",
  props: {
    msg: String,
  },
  data() {
    return {
      image: "",
    };
  },
  mounted() {
    let recaptchaScript = document.createElement("script");
    recaptchaScript.setAttribute(
      "src",
      "https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/js/bootstrap.bundle.min.js"
    );
    document.head.appendChild(recaptchaScript);
    this.getImgUrl("book");
  },
  methods: {
    getImgUrl(pic) {
      var images = require.context("../assets/img-shipping/", false, /\.png$/);
      this.image = images("./" + pic + ".png");
    },

    showImage(img) {
      this.getImgUrl(img);
    },
  },
};
</script>

<style scoped>
.pr-50 {
  padding-right: 50px;
}
.nav-tabs .nav-link:focus,
.nav-tabs .nav-link:hover {
  border-color: #fff #fff #0156ff;
}
.nav-tabs .nav-item.show .nav-link,
.nav-tabs .nav-link.active {
  border: 2px solid;
  border-color: #fff #fff #0156ff;
}
.text-title-card {
  font-size: 0.7rem;
}
.item-link {
  cursor: pointer;
}
.next {
  position: absolute;
  height: 80px;
  right: 20px;
  top: 45%;
  transform: translate(-50%, -50%);
  z-index: 100;
}
.prev {
  color: white;
  height: 80px;
  position: absolute;
  left: 50px;
  top: 45%;
  transform: translate(-50%, -50%);
  z-index: 100;
}

@media (max-width: 768px) {
  .next {
    right: -10px;
  }
  .prev {
    left: 30px;
  }
}
.btn-add {
  color: white;
  width: 209px;
  background: #0156ff;
  border-radius: 50px;
}
.btn-wishlist {
  color: white;
  width: 209px;
  background: #f2994a;
  border-radius: 50px;
}
.card-body:hover .btn-add-card {
  display: block;
}
.btn-add-card {
  border: 2px solid #0156ff;
  box-sizing: border-box;
  border-radius: 50px;
  padding-left: 10px;
  padding-right: 10px;
  font-size: 14px;
  line-height: 21px;
  color: #0156ff;
  display: none;
}
</style>
