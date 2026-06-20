# pagina-
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SISTEMA ELITE</title>

<style>
body{
  margin:0;
  background: radial-gradient(circle, #050505, #000000);
  color:#00ff88;
  font-family: monospace;
  display:flex;
  justify-content:center;
  align-items:center;
  height:100vh;
  overflow:hidden;
}

/* caja principal */
.card{
  border:1px solid #00ff88;
  padding:30px;
  text-align:center;
  box-shadow: 0 0 20px #00ff8850;
  animation: glow 2s infinite alternate;
}

/* glow suave */
@keyframes glow{
  from {box-shadow:0 0 10px #00ff8850;}
  to {box-shadow:0 0 25px #00ff88aa;}
}

/* glitch texto */
.glitch{
  font-size:28px;
  position:relative;
  animation: flicker 1.5s infinite;
}

@keyframes flicker{
  0%,100%{opacity:1;}
  50%{opacity:0.4;}
}

/* animación typing */
.typing{
  overflow:hidden;
  white-space:nowrap;
  border-right:2px solid #00ff88;
  width:0;
  animation: typing 3.5s steps(40,end) forwards;
}

@keyframes typing{
  from{width:0;}
  to{width:100%;}
}

/* scan line */
.scan{
  position:absolute;
  width:100%;
  height:2px;
  background:#00ff88;
  opacity:0.2;
  animation: scan 3s linear infinite;
}

@keyframes scan{
  0%{top:0;}
  100%{top:100%;}
}

button{
  margin-top:15px;
  background:black;
  border:1px solid #00ff88;
  color:#00ff88;
  padding:10px 15px;
  cursor:pointer;
}

button:hover{
  background:#00ff88;
  color:black;
}
</style>
</head>

<body>

<div class="scan"></div>

<div class="card">

  <div class="glitch">Δ SISTEMA ELITE</div>

  <p class="typing">Verificando acceso... sistema en línea</p>

  <p>Estado: CONECTADO</p>
  <p>Cifrado: ACTIVO</p>
  <p>ID: X-07-NULL</p>

  <button onclick="alert('SEÑAL ACTIVA')">ACTIVAR PROTOCOLO</button>

</div>

</body>
</html>