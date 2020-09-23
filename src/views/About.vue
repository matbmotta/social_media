<template>
  <div class="teste">
    <section class="section section-shaped section-lg my-0" style="height: 100vh">
        <div class="shape shape-style-1 bg-gradient-default">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div class="container-fluid pt-lg-md">
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
                                <b-button block v-b-toggle.accordion-1 variant="info">Amigos</b-button>
                              </b-card-header>
                              <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
                                <b-card-body>
                                  <b-input-group size="sm" class="mb-2">
                                    <b-input-group-prepend is-text>
                                      <b-icon icon="search"></b-icon>
                                    </b-input-group-prepend>
                                    <b-form-input type="search" placeholder="Search"></b-form-input>
                                  </b-input-group>
                                  <b-card-text></b-card-text>
                                  <b-card-text>{{ text }}</b-card-text>
                                </b-card-body>
                              </b-collapse>
                            </b-card>

                            <b-card no-body class="mb-1">
                              <b-card-header header-tag="header" class="p-1" role="tab">
                                <b-button block v-b-toggle.accordion-2 variant="info">Planos</b-button>
                              </b-card-header>
                              <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
                                <b-card-body>
                                  <b-card-text>{{ text }}</b-card-text>
                                </b-card-body>
                              </b-collapse>
                            </b-card>

                            <b-card no-body class="mb-1">
                              <b-card-header header-tag="header" class="p-1" role="tab">
                                <b-button block v-b-toggle.accordion-3 variant="info">Anúncios</b-button>
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
                            <div>
                             <b-card title="New Post">
                               <b-form-textarea
                                  id="textarea"
                                  v-model="text"
                                  placeholder="Enter something..."
                                  rows="3"
                                  max-rows="6"
                                ></b-form-textarea>
                                <pre class="mt-3 mb-0">{{ text }}</pre>
                                <a href="#" class="card-link">Card link</a>
                                <b-link href="#" class="card-link">Another link</b-link>
                            </b-card>
                          </div>                        
                        </template>
                        <hr>
                        <template>
                          <p>Body</p>
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


export default {
  name: 'About',
  components: {

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