# js_odevleri
document.body.style.backgroundColor = "grey";

var isim = prompt("Adınız nedir?");
function printHello(){
    document.getElementById("greeting").innerHTML =("Merhaba, " + isim+ "! Hoşgeldin!");  	
}
printHello(isim)

var d = new Date();
var gunler= ["Pazar","Pazartesi","Salı","Çarşamba","Perşembe","Cuma","Cumartesi"];
document.getElementById("day").innerHTML = gunler[d.getDay()];
function tarihSaat() {
    var date = new Date().toLocaleString('tr-TR');
    document.getElementById("zaman").innerHTML = date;
}
setInterval(tarihSaat, 1000); 
