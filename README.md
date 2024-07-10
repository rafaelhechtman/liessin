<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Site de Urários Escolares</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 20px;
        }
        h1 {
            text-align: center;
            color: #333;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .subject-buttons {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .subject-buttons a {
            display: block;
            width: 48%;
            margin-bottom: 10px;
            padding: 10px;
            background-color: #007BFF;
            color: #fff;
            text-align: center;
            text-decoration: none;
            border-radius: 5px;
        }
        .subject-buttons a:hover {
            background-color: #0056b3;
        }
        .upload-section {
            margin-top: 20px;
        }
        .upload-section label {
            display: block;
            margin-bottom: 10px;
        }
        .upload-section input[type="file"] {
            margin-bottom: 10px;
        }
        .upload-section input[type="date"] {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>

    <h1>Site de Urários Escolares</h1>

    <div class="container">
        <div class="subject-buttons">
            <a href="#matematica1">Matemática 1</a>
            <a href="#matematica2">Matemática 2</a>
            <a href="#fisica1">Física 1</a>
            <a href="#fisica2">Física 2</a>
            <a href="#portugues">Português</a>
            <a href="#quimica1">Química 1</a>
            <a href="#quimica2">Química 2</a>
            <a href="#historia">História</a>
            <a href="#geografia">Geografia</a>
        </div>

        <div class="upload-section">
            <h2>Upload de Urários</h2>
            <form action="upload.php" method="post" enctype="multipart/form-data">
                <label for="file">Selecione a imagem do urário:</label>
                <input type="file" name="file" id="file" required>
                
                <label for="uploadDate">Data do upload:</label>
                <input type="date" name="uploadDate" id="uploadDate" required>
                
                <input type="submit" value="Upload">
            </form>
        </div>
    </div>

</body>
</html>
