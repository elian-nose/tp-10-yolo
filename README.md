* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #151b2b;
    color: white;
    text-align: center;
}

header {
    background: #243451;
    padding: 25px;
}

header h1 {
    font-size: 35px;
    color: #55c8ff;
}

main {
    max-width: 800px;
    margin: 30px auto;
    padding: 15px;
}

section {
    background: #243451;
    padding: 25px;
    margin-bottom: 20px;
    border-radius: 15px;
}

h2 {
    margin-bottom: 20px;
}

.camera img {
    width: 100%;
    max-width: 500px;
    min-height: 200px;
    background: #080d17;
    border-radius: 10px;
    object-fit: contain;
}

.buttons {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 12px;
}

.middle {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    justify-content: center;
}

button {
    background: #168bd2;
    color: white;
    border: none;
    padding: 15px;
    border-radius: 10px;
    cursor: pointer;
    font-size: 15px;
}

button:hover {
    background: #0870ad;
}

#status, #cameraStatus {
    color: #55c8ff;
}

footer {
    padding: 20px;
    color: #aaa;
}
