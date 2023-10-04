# Soluciones

1. Interruptor OFF/ON:

        encendido = false
        color = "rojo"

        SI (interruptor pulsado) ENTONCES
          SI (encendido == false) ENTONCES
            encendido = true
            color = "verde"
          EN CASO CONTRARIO
            encendido = false
            color = "rojo"

2. Semáforo:

        estado = 1
        luzVerde = true
        luzAmbar = false
        luzRoja = false

        SI (semáforo cambia) ENTONCES
          SI (estado == 1) ENTONCES
            luzVerde = false
            luzAmbar = true
            estado = 2
          EN CASO CONTRARIO
          SI (estado == 2) ENTONCES
            luzAmbar = false
            luzRoja = true
            estado = 3
          EN CASO CONTRARIO
            luzRoja = false
            luzVerde = true
            estado = 1

3. Canción de los elefantes:

        contador = 1

        MIENTRAS (contador < 11)
          SI (contador == 1) ENTONCES
            "1 elefante se balanceaba sobre la tela de una araña y como veía que no se caía fue a llamar a otro elefante."
          EN CASO CONTRARIO
            contador + "elefantes se balanceaban sobre la tela de una araña y como veían que no se caían fueron a llamar a otro elefante."
          
          contador = contador + 1
        
        "Y al final se cayeron."