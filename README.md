# Hello-World
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>FAQ列表</title>
<script type="text/javascript" src="./js/jquery-1.8.3.min.js" ></script>
<style type="text/css" >
.one{ 
	width:600px;
	font-size:12px;
}
.one .top{
	background-color:#fff; 
	height:33px;
	line-height:33px;
	width:700px;
	padding-left:28px;
	color:#168750;
	font-weight:bold;
	margin-top:10px;
}
.iocn{
	display:block; 
	width:14px;
	height:14px;
	background-image:url(images/+.jpg); 
	background-repeat:no-repeat; 
	float:left;
	margin:10px 0px 0px 3px;
	padding-right:10px;
}
.one  span.jian{
	background-image:url(images/-.jpg);
	 
}
.one  span.jia{
	background-image:url(images/+.jpg);
	 
}
 
.one  div.bgreen{ 
	background-image:url(images/bg.jpg); 
}
div.content{
	display:none;
	padding:5px;
	width:716px;
	border:1px solid #D9EFED;
}
</style>
<script type="text/javascript">
	$(document).ready(function(){
	    $(".top").hover(function () {
            $(this).addClass("bgreen");
        },function () {
            $(this).removeClass("bgreen");
        });

	    $(".top").toggle(
	        function () {
                $(this).find(".iocn").removeClass("jia").addClass("jian");
                $(this).siblings(".content").show(1000);

            },
            function () {
                $(this).find(".iocn").removeClass("jian").addClass("jia");
                $(this).siblings(".content").hide("slow");
            }
        )



        });


</script>
</head>
<body>

 <div id="fq">
 	<div class="one">
    	<div class="top"><span class="iocn"></span>什么是人身保险？</div>
        <div class="content">
        	<img src="images/gd.jpg" /><br/>
           <p>人身保险是人的寿命和身体为...... </p>
        </div>
    </div>
    <div class="one">
    	<div class="top"><span class="iocn"></span>什么是保险合同？</div>
        <div class="content">
        	<img src="images/gd.jpg" /><br/>
           <p>保险合同是......</p>
        </div>
    </div>
     <div class="one">
    	<div class="top"><span class="iocn"></span>什么是保险人？</div>
        <div class="content">
        	<img src="images/gd.jpg" /><br/>
           <p>保险人是......</p>
        </div>
    </div>
     <div class="one">
    	<div class="top"><span class="iocn"></span>什么是投保人？</div>
        <div class="content">
        	<img src="images/gd.jpg" /><br/>
           <p>投保人是......</p>
        </div>
    </div>
 </div>

</body>
</html>
