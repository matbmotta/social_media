<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="primary">
      <b-navbar-brand href="#">Social Media</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Link</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
              <div class="h2 mx-3 mb-0" variant="primary">
                <b-icon-person></b-icon-person>
              </div>
              <b-iconstack font-scale="3">
                <b-icon stacked icon="circle-fill" variant="primary"></b-icon>
                <b-icon stacked icon="bell-fill" scale="0.5" variant="white"></b-icon>
                <b-icon stacked icon="circle" variant="primary"></b-icon>
              </b-iconstack>
          </b-nav-form>

          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template v-slot:button-content>
              <em>User</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <section class="section section-shaped section-lg my-0" style="height: 100vh">
        <div class="shape shape-style-1 bg-gradient-default">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div class="container-fluid py-0 lg-md">
            <div class="row justify-content-center">
              <div class="col-md-3">
                 <card type="secondary" shadow
                          header-classes="bg-white pb-5"
                          body-classes="px-lg-2 py-lg-2"
                          class="border-0">
                        <template>
                          <div>
                            <div class="my-3"> 
                             <img src="https://demos.creative-tim.com/argon-design-system-pro/assets/img/faces/team-4.jpg" alt="Raised circle image" class="img-fluid rounded-circle shadow-lg" style="width: 100px;">
                             <p class="mt-3">Ana Júlia</p>
                             </div>
                          </div>
                        </template>
                        <hr> 
                        <template>
                           <div class="accordion" role="tablist">
                            <b-card no-body class="mb-1">
                              <b-card-header header-tag="header" class="p-1" role="tab">
                                <b-button block v-b-toggle.accordion-1 variant="primary">Amigos</b-button>
                              </b-card-header>
                              <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
                                <b-card-body>
                                  <b-input-group size="sm" class="mb-2">
                                    <b-input-group-prepend is-text>
                                      <b-icon icon="search"></b-icon>
                                    </b-input-group-prepend>
                                    <b-form-input type="search" placeholder="Search"></b-form-input>
                                  </b-input-group>
                                  <div>
                                    <p>Suggestions<p/>
                                    <div>
                                      <b-avatar variant="primary" icon="people-fill" size="lg"></b-avatar>
                                    </div>
                                  </div>  
                                </b-card-body>
                              </b-collapse>
                            </b-card>

                            <b-card no-body class="mb-1">
                              <b-card-header header-tag="header" class="p-1" role="tab">
                                <b-button block v-b-toggle.accordion-2 variant="primary">Planos</b-button>
                              </b-card-header>
                              <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
                                <b-card-body>
                                  <b-card-text></b-card-text>
                                </b-card-body>
                              </b-collapse>
                            </b-card>

                            <b-card no-body class="mb-1">
                              <b-card-header header-tag="header" class="p-1" role="tab">
                                <b-button block v-b-toggle.accordion-3 variant="primary">Anúncios</b-button>
                              </b-card-header>
                              <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
                                <b-card-body>
                                   <div>
                                    <b-card
                                      title="Card Title"
                                      img-src="https://picsum.photos/600/300/?image=25"
                                      img-alt="Image"
                                      img-top
                                      tag="article"
                                      style="max-width: 20rem;"
                                      class="ml-5">
                                      <b-card-text>
                                        Some quick example text to build on the card title and make up the bulk of the card's content.
                                      </b-card-text>
                                      <b-button href="#" variant="primary">Go somewhere</b-button>
                                    </b-card>
                                  </div>
                                </b-card-body>
                              </b-collapse>
                            </b-card>
                          </div> 
                        </template>
                        <hr>
                        <template>
                         
                        </template>
                    </card>
                </div>
                <div class="col-md-6">
                    <card type="secondary" shadow
                          header-classes="bg-white pb-5"
                          body-classes="px-lg-2 py-lg-2"
                          class="border-0">
                        <template>
                          <posts></posts>
                        </template>
                        <template>
                          <p>footer</p>
                        </template>
                    </card>
                </div>
                <div class="col-md-3">
                   <card type="secondary" shadow
                          header-classes="bg-white pb-5"
                          body-classes="px-lg-2 py-lg-2"
                          class="border-0">
                        <template>
                            <div>
                              <b-embed
                                type="iframe"
                                aspect="4by3"
                                src="https://www.youtube.com/embed/zpOULjyy-n8?rel=0"
                                allowfullscreen
                              ></b-embed>
                            </div>
                        </template>
                        <hr>
                        <template>
                            
                        </template>
                        <hr>
                        <template>
                          <p>askdjaspjd</p>
                        </template>
                    </card>
                </div>
            </div>
        </div>  
    </section>
  </div>
</template>

<script>
import Posts from '@/components/Custom/Posts.vue'


export default {
  name: 'About',
  components: {
    Posts,
  },
};
</script>
<style scoped>
  .card-body{
    padding: 0.7rem;
  }
  .teste{
    margin-top: 0px;
  }
</style>