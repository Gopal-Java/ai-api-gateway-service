# ai-api-gateway-service
Java code to Integrate free AI API integration to execute the basic Integration

#https://ai.google.dev/gemini-api/docs/api-key#windows
#Sample Json Request 

{
    "safetySettings": [
        {
            "threshold": "BLOCK_ONLY_HIGH",
            "category": "HARM_CATEGORY_HATE_SPEECH"
        },
        {
            "threshold": "BLOCK_ONLY_HIGH",
            "category": "HARM_CATEGORY_DANGEROUS_CONTENT"
        },
        {
            "threshold": "BLOCK_ONLY_HIGH",
            "category": "HARM_CATEGORY_SEXUALLY_EXPLICIT"
        },
        {
            "threshold": "BLOCK_ONLY_HIGH",
            "category": "HARM_CATEGORY_HARASSMENT"
        }
    ],
    "contents": [
        {
            "role": "user",
            "parts": [
                {
                    "text": "share best team size to work "
                }
            ]
        }
    ],
    "generationConfig": {
        "temperature": 0.5,
        "topP": 0.99
    }
}