<!DOCTYPE html>
<html>
<head>
    <title>Ceviche Clicker - Perú</title>
    <style>
        body { 
            font-family: 'Arial', sans-serif; 
            text-align: center; 
            background: linear-gradient(to right, #D91023, #FFFFFF, #D91023);
            padding: 20px;
        }
        #ceviche { 
            font-size: 120px; 
            cursor: pointer;
            transition: transform 0.1s;
        }
        #ceviche:active { transform: scale(0.95); }
        #contador { 
            font-size: 36px; 
            margin: 20px;
            color: #D91023;
            font-weight: bold;
        }
        .mejora { 
            background: #FFD700; 
            border: 3px solid #D91023;
            border-radius: 10px;
            padding: 10px;
            margin: 5px;
            cursor: pointer;
            font-weight: bold;
        }
        .donacion {
            background: #D91023;
            color: white;
            padding: 15px;
            border-radius: 10px;
            margin-top: 30px;
            display: inline-block;
        }
        .bandera {
            font-size: 30px;
            margin: 10px;
        }
    </style>
</head>
<body>
    <div class="bandera">🇵🇪</div>
    <h1>CEVICHE CLICKER</h1>
    <div id="ceviche" onclick="picarCeviche()">🐟🍋🌶️</div>
    <div id="contador">Soles: 0</div>
    
    <h2>MEJORAS PERUANAS</h2>
    <div id="mejoras"></div>
    
    <div class="donacion">
        <h3>¿Te gusta el juego?</h3>
        <p>¡Apoya con un cafecito peruano!</p>
        <p>Yape al: 999-888-777</p>
        <p><small>Donación voluntaria 🇵🇪</small></p>
    </div>

    <script>
        let soles = 0;
        let mejoras = [
            {nombre: "🍋 Limón arequipeño", costo: 50, produccion: 1, comprado: false},
            {nombre: "👵 Abuelita picando cebolla", costo: 100, produccion: 3, comprado: false},
            {nombre: "🏪 Puesto en Mercado #1", costo: 500, produccion: 10, comprado: false},
            {nombre: "🚐 Mototaxi delivery", costo: 2000, produccion: 50, comprado: false}
        ];
        let produccionTotal = 0;

        function picarCeviche() {
            soles++;
            actualizarContador();
            document.getElementById('ceviche').style.transform = 'scale(0.95)';
            setTimeout(() => {
                document.getElementById('ceviche').style.transform = 'scale(1)';
            }, 100);
        }

        function comprarMejora(index) {
            const mejora = mejoras[index];
            if(!mejora.comprado && soles >= mejora.costo) {
                soles -= mejora.costo;
                mejora.comprado = true;
                produccionTotal += mejora.produccion;
                actualizarContador();
                actualizarMejoras();
                alert(`¡Comprado! ${mejora.nombre} genera ${mejora.produccion} soles/seg`);
            }
        }

        function actualizarContador() {
            document.getElementById('contador').innerText = `Soles: ${soles} | +${produccionTotal}/seg`;
            localStorage.setItem('cevicheSave', JSON.stringify({soles, mejoras, produccionTotal}));
        }

        function actualizarMejoras() {
            const container = document.getElementById('mejoras');
            container.innerHTML = '';
            mejoras.forEach((mejora, index) => {
                const btn = document.createElement('button');
                btn.className = 'mejora';
                btn.innerHTML = `${mejora.nombre}<br>💰 ${mejora.costo} soles`;
                btn.disabled = mejora.comprado || soles < mejora.costo;
                btn.onclick = () => comprarMejora(index);
                container.appendChild(btn);
            });
        }

        // Producción automática
        setInterval(() => {
            soles += produccionTotal;
            actualizarContador();
        }, 1000);

        // Guardado automático
        setInterval(() => {
            if(soles > 0) {
                localStorage.setItem('cevicheSave', 
                    JSON.stringify({soles, mejoras, produccionTotal}));
            }
        }, 5000);

        // Cargar partida
        window.onload = function() {
            const save = JSON.parse(localStorage.getItem('cevicheSave'));
            if(save) {
                soles = save.soles;
                mejoras = save.mejoras;
                produccionTotal = save.produccionTotal;
                actualizarContador();
                actualizarMejoras();
            }
        }

        // Inicializar
        actualizarMejoras();
    </script>
</body>
</html>
