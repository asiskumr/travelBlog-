# travelBlog-
Travel Blog website using nodejs
<%- include("partials/header"); -%>


<link rel="canonical" href="https://getbootstrap.com/docs/4.5/examples/carousel/">

<!-- Bootstrap core CSS -->
<link href="/docs/4.5/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
  

        <div class="container">
            <div class="row" style="margin-top: 40px;">
                <div class="col-lg-11">
                    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel"
                         style="margin-top: 15px; margin-bottom: 20px;">
                         <ol class="carousel-indicators">
                            <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
                            <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
                            <li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
                            <li data-target="#carouselExampleCaptions" data-slide-to="3"></li>
                          </ol>
                         
                        <!-- <div  class="carousel-inner">
                            <% posts.forEach(function(post){ %> 
                                <div style="background-color: blue; height: 100px;" class="carousel-item active">   
                                                                
                                    <a href="/blog" >                                    
                                           <img style="height: 450px; background-size: cover;" src="data:image/<%=post.image.contentType%>;base64, 
                                            <%=post.image.data.toString('base64')%>" class="d-block w-100" alt="">
                                        <div class="carousel-caption ">
                                            <h4 class="mainstoryheader"><%= post.title %></h4>
                                        </div>
                                       
                                    </a>   
                                   
                                </div>
                                <% }) %> 
                        </div> -->
                      

                        <div class="carousel-inner">
                            <% for (var i = 0; i < posts.length; i++) { %>
                                <div  class="carousel-item <%= i == 0 ? 'active' : '' %>">
                                    <a href="/blog">
                                        <img style="height: 450px; background-size: cover;" src="data:image/<%=posts[i].image.contentType%>;base64, 
                                        <%=posts[i].image.data.toString('base64')%>" class="d-block w-100" alt="">
                                            <div class="carousel-caption " >
                                                <h2 class="mainstoryheader"><%= posts[i].title %></h2>

                                            </div>
                                        
                                    </a>
                                </div>
                            <% } %>
                        </div>


                               
                        <!-- <div class="carousel-item">
                                <a href="/blog"  style=" text-decoration: none;">
                                    <div style="background-image: url(https://lakshmisharath.com/wp-content/uploads/2013/10/bosphorus2-630x500.jpg);height: 450px; background-size: cover;">
                                        <h4 class="mainstoryheader">Five reasons to visit Istanbul</h4>
                                    </div>
                                </a>
                            </div> -->
                            <!-- <div class="carousel-item">
                                <a href="/blog" style=" text-decoration: none;">
                                    <div style="background-image: url(https://www.travelseewrite.com/wp-content/uploads/2020/07/Atali-Ganga-near-Rishikesh-Uttarakhand.jpg);height: 450px; background-size: cover;">
                                        <h4 class="mainstoryheader" style="color: #fff; text-decoration: none;">Life After Lockdown: Safest Places To Visit In India P COVID19</h4>
                                    </div>
                                </a>
                            </div> --> 
                          
                        </div>
                        
                        <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="sr-only">Previous</span>
                          </a>
                          <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="sr-only">Next</span>
                          </a>
                    
                    </div>
                </div>
    
            </div>
        </div>

        <div class="container">

        </div>

        <div class="container"style="margin-top: 40px; position: relative; left: 55px;">
            <div class="row">
            <h5 style="position: relative; right: 42px;">Must Read</h5>
            <div class="col-md-3 col-sm-6 editorspickdiv" style="padding-left: 0; position: relative; right: 135px;">
                <h5></h5><br>
                <hr style="background-color: #6b98ad; width: 0; height: 2px; margin: 0;">
                <a href="">
                    <div style="background-image: url(https://images.indianexpress.com/2018/05/kumbh-mela.jpg);height: 220px; background-size: cover; border-radius: 45px; margin-top: 15px;">                      
                    </div>
                </a>
                <a href="" style=" text-decoration: none;">  
                    <h5 class="editorspickheader" style="color: rgb(41, 20, 231);">Prayag Kumbh Mela,Allahabad (Prayagraj), Uttar Pradesh </h5>                 
                </a>
                <p></p> The Prayag Kumbh Mela is a Hindu festival mela held at Prayag Triveni Sangam – the meeting points of three rivers: the Ganga, the Yamuna and the mythical Sarasvati – in Allahabad (officially known as Prayagraj), India.[1] The festival is marked by a ritual dip in the waters, but it <a href="/file">Read More</a></p>
            </div>
            <div class="col-md-3 col-sm-6 editorspickdiv" style="padding-left: 0; position: relative; right: 45px;">
                <h5></h5><br>
                <hr style="background-color: #F5F5F5; width: 0; height: 2px; margin: 0;">
                <a href="" style=" text-decoration: none;">
                    <div style="background-image: url(https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Narendra_Modi_visiting_the_Museum%2C_Exhibition_and_the_Viewers%E2%80%99_Gallery%2C_during_the_dedication_of_the_%E2%80%98Statue_of_Unity%E2%80%99_to_the_Nation%2C_on_the_occasion_of_the_Rashtriya_Ekta_Diwas%2C_at_Kevadiya%2C_in_Narmada_District_of_Gujarat_%283%29.JPG/800px-thumbnail.jpg);height: 220px; background-size: cover;border-radius: 45px; margin-top: 15px;">
                    </div>
                </a>  
                <a href="" style=" text-decoration:none;">     
                    <h5 class="editorspickheader" style="color: rgb(57, 21, 218);"> Welcome , The structure of the Statue of Unity , INDIA</h5>              
                </a>
                <p>The Statue of Unity is located right in the middle of the Narmada river flanked by<a href="/main">Read More</a></p>
            </div>
            <div class="col-md-3 col-sm-6 editorspickdiv" style="padding-left: 0;">
                <h5></h5><br>
                <hr style="background-color: #F5F5F5; width: 0; height: 2px; margin: 0;">
                <a href="" style=" text-decoration: none;">
                    <div style="background-image: url(https://blog.railyatri.in/wp-content/uploads/2019/01/Tips-for-Sundarban-trip.png);height: 220px; background-size: cover;border-radius: 45px; margin-top: 15px;">
                    </div>
                </a>
                <a href="" style=" text-decoration: none;">
                    <h5 class="editorspickheader" style="color: rgb(58, 21, 223);">All need to know for a perfect Sundarban tour!</h5>                   
                    </a>
                  <p>Situated 109 KM away from the busy metropolitan of Kolkata, Sundarbans national park is a must visit during the winters! Sundarban is the largest mangrove forest in the world and has been declared as an <a href="/list">Read More</a></p>
           
           
            
           
                    </div>


            </div>          
        </div>
        <br>


     
        <div class="container" style="padding-top: 20px;">
            <% posts.forEach(function(post){ %>
         
                <a href="/blog"><img style="height: 200px; width: 30%; margin: 0;" src="data:image/<%=post.image.contentType%>;base64, 
                   <%=post.image.data.toString('base64')%>"></a>
                
                   <% }) %>
         <!-- <a href="/blog"><img style="height: 200px; width: 30%; margin: 0;" src="https://scontent.cdnsnapwidget.com/vp/eadd06c41f774b8c012d00f0cef3f467/5E2B31DB/t51.2885-15/sh0.08/e35/s640x640/67595955_149252299497434_230715276025021704_n.jpg" alt=""></a>
         <a href="/blog"><img style="height: 200px; width: 30%; margin: 0;" src="https://scontent.cdnsnapwidget.com/vp/eff1dc9d4cafcda54e0f343bbfb35a97/5E1877F6/t51.2885-15/sh0.08/e35/s640x640/67128487_2262173010761304_721508016892663838_n.jpg" alt=""></a>
         <a href="/blog"><img style="height: 200px; width: 30%; margin: 0;" src="https://scontent.cdnsnapwidget.com/vp/d7ab29e8686319c555fbb1aa51579e9a/5E1BF765/t51.2885-15/sh0.08/e35/s640x640/66655802_1082655445278523_2957868173309326177_n.jpg" alt=""></a>
         <a href="/blog"><img style="height: 200px; width: 30%; margin: 0;" src="https://scontent.cdnsnapwidget.com/vp/a8e21509df7793733fe86c7b7babfd12/5E19C5BB/t51.2885-15/sh0.08/e35/s640x640/66824284_699025243843740_2043035200160934521_n.jpg" alt=""></a>
         <a href="/blog"><img style="height: 200px; width: 30%; margin: 0;" src="https://scontent.cdnsnapwidget.com/vp/3c1f409cbb7d2fa43489ac95a59143ca/5E366832/t51.2885-15/sh0.08/e35/s640x640/67805462_164698841351895_6790893418934881034_n.jpg" alt=""></a> -->
        

        
        </div>

        


        <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
        <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
        <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>

<%- include("partials/footer"); -%>
