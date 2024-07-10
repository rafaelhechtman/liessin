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
        h1, h2 {
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
        .upload-section input[type="file"], .upload-section input[type="date"] {
            margin-bottom: 10px;
        }
        .uploaded-images {
            margin-top: 20px;
        }
        .uploaded-images img {
            max-width: 100%;
            margin-bottom: 10px;
        }
        .hidden {
            display: none;
        }
    </style>
    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => section.classList.add('hidden'));
            document.getElementById(sectionId).classList.remove('hidden');
        }
    </script>
</head>
<body>

    <h1>Site de Urários Escolares</h1>

    <div class="container">
        <div class="subject-buttons">
            <a href="#" onclick="showSection('matematica1')">Matemática 1</a>
            <a href="#" onclick="showSection('matematica2')">Matemática 2</a>
            <a href="#" onclick="showSection('fisica1')">Física 1</a>
            <a href="#" onclick="showSection('fisica2')">Física 2</a>
            <a href="#" onclick="showSection('portugues')">Português</a>
            <a href="#" onclick="showSection('quimica1')">Química 1</a>
            <a href="#" onclick="showSection('quimica2')">Química 2</a>
            <a href="#" onclick="showSection('historia')">História</a>
            <a href="#" onclick="showSection('geografia')">Geografia</a>
        </div>

        <div id="matematica1" class="section hidden">
            <h2>Matemática 1</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="matematica1">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="matematica2" class="section hidden">
            <h2>Matemática 2</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="matematica2">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <!-- Adicione seções semelhantes para outras disciplinas aqui -->

        <div id="fisica1" class="section hidden">
            <h2>Física 1</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="fisica1">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="fisica2" class="section hidden">
            <h2>Física 2</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="fisica2">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="portugues" class="section hidden">
            <h2>Português</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="portugues">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="quimica1" class="section hidden">
            <h2>Química 1</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="quimica1">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="quimica2" class="section hidden">
            <h2>Química 2</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="quimica2">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="historia" class="section hidden">
            <h2>História</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="historia">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>

        <div id="geografia" class="section hidden">
            <h2>Geografia</h2>
            <div class="upload-section">
                <form action="upload.php" method="post" enctype="multipart/form-data">
                    <label for="file">Selecione a imagem do urário:</label>
                    <input type="file" name="file[]" id="file" multiple required>
                    
                    <label for="uploadDate">Data do upload:</label>
                    <input type="date" name="uploadDate[]" id="uploadDate" multiple required>
                    
                    <input type="hidden" name="subject" value="geografia">
                    <input type="submit" value="Upload">
                </form>
            </div>
            <div class="uploaded-images">
                <h2>Imagens Enviadas</h2>
                <!-- As imagens enviadas serão exibidas aqui -->
            </div>
        </div>
    </div>

</body>
</html>
