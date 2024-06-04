pipeline
{
    agent any
    
    environment
    {
        CIUDAD = "A Coruña"
        HABITANTES = 244850
    }
    
    stages
    {
        stage("Info ciudad")
        {
            steps
            {
                script
                {
                    climaActual = "21°C Precipitaciones: 0% Humedad: 69% Viento: 11 km/h"
                    println "Ciudad: ${env.CIUDAD}\nHabitantes: ${env.HABITANTES}\nClima: " + climaActual
                }
            }
        }
        
        stage("Ejecutar un bat")
        {
            steps
            {
                bat "ipconfig /flushdns"
            }
        }
        
        stage("Info usuario")
        {
            steps
            {
                script
                {
                    println "Usuario que ejecuta la tarea: ${env.USER_NAME}"
                }
            }
        }
    }
    
}
