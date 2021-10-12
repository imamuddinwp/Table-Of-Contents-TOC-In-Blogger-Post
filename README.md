# Table-Of-Contents-TOC-In-Blogger-Post
Original post is here: https://imamuddinwp.blogspot.com/2021/10/how-to-add-a-table-of-contents-toc-in-blogger-post.html
Video Tutorial For Add A Clickable Table Of Contents Toc To Blogger Post: https://www.youtube.com/watch?v=NTq_ApiEbJ8
<hr/>
<img src="https://github.com/imamuddinwp/Table-Of-Contents-TOC-In-Blogger-Post/blob/main/table-of-contents-toc-in-blogger-post-imamuddinwp-.png" alt="table-of-contents-toc-in-blogger-post-imamuddinwp" />
<br/>
Steps to create TOC In Blogger:
Go to your blogger dash board by login to blogger
Go to 'Edit HTML' from 'Theme' option
edit-html-blogger-template-blogger-theme-imamuddinwp
Then search </head>
After that Copy the following code and paste above </head>
<!-- Table of contents Javascript start-->

 <script type='text/javascript'>              
//<![CDATA[           
//*************TOC plugin by MyBloggerTricks.com           
function mbtTOC() {var mbtTOC=i=headlength=gethead=0;           
headlength = document.getElementById("post-toc").getElementsByTagName("h2").length;for (i = 0; i < headlength; i++)           
{gethead = document.getElementById("post-toc").getElementsByTagName("h2")[i].textContent;document.getElementById("post-toc").getElementsByTagName("h2")[i].setAttribute("id", "point"+i);mbtTOC = "<li><a href='#point"+i+"'>"+gethead+"</a></li>";document.getElementById("mbtTOC").innerHTML += mbtTOC;}}function mbtToggle() {var mbt = document.getElementById('mbtTOC');if (mbt .style.display === 'none') {mbt .style.display = 'block';} else {mbt .style.display = 'none';}}           
//]]>              
</script>
<!-- Table of contents Javascript end -->
After that search (by typing 'Ctrl+F' in keyboard) ]]></b:skin>
And copy the following code and paste above ]]></b:skin>
.mbtTOC{border:5px dashed dodgerblue;box-shadow:2px 0px 10px 4px silver;background-color:#f2f2f2;color:black;line-height:1.4em;margin:30px auto;padding:20px 30px 20px 10px; font-family:oswald, arial;display: block;width: 70%;}           
.mbtTOC ol,.mbtTOC ul {margin:0;padding:0;}           
.mbtTOC ul {list-style:none;}           
.mbtTOC ol li,.mbtTOC ul li {padding:15px 0 0; margin:0 0 0 30px;font-size:15px;}           
.mbtTOC a{color:#0080ff;text-decoration:none;}           
.mbtTOC a:hover{text-decoration:underline; }
.mbtTOC button{background:#f2f2f2; font-family:oswald, arial; font-size:20px;position:relative; outline:none;cursor:pointer; border:none; color:black;padding:0 0 0 15px;} 
.mbtTOC button:after{font-family:FontAwesome; position:relative; left:10px; font-size:20px;}

Here I have attached an image for better understanding of TOC in blogger theme!

table-of-contents-toc-in-blogger-theme-imamuddinwp
After That search for  <data:post.body/>
Note:- You might found more than one code, simply replace the codes with following codes:

<div id="post-toc"><data:post.body/></div>
After doing all the steps, just save the theme.
Go to Blogger Dash board.
Choose your desired post to apply TOC.
Open HTML View
Choose the right place to show TOC.
Copy the Code and paste those place.
<div class="mbtTOC"> 
    <button onclick="mbtToggle()">Table Of Contents ✓</button> 
    <ul id="mbtTOC"></ul> 
    </div>
After that, go to bottom of the post by scroll down.
Be sure the post is in HTML view
Copy the java scripts
Paste the code under the post where post will end.
<script>mbtTOC();</script>
See below image for better understanding of HTML view from my blog post:

blogger-theme-post-html-view-imamuddinwp
Also please see it:

table-of-contents-toc-in-blogger-post-imamuddinwp
After completing all these steps, just save your post. You Are All Done ! Now you can see the Table of Contents -TOC in Your Blog post. Here I have attached a screen shoot of TOC from this post.
