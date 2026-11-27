const SERVER_URL = "http://192.168.1.100:5000";

async function move(direction) {

    const status = document.getElementById("status");

    status.textContent = "Enviando comando: " + direction;

    try {
        const response = await fetch(
            SERVER_URL + "/api/move",
            {
                method: "POST",

                headers: {
                    "Content-Type": "application/json"
                },

                body: JSON.stringify({
                    comando: direction
                })
            }
        );

        if (!response.ok) {
            throw new Error("Error del servidor");
        }

        status.textContent = "Comando enviado: " + direction;

    } catch (error) {
        status.textContent = "No se pudo conectar al servidor";
        console.error(error);
    }
}
