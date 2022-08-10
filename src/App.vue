<template>
    <v-app id="inspire">
        <v-app-bar app elevation="0">
            <!-- <v-subheader><h1 class="green--text">Portfolio<span class="pink--text">.in</span></h1></v-subheader> -->
            <v-subheader><h1>Nymur</h1></v-subheader>
            <v-tabs center-active right background-color="transparent" active-class="active-tab">
                <v-tab><a href="#home">Home</a></v-tab>
                <v-tab><a href="#about">About</a></v-tab>
                <v-tab><a href="#education">Education</a></v-tab>
                <v-tab><a href="#experience">Experience</a></v-tab>
                <v-tab><a href="#portfolio">Portfolio</a></v-tab>
                <v-tab><a href="#contact">Contact</a></v-tab>
            </v-tabs>
            <v-btn large color="green" class="white--text ml-10">Send me an Email</v-btn>
        </v-app-bar>
        <v-main style="background-color: #F5F5F5">
            <section class="intro-section" id="home">
                <v-row class="align-center px-10" style="height: 690px">
                    <v-col lg="6" cols="6" class="pa-6 font-weight-bold py-16">
                        <!-- <h2 class="display-3">Visual <span class="green--text">Design</span> & <span class="pink--text">Art</span>
                            Director</h2> -->
                        <h5 class="display-1">Hi, I am <strong>Md. Nymur Rahman.</strong></h5><br>
                        <h5 class="display-1"> <span class="green--text">Software Engineer</span> & <span class="pink--text">Mathematics Teacher</span></h5>
                        <br>
                        <br>
                        <v-btn large elevation="5" color="green" class="white--text mt-10 px-10 py-5">Hire Me</v-btn>
                        <v-btn large elevation="5" color="pink" class="white--text mt-10 ml-10 px-10 py-5">Contact
                        </v-btn>
                        <v-row class="mt-16">
                            <v-chip class="px-4 ma-3" color="#4267B2">
                              <a href="https://www.facebook.com/naym01" target="_blank" class="text-white"><i class="bi-facebook"></i> Facebook</a>
                            </v-chip>
                            <v-chip class="px-4 ma-3 white--text" color="#0072b1">
                                <a href="https://www.linkedin.com/in/md-nymur-rahman-17aaa71ba/" target="_blank" class="text-white"><i class="bi-linkedin"></i> Linkedin</a>
                            </v-chip>
                            <v-chip class="px-4 ma-3" color="#171515">
                                <a href="https://github.com/naym00" target="_blank" class="text-white"><i class="bi-github"></i> GitHub</a>
                            </v-chip>
                            <v-chip class="px-4 ma-3" color="#3f729b">
                                <a href="https://www.instagram.com/naymhsain/" target="_blank" class="text-white"><i class="bi-instagram"></i> Instagram</a>
                            </v-chip>
                        </v-row>
                    </v-col>
                    <v-col lg="6" cols="6">
                        <img src="./assets/my-image.png" class="img-fluid">
                        
                    </v-col>
                </v-row>
            </section>
            <section class="about-me" id="about">
                <v-img class="pa-10" height="400" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                       src="https://thumbs.dreamstime.com/b/technical-network-abstract-background-modern-theme-63068618.jpg">
                    <v-row justify="center" class="align-center">
                        <v-col lg="6" cols="6">
                            <v-card class="text-center pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                                <v-card-subtitle class="display-1"><strong>About Myself</strong></v-card-subtitle>
                                <h5>
                                    Currently I am teaching in an English medium coaching where I teach 
                                    mathematics, additional mathematics, pure mathematics, physics and 
                                    computer.
                                    I also run a YouTube channel named in ‘white board’ where I teach 
                                    mathematics.
                                </h5>

                                <v-btn large elevation="5" color="pink" class="white--text mt-10 px-10 py-5">Download
                                    Resume
                                    <v-icon>mdi-download</v-icon>
                                </v-btn>

                            </v-card>
                        </v-col>
                        <v-col lg="6" cols="6">
                            <v-card class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
                                <div class="py-1" v-for="(item,index) in items" :key="index">
                                    <label>{{ item.title }}</label>
                                    <v-progress-linear
                                            :color="item.color"
                                            height="5"
                                            :value="item.value"
                                    ></v-progress-linear>
                                </div>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-img>
            </section>
            <section class="educaion py-6" id ="education">
                <v-container>
                    <h4 class="display-2 text-center">Education</h4>
                    <v-row class="py-8">
                        <v-col cols="12" lg="6">
                            <v-card class="pa-6 rounded-xl " elevation="5">
                                <div class="d-flex align-center justify-space-between">
                                    <div class="">
                                        <h4>Computer Science and Engineering</h4>
                                        <span><i>April 2016 - April 2020</i></span>
                                    </div>
                                    <a class="green--text">University of Asia Pacific<v-icon color="green">mdi-link</v-icon></a>
                                </div>
                                <v-card-text>
                                    Random Speech Random Speech Random Speech Random Speech Random Speech 
                                    Random Speech Random Speech Random Speech Random Speech Random Speech
                                    Random Speech Random Speech Random Speech Random Speech Random Speech
                                    Random Speech Random Speech Random Speech.
                                </v-card-text>
                            </v-card>
                        </v-col>
                        <v-col cols="12" lg="6">
                            <v-card class="pa-6 rounded-xl " elevation="5">
                                <div class="d-flex align-center justify-space-between">
                                    <div class="">
                                        <h4>Higher Secondary Certificate (HSC)</h4>
                                        <span><i>July 2012 – March 2014</i></span>
                                    </div>
                                    <a class="green--text">Stamford College, Dhaka<v-icon color="green">mdi-link</v-icon></a>
                                </div>
                                <v-card-text>
                                    Random Speech Random Speech Random Speech Random Speech Random Speech 
                                    Random Speech Random Speech Random Speech Random Speech Random Speech
                                    Random Speech Random Speech Random Speech Random Speech Random Speech
                                    Random Speech Random Speech Random Speech.
                                </v-card-text>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-container>
            </section>
            <section class="experiance py-6" id = "experience">
                <v-img class="pa-10" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                       src="https://designshack.net/wp-content/uploads/Home-office.jpg">
                    <v-container>
                        <h4 class="display-2 text-center">Experience</h4>
                        <v-timeline>
                            <v-timeline-item v-for="(exper,index) in experience" :key="index"
                                             :color="index % 2 === 0 ?'pink':'green'">
                                <v-card class="rounded-xl">
                                    <v-card-title :color="index % 2 === 0 ?'pink':'green'">
                                        {{exper.title}}
                                    </v-card-title>
                                    <v-card-text>
                                        <b>{{exper.date}}</b><br>
                                        <b>@{{exper.institute}}</b><br>
                                        {{exper.decription}}
                                    </v-card-text>
                                </v-card>
                            </v-timeline-item>
                        </v-timeline>
                    </v-container>
                </v-img>

            </section>
            <section class="portfolio" id="portfolio">
                <h4 class="display-2 text-center">Portfolio</h4>
                <v-slide-group
                        class="pa-4"
                        active-class="success"
                        show-arrows
                >
                    <v-slide-item v-for="(slider,index) in sliders" :key="index">
                        <v-card height="250" width="250" class="mx-2">
                            <img height="100%" width="100%" :src="slider" alt="">
                        </v-card>
                    </v-slide-item>
                </v-slide-group>
            </section>
            <section class="contact-us pt-10" id="contact">
                <v-img class="pt-10" gradient="to bottom, rgb(166 199 156), rgb(227 227 227 / 86%)" src="https://img.freepik.com/free-photo/contact-us_36325-2135.jpg?size=626&ext=jpg">
                    <v-container>
                        <h3>
                            I am Nayeem Hossain. I always love Mathematics and Programing. My favorite programing languages are C, C++, Python and Assembly. Youtube Channel: 'White Board'.
                        </h3>
                        <v-divider />
                        <br>
                        <v-row>
                            <v-col cols="12" lg="6">
                                <v-card-title><strong>DROP A Message</strong></v-card-title>
                                <v-form>
                                    <v-text-field label="Your Name" />
                                    <v-text-field label="Email" />
                                    <v-text-field label="Subject" />
                                    <v-textarea label="Message" />
                                    <v-btn large color="green" class="white--text">Send Message</v-btn>
                                </v-form>
                            </v-col>
                            <v-col cols="12" lg="3" offset="2">
                                <v-card-title>CONTACT ME</v-card-title>
                                <v-card-text>
                                    Luxmibazar, Old Dhaka, 1100 <br>
                                    +8801794603522 <br>
                                    naymhsain00@gmail.com <br>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn large elevation="5" color="pink" class="white--text mt-10 px-10 py-5">Download
                                        Resume
                                        <v-icon>mdi-download</v-icon>
                                    </v-btn>
                                </v-card-actions>
                            </v-col>
                        </v-row>
                    </v-container>
                    <v-footer class="mt-4">
                        <v-col
                                class="text-center"
                                cols="12"
                        >
                        </v-col>
                    </v-footer>
                </v-img>
            </section>
        </v-main>
    </v-app>
</template>

<script>
    export default {
        name: 'App',

        data: () => ({
            drawer: null,
            items: [
                {title: 'C', value: 100, color: 'light-blue'},
                {title: 'Python', value: 95, color: 'light-blue'},
                {title: 'Django', value: 80, color: 'light-blue'},
                {title: 'C++', value: 80, color: 'light-blue'},
                {title: 'Javascript', value: 70, color: 'deep-orange'},
                {title: 'Vuejs', value: 70, color: 'deep-orange'},
                {title: 'Java', value: 60, color: 'black'},
            ],
            experience: [
                {
                    title: 'Full Stack Software Engineer',
                    date: 'December 20, 2021 – June 19, 2022',
                    institute: 'W3engineers Ltd',
                    decription: 'I have completed my internship under Sabbir Rahman and my internship was 6 months long. I have worked in cement framework which is python based.'
                },
                {
                    title: 'Mathematics Teacher',
                    date: 'January 2017 - Present',
                    institute: 'Radiant Coaching Centre',
                    decription: 'Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech Random speech'
                },
            ],
            sliders:[
                'https://hatrabbits.com/wp-content/uploads/2017/01/random.jpg',
                'https://images.unsplash.com/photo-1513542789411-b6a5d4f31634?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8cmFuZG9tfGVufDB8fDB8fA%3D%3D&w=1000&q=80',
                'https://cdn.pixabay.com/photo/2016/07/07/16/46/dice-1502706__340.jpg',
                'https://cdn.wallpapersafari.com/40/52/lHEsPO.jpg',
                'https://images.unsplash.com/photo-1493612276216-ee3925520721?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8aWRlYXxlbnwwfHwwfHw%3D&w=1000&q=80',
                'https://images.unsplash.com/photo-1567177662154-dfeb4c93b6ae?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8aW5ub3ZhdGlvbnxlbnwwfHwwfHw%3D&w=1000&q=80',
            ]
        }),
    }
</script>
<style>
    .v-tab.active-tab {
        color: #e91e63;
    }

    .v-tab.active-tab::before {
        background-color: #4caf50;
    }
</style>