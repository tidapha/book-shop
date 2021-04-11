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
    <div class="container">
      <carousel :nav="false" :dots="false" :items="1">
        <template class="owl-prev" slot="prev">
          <img class="prev" src="../assets/img-shipping/owl-left-arrow.png" />
        </template>

        <template class="owl-next" slot="next">
          <img class="next" src="../assets/img-shipping/owl-right-arrow.png" />
        </template>

        <div class="image-crop">
          <img class="" src="../assets/img-shipping/book.png" />
        </div>
        <div class="image-crop">
          <img class="" src="../assets/img-shipping/book.png" />
        </div>
        <div class="image-crop">
          <img class="" src="../assets/img-shipping/book.png" />
        </div>
        <div class="image-crop">
          <img class="" src="../assets/img-shipping/book.png" />
        </div>
        <div class="image-crop">
          <img class="" src="../assets/img-shipping/book.png" />
        </div>
      </carousel>

      <div class="row mt-5">
        <div class="col-6" align="left">
          <h5>สินค้าขายดี</h5>
        </div>
        <div class="col-6" align="right">
          <small> <a href=""> ดูสินค้าขายดีทั้งหมด </a> </small>
        </div>
        <div class="col">
          <carousel
            :nav="false"
            :dots="false"
            :responsive="{
              0: { items: 2 },
              700: { items: 5 },
            }"
          >
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

      <div class="row mt-5">
        <div class="col-6" align="left">
          <h5>สินค้าแนะนำ</h5>
        </div>
        <div class="col-6" align="right">
          <small> <a href=""> ดูสินค้าแนะนำทั้งหมด </a> </small>
        </div>
        <div class="col">
          <carousel
            :nav="false"
            :dots="false"
            :responsive="{
              0: { items: 2 },
              700: { items: 5 },
            }"
          >
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
  name: "Three",
  props: {
    msg: String,
  },
  mounted() {
    let recaptchaScript = document.createElement("script");
    recaptchaScript.setAttribute(
      "src",
      "https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/js/bootstrap.bundle.min.js"
    );
    document.head.appendChild(recaptchaScript);
  },
};
</script>
<style scoped>
.pr-50 {
  padding-right: 50px;
}
.text-title-card {
  font-size: 0.7rem;
}
.owl-next {
  position: relative;
}
.next {
  position: absolute;
  height: 80px;
  right: 80px;
  top: 45%;
  transform: translate(-50%, -50%);
  z-index: 100;
}
.prev {
  color: white;
  height: 80px;
  position: absolute;
  left: 130px;
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
.image-crop {
  width: 100%;
  height: 330px;
  position: relative;
  overflow: hidden;
}
.image-crop img {
  display: inline;
  margin: 0 auto;
  width: 100%;
  height: auto;
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
