<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Grupo Albert’s CRM PRO</title>

<style>
body{font-family:Arial;margin:0;background:#0f172a;color:white}
header{background:#020617;padding:10px;text-align:center;font-weight:bold}
.container{padding:10px}
input,button,select,textarea{
width:100%;margin:5px 0;padding:10px;border-radius:8px;border:none
}
button{background:#2563eb;color:white;font-weight:bold}
.card{background:#1e293b;padding:10px;margin:10px 0;border-radius:10px}
.hidden{display:none}
.result{background:#334155;padding:8px;margin:5px 0;border-radius:6px}
</style>
</head>

<body>

<header>Grupo Albert’s CRM PRO</header>

<div class="container">

<!-- LOGIN -->
<div id="login">
<h3>Login</h3>
<input id="email" placeholder="Correo">
<input id="pass" type="password" placeholder="Contraseña">
<button onclick="login()">Entrar</button>
</div>

<!-- APP -->
<div id="app" class="hidden">

<h3>Dashboard</h3>
<input id="buscarDash" placeholder="Buscar cliente..." onkeyup="buscarClienteDash()">
<div id="dashResultados"></div>

<div id="menu">
<button onclick="mostrar('altaCliente')">Alta Cliente</button>
<button onclick="mostrar('buscarCliente')">Buscar Cliente</button>
<button onclick="mostrar('venta')">Nueva Venta</button>
<button onclick="mostrar('historia')">Historia Clínica</button>
<button onclick="mostrar('nota')">Nota</button>
<button onclick="logout()">Salir</button>
</div>

<!-- ALTA -->
<div id="altaCliente" class="hidden card">
<h4>Alta Cliente</h4>
<input id="c_nombre" placeholder="Nombre">
<input id="c_tel" placeholder="Teléfono">
<button onclick="guardarCliente()">Guardar</button>
</div>

<!-- BUSCAR -->
<div id="buscarCliente" class="hidden card">
<h4>Buscar Cliente</h4>
<input id="buscarInput" onkeyup="buscarCliente()" placeholder="Nombre">
<div id="resultados"></div>
</div>

<!-- VENTA -->
<div id="venta" class="hidden card">
<h4>Nueva Venta</h4>
<input id="v_cliente" placeholder="Cliente">
<input id="v_producto" placeholder="Producto">
<input id="v_costo" type="number" placeholder="Costo" oninput="calcular()">
<input id="v_descuento" type="number" placeholder="Descuento" oninput="calcular()">
<input id="v_total" placeholder="Total" readonly>
<input id="v_anticipo" type="number" placeholder="Anticipo" oninput="calcular()">
<input id="v_saldo" placeholder="Saldo" readonly>
<select id="v_tipo">
<option>Contado</option>
<option>Crédito</option>
</select>
<button onclick="guardarVenta()">Guardar</button>
</div>

<!-- HISTORIA -->
<div id="historia" class="hidden card">
<h4>Historia Clínica</h4>
<input id="h_cliente" placeholder="Cliente">
<textarea id="h_diag" placeholder="Diagnóstico"></textarea>
<button onclick="guardarHistoria()">Guardar</button>
</div>

<!-- NOTA -->
<div id="nota" class="hidden card">
<h4>Nota</h4>
<input id="n_cliente" placeholder="Cliente">
<button onclick="generarNota()">Generar</button>
<div id="notaVista"></div>
</div>

</div>
</div>

<script>

let clientes = JSON.parse(localStorage.getItem("clientes")) || [];
let ventas = JSON.parse(localStorage.getItem("ventas")) || [];

function login(){
if(email.value==="admin" && pass.value==="1234"){
login.style.display="none";
app.style.display="block";
}
}

function logout(){location.reload();}

function mostrar(id){
document.querySelectorAll(".card").forEach(x=>x.classList.add("hidden"));
document.getElementById(id).classList.remove("hidden");
}

function guardarCliente(){
if(!c_nombre.value){alert("Nombre requerido");return;}
clientes.push({nombre:c_nombre.value,tel:c_tel.value});
localStorage.setItem("clientes",JSON.stringify(clientes));
alert("Cliente guardado");
}

function buscarCliente(){
let txt=buscarInput.value.toLowerCase();
resultados.innerHTML=clientes
.filter(c=>c.nombre.toLowerCase().includes(txt))
.map(c=>`<div class="result">${c.nombre} - ${c.tel}</div>`)
.join("");
}

function buscarClienteDash(){
let txt=buscarDash.value.toLowerCase();
dashResultados.innerHTML=clientes
.filter(c=>c.nombre.toLowerCase().includes(txt))
.map(c=>`<div class="result">${c.nombre}</div>`)
.join("");
}

function calcular(){
let costo=parseFloat(v_costo.value)||0;
let desc=parseFloat(v_descuento.value)||0;
let anticipo=parseFloat(v_anticipo.value)||0;

let total=costo-desc;
let saldo=total-anticipo;

v_total.value=total;
v_saldo.value=saldo;
}

function guardarVenta(){
if(!v_cliente.value){alert("Cliente requerido");return;}

ventas.push({
cliente:v_cliente.value,
producto:v_producto.value,
total:v_total.value,
saldo:v_saldo.value
});

localStorage.setItem("ventas",JSON.stringify(ventas));
alert("Venta guardada");
}

function guardarHistoria(){
alert("Historia guardada");
}

function generarNota(){
let v=ventas.find(x=>x.cliente===n_cliente.value);
if(!v){notaVista.innerHTML="Sin venta";return;}

notaVista.innerHTML=`
<div class="card">
Cliente: ${v.cliente}<br>
Producto: ${v.producto}<br>
Total: $${v.total}<br>
Saldo: $${v.saldo}
</div>`;
}

</script>

</body>
</html>