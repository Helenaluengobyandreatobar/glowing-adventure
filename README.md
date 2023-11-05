# glowing-adventure
Eliza
{[:) helmeth 
(vigor :
TTX
//() HTML5 versionados allinguaje
 
import random

# Definir las variables del jugador y los enemigos
jugador = {
    "nombre": "Aya Brea",
    "salud": 100,
    "ataque": 20,
    "defensa": 10
}

enemigo = {
    "nombre": "Criatura",
    "salud": 50,
    "ataque": 15,
    "defensa": 5
}

# Función para simular un combate
def combate(jugador, enemigo):
    print(f"¡{jugador['nombre']} vs {enemigo['nombre']}!")
    while jugador['salud'] > 0 and enemigo['salud'] > 0:
        # Turno del jugador
        jugador_danio = max(0, jugador['ataque'] - enemigo['defensa'])
        enemigo['salud'] -= jugador_danio
        print(f"{jugador['nombre']} hace {jugador_danio} de daño a {enemigo['nombre']}")

        # Turno del enemigo
        enemigo_danio = max(0, enemigo['ataque'] - jugador['defensa'])
        jugador['salud'] -= enemigo_danio
        print(f"{enemigo['nombre']} hace {enemigo_danio} de daño a {jugador['nombre']}")

    # Mostrar el resultado del combate
    if jugador['salud'] <= 0:
        print("¡Has sido derrotado!")
    else:
        print("¡Has vencido al enemigo!")

# Iniciar el juego
print("Bienvenido a <link category="CULTURE">Parasite Eve 2</link>")
print("Prepárate para la batalla")
input("Presiona Enter para comenzar")

# Simular un combate
combate(jugador, enemigo)
{
          from rasa import runway


# Definir las acciones del chatbot
class Actions:
    def saludar(self, dispatcher, tracker, domain):
        dispatcher.utter_message("¡Hola! ¿En qué puedo ayudarte?")
        return []

    def despedir(self, dispatcher, tracker, domain):
        dispatcher.utter_message("Hasta luego, ¡que tengas un buen día!")
        return []

    def obtener_informacion(self, dispatcher, tracker, domain):
        # Lógica para obtener información y enviarla al usuario
        dispatcher.utter_message("Aquí tienes la información que solicitaste.")
        return []

# Configurar el chatbot y entrenar el modelo
def train_chatbot():
    run.train(
        domain="domain.yml",
        config="config.yml",
        training_files="data/",
        output="models/",
    )

# Iniciar el chatbot
def start_chatbot():
    run.run(
        model="models/",
        endpoints="endpoints.yml",
        action=Actions(),
    )

# Entrenar y ejecutar el chatbot
if __name__ == "__main__":
    train_chatbot()
    start_chatbot()
 

En Definición de patrones y respuestas
(defvar *patterns*
  '(("Hola" "Hola, ¿en qué puedo ayudarte?")
    ("Me siento triste" "Entiendo, ¿puedes contarme más sobre eso?")
    ("No sé qué hacer" "A veces es útil hablar sobre tus preocupaciones. ¿Qué te preocupa en particular?")))

;; Función para buscar coincidencias en el mensaje del usuario
(defun match-pattern (input)
  (loop for pattern in *patterns*
        do (loop for item in pattern
                 when (string-equal input item)
                 return (second pattern))))

;; Función principal para procesar la entrada del usuario y generar una respuesta
(defun eliza ()
  (format t "Eliza: ")
  (let ((input (read-line)))
    (let ((response (match-pattern input)))
      (if response
          (format t "~a~%" response)
          (format t "Lo siento, no entiendo. ¿Podrías ser más claro?~%"))))
          
;; Ejecutar el programa          
(eliza)

;; Definición de patrones y respuestas
(defvar *patterns*
  '(("Hola" "Hola, ¿en qué puedo ayudarte?")
    ("Me siento triste" "Entiendo, ¿puedes contarme más sobre eso?")
    ("No sé qué hacer" "A veces es útil hablar sobre tus preocupaciones. ¿Qué te preocupa en particular?")))

;; Función para buscar coincidencias en el mensaje del usuario
(defun match-pattern (input)
  (loop for pattern in *patterns*
        do (loop for item in pattern
                 when (string-equal input item)
                 return (second pattern))))

;; Función principal para procesar la entrada del usuario y generar una respuesta
(defun eliza ()
  (format t "Eliza: ")
  (let ((input (read-line)))
    (let ((response (match-pattern input)))
      (if response
          (format t "~a~%" response)
          (format t "Lo siento, no entiendo. ¿Podrías ser más claro?~%")))))

;; Ejecutar el programa          
(eliza)
Token
 (defvar *patterns* '(("Hola" "Hola, ¿en qué puedo ayudarte?") ("Me siento triste" "Entiendo, ¿puedes contarme más sobre eso?") ("No sé qué hacer" "A veces es útil hablar sobre tus preocupaciones. ¿Qué te preocupa en particular?"))) 
 (defun match-pattern (input) (loop for pattern in *patterns* do (loop for item in pattern when (string-equal input item) return (second pattern)))) 
 (defun eliza () (format t "Eliza: ") (let ((input (read-line))) (let ((response (match-pattern input))) (if response (format t "~a~%" response) (format t "Lo siento, no entiendo. ¿Podrías ser más claro?~%"))))) 
 (eliza) 
¡Hola!

Aquí tienes un ejemplo de código de Réplica para que puedas compararlo con Eliza:

 
 
import random

# Lista de respuestas de Réplica
respuestas_replica = [
    "Cuéntame más sobre eso.",
    "¿Cómo te hace sentir eso?",
    "¿Qué te llevó a pensar eso?",
    "¿Puedes profundizar en ese tema?",
    "Háblame más sobre tus emociones al respecto.",
]

# Función principal de Réplica
def replica():
    while True:
        entrada_usuario = input("Usuario: ")
        respuesta = random.choice(respuestas_replica)
        print("Réplica: " + respuesta)

# Ejecutar Réplica
replica()

Puedes personalizar las respuestas en la lista  respuestas_replica  para adaptarlas a tus necesidades.
Token Helena luengo 
