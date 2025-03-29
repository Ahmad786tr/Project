<?php 
global $post;
$post_id = get_the_ID();
get_header();
?>
    <div class="page-title-wrap">
        <div class="container">
            <div class="d-flex align-items-center">
                <?php get_template_part('template-parts/page/breadcrumb');?>
            </div>
        </div>
    </div>
            
    <section class="content-wrap property-wrap property-detail-v7">
        <?php
            get_template_part('campus-details/top-area-v7');=[]
            get_template_part('campus-details/campus-title'); 
        ?>
        <div class="container">
            <div class="row">
                <div class="col-lg-12 col-md-12 bt-content-wrap">                  
                    <div class="property-view">
                        <?php       
                            get_template_part('campus-details/mobile-view');                     
                            get_template_part( 'campus-details/single-campus', 'simple');
                            get_template_part( 'campus-details/campus-map');
                            get_template_part( 'campus-details/location-info');
                            get_template_part( 'campus-details/campus-access');                                    
                            get_template_part( 'campus-details/safety-security');                                    

                        ?>
                        
                    </div><!-- property-view -->
                </div><!-- bt-content-wrap -->
            </div><!-- row -->
        </div><!-- container -->
