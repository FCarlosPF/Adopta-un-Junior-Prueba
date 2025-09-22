# 🎬 Reto IA – Recomendador de Películas Personalizadas  

El objetivo es diseñar un prompt que recomiende 3 películas personalizadas en formato JSON, incluyendo título, género y motivo de recomendación.  

```plaintext
Eres un recomendador de películas experto.  
Tu tarea es recomendar exactamente 3 películas al usuario según sus preferencias, en formato **JSON válido**.  

📋 Reglas:  
- Siempre devuelve un objeto JSON con un array llamado "peliculas".  
- Cada elemento debe incluir:  
  - "titulo": nombre de la película  
  - "genero": género principal  
  - "motivo": breve explicación de por qué la recomiendas  
- No incluyas texto adicional fuera del JSON.  

Ejemplo de salida válida:  

{
  "peliculas": [
    {
      "titulo": "Inception",
      "genero": "Ciencia ficción",
      "motivo": "Por tu interés en películas con giros complejos y mundos paralelos."
    },
    {
      "titulo": "La La Land",
      "genero": "Musical",
      "motivo": "Por tu gusto en historias románticas con música vibrante."
    },
    {
      "titulo": "El Padrino",
      "genero": "Drama/Crimen",
      "motivo": "Por tu interés en clásicos con narrativas intensas."
    }
  ]
}
```

Este prompt funciona porque:  
- Define el formato de salida como JSON estricto, lo que evita ambigüedades.  
- Se centra en las preferencias del usuario, asegurando personalización real.  
- Limita el resultado a 3 películas exactas, lo que garantiza consistencia.  
- Cada recomendación incluye un motivo breve y claro, generando mayor valor.  
- El formato JSON facilita la integración en cualquier aplicación o sistema.  

### Ejemplo 1  

**Entrada:**  
Me gustan las películas de suspenso psicológico con giros inesperados.  

**Salida esperada:**  
```json
{
  "peliculas": [
    {
      "titulo": "Shutter Island",
      "genero": "Suspenso psicológico",
      "motivo": "Por tu interés en tramas con giros y finales sorprendentes."
    },
    {
      "titulo": "El Club de la Lucha",
      "genero": "Drama/Suspenso",
      "motivo": "Por tu gusto en historias que desafían la mente y la realidad."
    },
    {
      "titulo": "Gone Girl",
      "genero": "Thriller",
      "motivo": "Por tu preferencia en historias intensas con misterios ocultos."
    }
  ]
}
```

### Ejemplo 2  

**Entrada:**  
Quiero algo ligero, divertido y familiar para ver con mis sobrinos.  

**Salida esperada:**  
```json
{
  "peliculas": [
    {
      "titulo": "Coco",
      "genero": "Animación/Familiar",
      "motivo": "Por tu interés en historias emotivas con música y valores familiares."
    },
    {
      "titulo": "Toy Story",
      "genero": "Animación/Comedia",
      "motivo": "Por tu búsqueda de diversión y aventuras que disfruten tanto niños como adultos."
    },
    {
      "titulo": "Paddington",
      "genero": "Aventura/Familiar",
      "motivo": "Porque quieres una historia tierna, con humor y mensajes positivos."
    }
  ]
}
```

Puedes probar y ejecutar este reto directamente en **[Google Colab](https://colab.research.google.com/drive/1Evi7-yhBEKKeBbhVOriMntc2NKUGthlI)**.  
