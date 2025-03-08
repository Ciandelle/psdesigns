---
title: Career history 
description: All about me in this page
layout: layouts/post.njk
eleventyNavigation:
  key: Career
  weight: 2
---

<div class="timeline">
	<div class="career-container left">
	  <div class="career-content">
		<h2 class="h2-career">Government Digital Service</h2>
		<p class="p-career-job">Interaction Designer for <a href="https://design-system.service.gov.uk/">GOV.UK Design System</a></p>
		<p class="p-career">March 2022 to present</p>
	  </div>
	</div>
	<div class="career-container right">
		<div class="career-content">
			<h2 class="h2-career">Gambling Commission</h2>
			<p class="p-career-job">Junior Service Designer</p>
			<p class="p-career">April 2020 to February 2022</p>
		</div>
	</div>
	<div class="career-container left">
		<div class="career-content">
		  <h2 class="h2-career">Gambling Commission</h2>
		  <p class="p-career-job">ICT Implementation Analyst Officer<br></p>
		  <p class="p-career">November 2017 to April 2020</p>
		</div>
	  </div>
	  <div class="career-container right">
		  <div class="career-content">
			  <h2 class="h2-career">OneAdvanced</h2>
			  <p class="p-career-job">Customer Support Consultant<br></p>
			  <p class="p-career">July 2016 to February 2017</p>
		  </div>
	  </div>
	  <div class="career-container left">
		<div class="career-content">
		  <h2 class="h2-career">JD Wetherspoon</h2>
		  <p class="p-career-job">Shift Manager<br></p>
		  <p class="p-career">August 2008 to July 2016</p>
		</div>
	  </div>
  </div>

<style>
  /* The actual timeline (the vertical ruler) */
  .timeline {
	position: relative;
	max-width: 1200px;
	margin: 0 auto;
  }
  
  /* The actual timeline (the vertical ruler) */
  .timeline::after {
	content: '';
	position: absolute;
	width: 6px;
	background-color: #3775D2;
	top: 0;
	bottom: 0;
	left: 50%;
	margin-left: 42px;
  }
  
  /* Container around content */
  .career-container {
	padding: 10px 40px;
	position: relative;
	background-color: inherit;
	width: 45%;
	padding-bottom: 20px;
  }
  
  /* The circles on the timeline */
  .career-container::after {
	content: '';
	position: absolute;
	width: 25px;
	height: 25px;
	right: -14px;
	background-color: #FFFFFF;
	border: 5px solid #3775D2;
	top: 15px;
	border-radius: 50%;
	z-index: 1;
  }
  
  /* Place the container to the left */
  .left {
	left: 0;
  }
  
  /* Place the container to the right */
  .right {
	left: 56.5%;
  }
  
  /* Add arrows to the left container (pointing right) */
  .left::before {
	content: " ";
	height: 0;
	position: absolute;
	top: 22px;
	width: 0;
	z-index: 1;
	right: 42px;
	border: medium solid white;
	border-width: 10px 0 10px 10px;
	border-color: transparent transparent transparent white;
  }
  
  /* Add arrows to the right container (pointing left) */
  .right::before {
	content: " ";
	height: 0;
	position: absolute;
	top: 22px;
	width: 0;
	z-index: 1;
	left: 50px;
	border: medium solid white;
	border-width: 10px 10px 10px 0;
	border-color: transparent white transparent transparent;
  }
  
  /* Fix the circle for containers on the right side */
  .right::after {
	left: -14px;
  }
  
  /* The actual content */
  .career-content {
	padding: 10px 50px;
	padding-left: 20px;
	background-color: white;
	position: relative;
	border-radius: 5px;
	border: solid 2px #3775D2;
  }

  .h2-career {
	color: #3775D2;
	text-align: left;
	font-size: 1.602rem;
	font-weight: 700;
  }

  .p-career {
	color: #0A090C;
	text-align: left;
  }
  
  .p-career-job {
	color: #0A090C;
	font-weight: 700;
	text-align: left;
  }

  /* Media queries - Responsive timeline on screens less than 600px wide */
  @media screen and (max-width: 600px) {
  /* Place the timelime to the left */
	.timeline::after {
	  left: 31px;
	}
  
  /* Full-width containers */
	.career-container {
	  width: 100%;
	  padding-left: 70px;
	  padding-right: 25px;
	}
  
  /* Make sure that all arrows are pointing leftwards */
	.career-container::before {
	  left: 60px;
	  border: medium solid white;
	  border-width: 10px 10px 10px 0;
	  border-color: transparent white transparent transparent;
	}
  
  /* Make sure all circles are at the same spot */
	.left::after, .right::after {
	  left: 10px;
	}
  
  /* Make all right containers behave like the left ones */
	.right {
	  left: 0%;
	}
  }
  </style>
