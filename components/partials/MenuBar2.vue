<template>
  <!-- Menu Area Start -->
  <section class="menu-section-area default-menu-area">
    <!--Top Menu-->
    <div class="top-menu bg-different py-2">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-6 col-md-8">
            <div class="header_topbar_info d-flex align-items-center">
              <div class="header_offer">
                <a href="tel:99425211">Hotline: +99 42 52 11</a>
              </div>
              <div class="download_wrap d-flex align-items-center">
                <span class="mr-2">Download App</span>
                <ul class="icon_list text-center text-lg-left d-flex align-items-center">
                  <li><a href="https://www.apple.com/shop" target="_blank"><i class="fab fa-apple"></i></a></li>
                  <li><a href="https://play.google.com/store" target="_blank"><i class="fab fa-android"></i></a></li>
                </ul>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-md-4">
            <div class="d-flex align-items-center justify-content-center justify-content-md-end">

              <b-dropdown id="dropdown-1" class="lng_dropdown">
                <template #button-content class="bg-transparent">
                  <img :src="require('@/assets/images/eng.png')" alt="english">English<i class="fas fa-angle-down"></i>
                </template>
                <b-dropdown-item><img :src="require('@/assets/images/eng.png')" alt="english">English</b-dropdown-item>
                <b-dropdown-item><img :src="require('@/assets/images/fn.png')" alt="France">France</b-dropdown-item>
                <b-dropdown-item><img :src="require('@/assets/images/us.png')" alt="United States">United States</b-dropdown-item>
              </b-dropdown>

              <b-dropdown id="dropdown-1" class="ml-3 lng_dropdown currency_dropdown">
                <template #button-content class="bg-transparent">
                  USD<i class="fas fa-angle-down"></i>
                </template>
                <b-dropdown-item to="#">USD</b-dropdown-item>
                <b-dropdown-item to="#">EUR</b-dropdown-item>
                <b-dropdown-item to="#">GBR</b-dropdown-item>
              </b-dropdown>

            </div>
          </div>
        </div>
      </div>
    </div>

    <!--Middle Menu-->
    <div class="middle-menu py-2">
      <div class="container">
        <div class="row">
          <div class="col-12 d-flex justify-content-between align-items-center">
            <nuxt-link to="/fashion" class="navbar-brand">
              <img :src="require('@/assets/images/logo.png')" alt="logo">
            </nuxt-link>
            <ProductSearch />
            <ul class="attr-nav d-flex align-items-center">
              <b-dropdown id="dropdown-1" class="cart_dropdown middle-menu-dropdown">
                <template #button-content class="bg-transparent">
                  <i class="fas fa-cart-arrow-down"></i>
                  <span class="cart_count">2</span>
                </template>

                <div class="cart_list">

                  <b-dropdown-item to="/product-details">
                    <img :src="require('@/assets/images/fashion/1.jpg')" class="mr-3" alt="product">
                    <div class="media-body">
                      <h6 class="mt-0 mb-1 d-flex justify-content-between align-items-center font-14 text-capitalize"><span>Ladis Tops</span><i class="fas fa-times"></i></h6>
                      <p>1x$80.00</p>
                    </div>
                  </b-dropdown-item>

                  <b-dropdown-item to="/product-details/left-thumb">
                    <img :src="require('@/assets/images/fashion/2.jpg')" class="mr-3" alt="product">
                    <div class="media-body">
                      <h6 class="mt-0 mb-1 d-flex justify-content-between align-items-center font-14 text-capitalize"><span>Coat</span><i class="fas fa-times"></i></h6>
                      <p>1x$20.00</p>
                    </div>
                  </b-dropdown-item>

                  <div class="cart_footer">
                    <p class="cart_total d-flex align-items-center justify-content-between">
                      <strong>Subtotal:</strong>
                      <span class="cart_price">
                      <span class="price_symbole">$100.00</span></span>
                    </p>
                    <p class="cart_buttons d-flex justify-content-center">
                      <nuxt-link class="small-button theme-button rounded view-cart" to="/cart">View Cart</nuxt-link>
                      <nuxt-link to="/checkout" class="small-button theme-button rounded checkout">Checkout</nuxt-link>
                    </p>
                  </div>

                </div>
              </b-dropdown>

              <b-dropdown id="dropdown-2" class="middle-menu-dropdown notification_dropdown">
                <template #button-content class="bg-transparent">
                  <i class="far fa-bell"></i>

                  <span class="cart_count">2</span>
                </template>

                <div class="cart_list notification_dropdown_list">

                  <b-dropdown-item to="#" class="media position-relative">
                    <div class="mr-3"><i class="far fa-bell"></i></div>
                    <div class="media-body d-flex justify-content-align-content-between">
                      <div class="notification-content pr-4">
                        <p class="font-14 text-break" style="white-space: pre-line"><strong>Morgan Mor</strong> says something about him. Says something....</p>
                        <p class="font-12"><i class="far fa-clock"></i> 1 day</p>
                      </div>
                      <div class="notification-buttons fon-12 d-flex flex-column justify-content-around">
                        <i class="fas fa-times"></i>
                        <i class="fas fa-check-circle"></i>
                      </div>
                    </div>
                  </b-dropdown-item>

                  <b-dropdown-item to="#" class="media position-relative">
                    <div class="mr-3"><i class="far fa-bell"></i></div>
                    <div class="media-body d-flex justify-content-align-content-between">
                      <div class="notification-content pr-4">
                        <p class="font-14 text-break" style="white-space: pre-line"><strong>Jenifar Lee</strong> says something about him. Says something....</p>
                        <p class="font-12"><i class="far fa-clock"></i> 1 day</p>
                      </div>
                      <div class="notification-buttons fon-12 d-flex flex-column justify-content-around">
                        <i class="fas fa-times"></i>
                        <i class="fas fa-check-circle"></i>
                      </div>
                    </div>
                  </b-dropdown-item>

                  <b-dropdown-item to="#" class="media position-relative">
                    <div class="mr-3"><i class="far fa-bell"></i></div>
                    <div class="media-body d-flex justify-content-align-content-between">
                      <div class="notification-content pr-4">
                        <p class="font-14 text-break" style="white-space: pre-line"><strong>Asif Ak</strong> says something about him. Says something....</p>
                        <p class="font-12"><i class="far fa-clock"></i> 1 day</p>
                      </div>
                      <div class="notification-buttons fon-12 d-flex flex-column justify-content-around">
                        <i class="fas fa-times"></i>
                        <i class="fas fa-check-circle"></i>
                      </div>
                    </div>
                  </b-dropdown-item>

                  <div class="text-center see-all-btn"><nuxt-link to="/my-account/notifications" class="small-button theme-button rounded">See all</nuxt-link></div>

                </div>
              </b-dropdown>

              <b-dropdown id="dropdown-3" class="middle-menu-dropdown user_dropdown">
                <template #button-content class="bg-transparent">
                  <i class="far fa-user"></i>
                </template>

                <div class="cart_list user_dropdown_list">
                  <!--  For Authenticate Users -->
                  <span>
                    <b-dropdown-item to="/my-account">
                      <div class="mr-3"><i class="far fa-smile"></i></div>
                      <div class="media-body">
                        <p>Manage my account</p>
                      </div>
                    </b-dropdown-item>

                    <b-dropdown-item to="/my-account/wishlist">
                      <div class="mr-3"><i class="far fa-heart"></i></div>
                      <div class="media-body">
                        <p>My wishlist</p>
                      </div>
                    </b-dropdown-item>

                    <b-dropdown-item to="/my-account/my-reviews">
                      <div class="mr-3"><i class="far fa-star"></i></div>
                      <div class="media-body">
                        <p>My reviews</p>
                      </div>
                    </b-dropdown-item>

                    <b-dropdown-item to="/my-account/my-orders/">
                      <div class="mr-3"><i class="far fa-times-circle"></i></div>
                      <div class="media-body">
                        <p>My Orders</p>
                      </div>
                    </b-dropdown-item>
                    
                    <b-dropdown-item to="/my-account/auth/registration">
                      <div class="mr-3"><i class="far fa-user"></i></div>
                        <div class="media-body">
                          <p>Signup</p>
                        </div>
                    </b-dropdown-item>

                    <b-dropdown-item to="/my-account/auth/login">
                      <div class="mr-3"><i class="fas fa-key"></i></div>
                        <div class="media-body">
                          <p>Login</p>
                        </div>
                    </b-dropdown-item>

                    <b-dropdown-item to="/">
                      <div class="mr-3"><i class="fas fa-sign-out-alt"></i></div>
                      <div class="media-body">
                        <p>Logout</p>
                      </div>
                    </b-dropdown-item>
                  </span>
                  
                </div>
              </b-dropdown>

            </ul>
          </div>
        </div>
      </div>
    </div>

    <!--Bottom Menu-->
    <div class="bottom-menu bg-dark">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <nav id="mainNav" class="navbar navbar-expand-lg">

              <div class="col-md-3 col-lg-3 pl-0">
                <div class="mr-1 h-100">
                  <!-- Categories Nav Dropdown for Desktop -->
                  <b-dropdown id="categories_nav_dropdown" class="all-categories-button w-100  bg-red px-3 categories_nav_dropdown">
                    <template #button-content class="bg-transparent">
                      <h6><i class="fas fa-bars mr-2"></i><span>All categories</span></h6><i class="fas fa-angle-down ml-2"></i>
                    </template>
                    <ParentCategoryList />
                  </b-dropdown>
                </div>
              </div>

              <div class="col-md-9 col-lg-9 p-0">
                <div class="collapse navbar-collapse" id="main_menu_wrap">

                  <ul class="navbar-nav ml-auto my-2 my-lg-0">
                    
                    <li class="nav-item">
                      <nuxt-link to="#" class="nav-link">Home<i class="fas fa-angle-down ml-2"></i></nuxt-link>
                      <div class="submenu">
                        <ul>
                          <li><nuxt-link to="/fashion">Fashion</nuxt-link></li>
                          <li><nuxt-link to="/electronics">Electronics</nuxt-link></li>
                          <li><nuxt-link to="/furniture">Furniture</nuxt-link></li>
                          <li><nuxt-link to="/groceries">Groceries</nuxt-link></li>
                        </ul>
                      </div>
                    </li>
                    <li class="nav-item">
                      <nuxt-link class="nav-link" to="/shops">Shop</nuxt-link>
                    </li>
                    <li class="nav-item">
                      <nuxt-link to="#" class="nav-link">Products<i class="fas fa-angle-down ml-2"></i></nuxt-link>
                      <div class="submenu">
                        <ul>
                          <li><nuxt-link to="/search-results">Left Sidebar</nuxt-link></li>
                          <li><nuxt-link to="/search-results/right-sidebar">Right Sidebar</nuxt-link></li>
                          <li><nuxt-link to="/best-sellers">No Sidebar</nuxt-link></li>
                          <li><a href="javascript: void(0);">Product Details<i class="fas fa-angle-right ml-2"></i></a>
                            <ul class="submenu">
                              <li><nuxt-link to="/product-details">Style 1</nuxt-link></li>
                              <li><nuxt-link to="/product-details/left-thumb">Style 2</nuxt-link></li>
                              <li><nuxt-link to="/product-details/right-thumb">Style 3</nuxt-link></li>
                            </ul>
                          </li>
                        </ul>
                      </div>
                    </li>
                    <li class="nav-item">
                      <nuxt-link to="#" class="nav-link">Pages<i class="fas fa-angle-down ml-2"></i></nuxt-link>
                      <div class="submenu">
                        <ul>
                          <li><nuxt-link to="/about-us">About Us</nuxt-link></li>
                          <li><nuxt-link to="/contact-us">Contact Us</nuxt-link></li>
                          <li><nuxt-link to="/news-feed/">News Feeds</nuxt-link></li>
                          <li><nuxt-link to="/faq">FAQ</nuxt-link></li>
                          <li>
                            <a href="javascript: void(0);">Account<i class="fas fa-angle-right ml-2"></i></a>
                            <ul class="submenu">
                              <li><nuxt-link to="/my-account">Dashboard</nuxt-link></li>
                              <li><nuxt-link to="/my-account/address-book">Address Book</nuxt-link></li>
                              <li><nuxt-link to="/cart">Cart</nuxt-link></li>
                              <li><nuxt-link to="/my-account/wishlist">Wishlist</nuxt-link></li>
                              <li><nuxt-link to="/checkout">Checkout</nuxt-link></li>
                              <li><nuxt-link to="/compare">Compare</nuxt-link></li>
                              <li><nuxt-link to="/my-account/my-orders">My Orders</nuxt-link></li>
                              <li><nuxt-link to="/my-account/my-reviews">My Reviews</nuxt-link></li>
                              <li><nuxt-link to="/my-account/wallet">Wallet Service</nuxt-link></li>
                              <li><nuxt-link to="/my-account/notifications">Notifications</nuxt-link></li>
                            </ul>  
                          </li>
                          <li>
                            <a href="javascript: void(0);">Authentication<i class="fas fa-angle-right ml-2"></i></a>
                            <ul class="submenu">
                              <li><nuxt-link to="/my-account/auth/login">Login</nuxt-link></li>
                              <li><nuxt-link to="/my-account/auth/registration">Register</nuxt-link></li>
                              <li><nuxt-link to="/my-account/auth/forget-password">Forget Password</nuxt-link></li>
                              <li><nuxt-link to="/my-account/auth/reset-password">Reset Password</nuxt-link></li>
                              <li><nuxt-link to="/my-account/auth/verify-email-address">Verify Email Address</nuxt-link></li>
                              <li><nuxt-link to="/my-account/auth/verify-mobile-no">Verify Mobile No.</nuxt-link></li>
                              <li><nuxt-link to="/my-account/auth/verify-otp">Verify OTP</nuxt-link></li>
                            </ul>  
                          </li>
                          <li>
                            <a href="javascript: void(0);">Merchant Account<i class="fas fa-angle-right ml-2"></i></a>
                            <ul class="submenu">
                              <li><nuxt-link to="/merchant-account">Dashboard</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/products">Products</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/products/add-product">Add Products</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/orders">Orders</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/profile">Profile</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/settings">Settings</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/login">Login</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/registration">Registration</nuxt-link></li>
                              <li><nuxt-link to="/merchant-account/forget-password">Forget Password</nuxt-link></li>
                            </ul>  
                          </li>
                          <li><nuxt-link to="/terms-and-conditions">Terms & Conditions</nuxt-link></li>
                          <li><nuxt-link to="/return-policy">Return Policy</nuxt-link></li>
                          <li><nuxt-link to="/404">404</nuxt-link></li>
                          <li><nuxt-link to="/coming-soon">Coming Soon</nuxt-link></li>
                        </ul>
                      </div>
                    </li>
                    <li class="nav-item">
                      <nuxt-link to="#" class="nav-link">Blog<i class="fas fa-angle-down ml-2"></i></nuxt-link>
                      <div class="submenu">
                        <ul>
                          <li><nuxt-link to="/blog/">Left Sidebar</nuxt-link></li>
                          <li><nuxt-link to="/blog/right-sidebar">Right Sidebar</nuxt-link></li>
                          <li><nuxt-link to="/blog/no-sidebar">No Sidebar</nuxt-link></li>
                          <li><nuxt-link to="/blog/blog-details">Blog Details</nuxt-link></li>
                        </ul>
                      </div>
                    </li>
                    <li class="nav-item">
                      <nuxt-link to="/merchant-account/login" class="nav-link">Sell on Andshop</nuxt-link>
                    </li>
                    <li class="nav-item">
                      <nuxt-link to="/my-account/my-orders/1" class="nav-link">Track my order</nuxt-link>
                    </li>

                  </ul>
                </div>
              </div>

              <!-- Mobile Device Menu and Buttons Wrap -->
              <div class="mobile_all_menu_container w-100 d-flex align-content-center justify-content-between">

                <!-- Mobile Sidebar Category Menu Left -->
                <b-button v-b-toggle.sidebar_category_menu class="sidebar-menu-button bg-transparent border-0"><i class="fas fa-bars"></i></b-button>

                <!-- Sidebar Mobile Category Menu Left -->
                <b-sidebar id="sidebar_category_menu" left shadow backdrop>
                  <div class="px-3 py-2">
                    <ParentCategoryList />
                  </div>
                </b-sidebar>
                <!-- Mobile Sidebar Category Menu -->

                <div class="mobile_right_menu_wrap d-flex align-content-center">
                  <div class="mobile_menu_search_wrap position-relative mr-3">
                    <ProductSearch />
                  </div>

                  <!-- Sidebar Menu General -->
                    <!-- Sidebar Menu General Button -->
                    <b-button v-b-toggle.sidebar_general_menu class="sidebar-menu-button bg-transparent border-0"><i class="fas fa-bars"></i></b-button>

                    <b-sidebar id="sidebar_general_menu" right shadow backdrop>
                      <div class="px-3 py-2">

                        <ul class="accordion" role="tablist">
                          <li class="mb-0 custom-accordion position-relative">
                            <a v-b-toggle.home class="text-hover-color" href="javascript: void(0);">
                              Home
                              <i class="fas fa-minus accordion-arrow"></i>
                            </a>
                            <b-collapse class="mobile-submenu" id="home" accordion="my-accordion2" role="tabpanel">
                              <li><nuxt-link to="/fashion">Fashion</nuxt-link></li>
                              <li><nuxt-link to="/electronics">Electronics</nuxt-link></li>
                              <li><nuxt-link to="/furniture">Furniture</nuxt-link></li>
                              <li><nuxt-link to="/groceries">Groceries</nuxt-link></li>
                            </b-collapse>
                          </li>

                          <li class="mb-0 custom-accordion position-relative">
                            <nuxt-link to="/shops">Shop</nuxt-link>
                          </li>

                          <li class="mb-0 custom-accordion position-relative">
                            <a v-b-toggle.m-products-dropdown class="text-hover-color" href="javascript: void(0);">
                              Products
                              <i class="fas fa-minus accordion-arrow"></i>
                            </a>
                            <b-collapse class="mobile-submenu" id="m-products-dropdown" accordion="my-accordion2" role="tabpanel">
                              <li><nuxt-link to="/search-results">Left Sidebar</nuxt-link></li>
                              <li><nuxt-link to="/search-results/right-sidebar">Right Sidebar</nuxt-link></li>
                              <li><nuxt-link to="/best-sellers">No Sidebar</nuxt-link></li>
                              <li><nuxt-link to="/product-details">Product Details</nuxt-link></li>
                            </b-collapse>
                          </li>

                          <li class="mb-0 custom-accordion position-relative">
                            <a v-b-toggle.pages class="text-hover-color" href="javascript: void(0);">
                              Pages
                              <i class="fas fa-minus accordion-arrow"></i>
                            </a>
                            <b-collapse class="mobile-submenu" id="pages" accordion="my-accordion2" role="tabpanel">
                              <li><nuxt-link to="/about-us">About Us</nuxt-link></li>
                              <li><nuxt-link to="/contact-us">Contact Us</nuxt-link></li>
                              <li><nuxt-link to="/news-feed/">News Feeds</nuxt-link></li>
                              <li><nuxt-link to="/faq">FAQ</nuxt-link></li>
                              <li class="mb-0 custom-accordion">
                                <div class="m-0 position-relative">
                                  <a v-b-toggle.account class="text-hover-color">Account <i class="fas fa-minus accordion-arrow"></i></a>
                                </div>
                                <b-collapse id="account" class="mobile-submenu">
                                  <ul>
                                    <li><nuxt-link to="/my-account">Dashboard</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/address-book">Address Book</nuxt-link></li>
                                    <li><nuxt-link to="/cart">Cart</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/wishlist">Wishlist</nuxt-link></li>
                                    <li><nuxt-link to="/checkout">Checkout</nuxt-link></li>
                                    <li><nuxt-link to="/compare">Compare</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/my-orders">My Orders</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/my-reviews">My Reviews</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/wallet">Wallet Service</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/notifications">Notifications</nuxt-link></li>
                                  </ul>
                                </b-collapse>
                              </li>
                              <li class="mb-0 custom-accordion">
                                <div class="m-0 position-relative">
                                  <a v-b-toggle.authentication class="text-hover-color">Authentication <i class="fas fa-minus accordion-arrow"></i></a>
                                </div>
                                <b-collapse id="authentication" class="mobile-submenu">
                                  <ul>
                                    <li><nuxt-link to="/my-account/auth/login">Login</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/registration">Register</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/forget-password">Forget Password</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/reset-password">Reset Password</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/verify-email-address">Verify Email Address</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/verify-mobile-no">Verify Mobile No.</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/verify-otp">Verify OTP</nuxt-link></li>
                                  </ul>
                                </b-collapse>
                              </li>
                              <li class="mb-0 custom-accordion">
                                <div class="m-0 position-relative">
                                  <a v-b-toggle.mobile-merchant-dropdown class="text-hover-color">Merchant Account <i class="fas fa-minus accordion-arrow"></i></a>
                                </div>
                                <b-collapse id="mobile-merchant-dropdown" class="mobile-submenu">
                                  <ul>
                                    <li><nuxt-link to="/my-account/auth/login">Login</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/registration">Register</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/forget-password">Forget Password</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/reset-password">Reset Password</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/verify-email-address">Verify Email Address</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/verify-mobile-no">Verify Mobile No.</nuxt-link></li>
                                    <li><nuxt-link to="/my-account/auth/verify-otp">Verify OTP</nuxt-link></li>
                                  </ul>
                                </b-collapse>
                              </li>
                              <li><nuxt-link to="/terms-and-conditions">Terms & Conditions</nuxt-link></li>
                              <li><nuxt-link to="/return-policy">Return Policy</nuxt-link></li>
                              <li><nuxt-link to="/404">404</nuxt-link></li>
                              <li><nuxt-link to="/coming-soon">Coming Soon</nuxt-link></li>

                            </b-collapse>
                          </li>

                          <li class="mb-0 custom-accordion position-relative">
                            <a v-b-toggle.m-blog-dropdown class="text-hover-color" href="javascript: void(0);">
                              Blog
                              <i class="fas fa-minus accordion-arrow"></i>
                            </a>
                            <b-collapse class="mobile-submenu" id="m-blog-dropdown" accordion="my-accordion2" role="tabpanel">
                              <li><nuxt-link to="/blog/">Left Sidebar</nuxt-link></li>
                              <li><nuxt-link to="/blog/right-sidebar">Right Sidebar</nuxt-link></li>
                              <li><nuxt-link to="/blog/no-sidebar">No Sidebar</nuxt-link></li>
                              <li><nuxt-link to="/blog/blog-details">Blog Details</nuxt-link></li>
                            </b-collapse>
                          </li>

                          <li class="mb-0 custom-accordion position-relative">
                            <nuxt-link to="/merchant-account/login">Sell on Andshop</nuxt-link>
                          </li>
                          
                          <li class="mb-0 custom-accordion position-relative">
                            <nuxt-link to="/my-account/my-orders/1">Track my order</nuxt-link>
                          </li>

                        </ul>

                      </div>
                    </b-sidebar>
                  <!-- Sidebar Menu General -->

                </div>
              </div>
              <!-- Mobile Device Menu and Buttons Wrap -->

            </nav>

          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Menu Area End -->
</template>

<script>
  export default {
    name: 'menuBar2',
  }
</script>