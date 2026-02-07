var respuesta = "si";
while (respuesta == "si") {
    var compu = Math.floor(Math.random() * 9) + 1;
    var usuario = parseInt(prompt("Ingrese un numero del 1 al 9:"))
    while (usuario < 1 || usuario > 9) {
        usuario = parseInt(prompt("eror. Ingrese un numero del 1 al 9:"));
    }
    var prediccion = prompt("Tu numero es mayor, menor o igual?").toLowerCase();
    if (prediccion == "mayor" && usuario > compu) {
        alert("ganastes la compu tenia" + compu + "y tu numero era" + usuario);
    }
    else if (prediccion == "menor" && usuario < compu) {
        alert("ganastes la compu tenia" + compu + " y tu tenias" + usuario)
    }
    else if (prediccion == "igual" && usuario == compu) {
        alert(" ganastes la compu tenia" + compu + " y tu tenias" + usuario)
    }
    else {
        alert("perdiste la compu tenia" + compu + " y tu tenias" + usuario)
    }
    respuesta = prompt("Quieres jugar de nuevo? (si/no) ").toLowerCase();
}
alert("Nombre: Jose Angel Ramirez Rodriguez\nCarnet: 26000155\nCarrera:Ingenieria en Sistemas\nFecha: 2/02/2026") 