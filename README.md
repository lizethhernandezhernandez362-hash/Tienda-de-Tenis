<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>TIENDA DE TENIS ADIDAS y más</title>
    <script>
        let total = 0;
        function agregarCarrito(precio) {
            total = total + precio;
            document.getElementById("total").innerText = total.toFixed(2);
            alert("✅ ¡Agregado al carrito!");
        }

        function mostrarSeccion(idSeccion) {
            // Oculta todas las secciones principales
            document.getElementById('inicio-bienvenida').style.display = 'none';
            document.getElementById('pantalla-siguiente').style.display = 'none';
            document.getElementById('tienda-principal').style.display = 'none';
            
            // Muestra la sección solicitada
            document.getElementById(idSeccion).style.display = 'block';
        }
    </script>
</head>
<body style="background-color: #154360; color: white; font-family: sans-serif; margin: 0; padding: 0;">

    <div id="inicio-bienvenida" style="background-image: url('mar.jpg'); background-size: cover; background-repeat: no-repeat; min-height: 100vh; text-align: center; padding-top: 100px;">
        <h1 style="font-size: 60px; color: red; font-weight: bold; margin-bottom: 50px;">TENIS ADIDAS</h1>
        
        <button onclick="mostrarSeccion('pantalla-siguiente')" style="font-size: 24px; padding: 15px 40px; background-color: white; color: green; border: 2px solid white; font-weight: bold; cursor: pointer;">
            VER CATÁLOGO
        </button>
    </div>

    <div id="pantalla-siguiente" style="display: none; background-image: url('te.jpg'); background-size: cover; background-repeat: no-repeat; min-height: 100vh; text-align: center; padding-top: 100px;">
        
        <button onclick="mostrarSeccion('tienda-principal')" style="font-size: 24px; padding: 15px 48px; background-color: white; color: lime; border: 2px solid white; font-weight: bold; cursor: pointer;">
            SIGUIENTE
        </button>
    </div>

    <div id="tienda-principal" style="display: none; text-align: center; padding: 40px 20px;">
        
        <p style="font-size: 20px; font-style: italic;">"Paso a paso, siempre con estilo y comodidad"</p>
        <p style="font-size: 24px; font-weight: bold;">Las mejores marcas y los mejores precios</p>
        
        <button onclick="document.getElementById('contenido-catalogo').style.display='block'" 
                style="background: yellow; color: black; padding: 15px 30px; font-size: 22px; border: 3px solid black; border-radius: 10px; cursor: pointer; font-weight: bold; margin-bottom: 30px;">
            🚀 MOSTRAR PRODUCTOS
        </button>

        <div id="contenido-catalogo" style="display: none;">

            <div style="background: rgba(0,0,0,0.4); margin: 20px auto; padding: 15px; width: 90%; border-radius: 10px; border: 3px solid white;">
                <h2 style="color: yellow;">HOMBRES</h2>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="nike.jpg" width="140" alt="Nike Air Max"><br>
                    <b>Nike Air Max</b><br>
                    <span style="color: yellow;">Tallas: 25 al 29</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$2,499</b></span><br>
                    <button onclick="agregarCarrito(2499)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="ultra.jpg" width="140" alt="Adidas Ultraboost"><br>
                    <b>Adidas Ultraboost</b><br>
                    <span style="color: yellow;">Tallas: 25 al 30</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$2,299</b></span><br>
                    <button onclick="agregarCarrito(2299)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="puma.jpg" width="140" alt="Puma RS-X"><br>
                    <b>Puma RS-X</b><br>
                    <span style="color: yellow;">Tallas: 24.5 al 28</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,850</b></span><br>
                    <button onclick="agregarCarrito(1850)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="clas.jpg" width="140" alt="Reebok Classic"><br>
                    <b>Reebok Classic</b><br>
                    <span style="color: yellow;">Tallas: 24 al 28</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,450</b></span><br>
                    <button onclick="agregarCarrito(1450)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="new.jpg" width="140" alt="New Balance"><br>
                    <b>New Balance</b><br>
                    <span style="color: yellow;">Tallas: 25 al 29</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,890</b></span><br>
                    <button onclick="agregarCarrito(1890)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="jor.jpg" width="140" alt="Jordan Retro"><br>
                    <b>Jordan Retro</b><br>
                    <span style="color: yellow;">Tallas: 25 al 29</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$2,600</b></span><br>
                    <button onclick="agregarCarrito(2600)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>
            </div>

            <div style="background: rgba(0,0,0,0.4); margin: 20px auto; padding: 15px; width: 90%; border-radius: 10px; border: 3px solid white;">
                <h2 style="color: pink;">MUJERES</h2>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="oze.jpg" width="140"><br>
                    <b>Adidas Ozelia</b><br>
                    <span style="color: yellow;">Tallas: 22 al 25</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,999</b></span><br>
                    <button onclick="agregarCarrito(1999)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="th.jpg" width="140"><br>
                    <b>Nike Waffle</b><br>
                    <span style="color: yellow;">Tallas: 22.5 al 24.5</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,750</b></span><br>
                    <button onclick="agregarCarrito(1750)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="vik.jpg" width="140"><br>
                    <b>Puma Vikky</b><br>
                    <span style="color: yellow;">Tallas: 22 al 25</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,550</b></span><br>
                    <button onclick="agregarCarrito(1550)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="con.jpg" width="140"><br>
                    <b>Converse Plataforma</b><br>
                    <span style="color: yellow;">Tallas: 22 al 25</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,300</b></span><br>
                    <button onclick="agregarCarrito(1300)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="ree.jpg" width="140"><br>
                    <b>Vans Old Skool</b><br>
                    <span style="color: yellow;">Tallas: 22 al 25</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,250</b></span><br>
                    <button onclick="agregarCarrito(1250)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="ros.jpg" width="140"><br>
                    <b>New Balance Rosa</b><br>
                    <span style="color: yellow;">Tallas: 22 al 25</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,600</b></span><br>
                    <button onclick="agregarCarrito(1600)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 180px; vertical-align: top;">
                    <img src="mor.jpg" width="140"><br>
                    <b>New Balance Morado</b><br>
                    <span style="color: yellow;">Tallas: 22 al 27</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$1,700</b></span><br>
                    <button onclick="agregarCarrito(1700)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>
            </div>

            <div style="background: rgba(0,0,0,0.4); margin: 20px auto; padding: 15px; width: 90%; border-radius: 10px; border: 3px solid white;">
                <h2 style="color: cyan;">NIÑOS</h2>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="ten.jpg" width="120"><br>
                    <b>Adidas Tensaur</b><br>
                    <span style="color: yellow;">Tallas: 18 al 22</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$999</b></span><br>
                    <button onclick="agregarCarrito(999)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="runner.jpg" width="120"><br>
                    <b>Nike Star Runner</b><br>
                    <span style="color: yellow;">Tallas: 17 al 21</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$950</b></span><br>
                    <button onclick="agregarCarrito(950)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="pum.jpg" width="120"><br>
                    <b>Puma Stepfleex</b><br>
                    <span style="color: yellow;">Tallas: 18 al 21</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$890</b></span><br>
                    <button onclick="agregarCarrito(890)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="verde.jpg" width="120"><br>
                    <b>Reebok Niño</b><br>
                    <span style="color: yellow;">Tallas: 16 al 19</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$800</b></span><br>
                    <button onclick="agregarCarrito(800)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="dc.jpg" width="120"><br>
                    <b>DC Shoes</b><br>
                    <span style="color: yellow;">Tallas: 19 al 22</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$850</b></span><br>
                    <button onclick="agregarCarrito(850)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="um.jpg" width="120"><br>
                    <b>Umbro Niño</b><br>
                    <span style="color: yellow;">Tallas: 18 al 21</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$700</b></span><br>
                    <button onclick="agregarCarrito(700)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>
            </div>

            <div style="background: rgba(0,0,0,0.4); margin: 20px auto; padding: 15px; width: 90%; border-radius: 10px; border: 3px solid white;">
                <h2 style="color: magenta;">NIÑAS</h2>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="cour.jpg" width="120"><br>
                    <b>Adidas Grand Court</b><br>
                    <span style="color: yellow;">Tallas: 18 al 22</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$980</b></span><br>
                    <button onclick="agregarCarrito(980)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="flex.jpg" width="120"><br>
                    <b>Nike Flex</b><br>
                    <span style="color: yellow;">Tallas: 17 al 20</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$960</b></span><br>
                    <button onclick="agregarCarrito(960)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="car.jpg" width="120"><br>
                    <b>Puma Caracal</b><br>
                    <span style="color: yellow;">Tallas: 18 al 21</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$900</b></span><br>
                    <button onclick="agregarCarrito(900)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="reb.jpg" width="120"><br>
                    <b>Reebok Rosa</b><br>
                    <span style="color: yellow;">Tallas: 16 al 19</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$820</b></span><br>
                    <button onclick="agregarCarrito(820)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="sk.jpg" width="120"><br>
                    <b>Skechers Niña</b><br>
                    <span style="color: yellow;">Tallas: 18 al 21</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$950</b></span><br>
                    <button onclick="agregarCarrito(950)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>

                <div style="display: inline-block; background: rgba(255,255,255,0.1); margin: 10px; padding: 10px; border-radius: 8px; width: 160px; vertical-align: top;">
                    <img src="fila.jpg" width="120"><br>
                    <b>Fila Disruptor</b><br>
                    <span style="color: yellow;">Tallas: 19 al 22</span><br>
                    <span style="color: lime; font-size: 18px;"><b>$880</b></span><br>
                    <button onclick="agregarCarrito(880)" style="background: orange; color: black; border: none; padding: 5px 10px; margin-top: 8px; border-radius: 5px; cursor: pointer;">🛒 AGREGAR</button>
                </div>
            </div>

            <br><br>
            
            <div style="border: 3px solid yellow; background: black; padding: 10px; width: 300px; margin: auto; border-radius: 10px;">
                <h2>🛒 CARRITO</h2>
                <h3>Total: $<span id="total">0.00</span> MXN</h3>
            </div>

            <br><br>

            <div style="background: rgba(0,0,0,0.6); margin: 30px auto; padding: 20px; width: 80%; max-width: 500px; border: 2px solid yellow; border-radius: 10px;">
                <h2><font color="yellow">💳 PAGO CON TARJETA</font></h2>
                <p><input type="text" placeholder="Número de tarjeta" style="padding: 8px; width: 80%; max-width: 250px;"></p>
                <p>
                    <input type="text" placeholder="MM/AA" style="padding: 8px; width: 80px;"> 
                    <input type="text" placeholder="CVV" style="padding: 8px; width: 80px;">
                </p>
                <p><input type="text" placeholder="Nombre completo" style="padding: 8px; width: 80%; max-width: 250px;"></p>
                <button onclick="alert('¡Compra realizada con éxito! ✅')" style="background: lime; color: black; border: none; padding: 10px 20px; font-size: 18px; font-weight: bold; border-radius: 5px; cursor: pointer; margin-top: 10px;">
                    PAGAR AHORA
                </button>
            </div>

        </div>
    </div>

</body>
</html>
