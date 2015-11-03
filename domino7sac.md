<html>
<title>domino rainbow</title>
<link href="http://getbootstrap.com/dist/css/bootstrap.min.css" rel="stylesheet">
<style>
.card{width:3.370in;height:2.125in;}
.item{width:1.5in;height:1.5in;border-radius:2.88mm;position:relative}
div.item p {font-size:1in;color:#fff;margin: 0;position: absolute;top: 50%;left: 50%;margin-right: -50%;transform: translate(-50%, -50%) }	
</style>
<body>
<script>
var rainbow = ["red","orange","yellow","green","blue","indigo","violet"];
var mica = ["102","202","235","348","322","137","134"];
var sac7 = ["f00","f60","ff0","0f0","00f","609","d0f"];
var cnt=0;
for (i=0;i<7;i++){
	for (j=0;j<7;j++){
		if (j>=i){
		//document.write(i+'-'+j);
		//document.write(sac7[i]+'-'+sac7[j]);
		document.write('<div class="col-md-2">');
		document.write('<div style="background:'+rainbow[i]+'" class="item"><p class="trang">'+i+'</p></div>');
		document.write('<div style="background:'+rainbow[j]+'" class="item"><p class="trang">'+j+'</p></div>');
		document.write('<hr>');
		document.write('</div>');
		cnt+=1;
		}
	}
}
document.write(cnt);
</script>
</body>
</html>