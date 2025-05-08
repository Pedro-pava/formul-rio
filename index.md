<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Primeiro Site HTML</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        h1, h4 {
            text-align: center;
        }
        .divprincipal {
            background-color: darkgreen;
            border: solid 2px #000;
            width: 600px;
            margin: 20px auto;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            color: white;
        }
        .divprincipal label {
            display: block;
            margin-top: 10px;
            font-weight: bold;
        }
        .divprincipal input, .divprincipal select {
            border-radius: 10px;
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border: 1px solid #ccc;
            box-sizing: border-box;
        }
        .divprincipal input:focus, .divprincipal select:focus {
            outline: none;
            border-color: #4CAF50;
        }
        button {
            background-color: green;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-size: 16px;
            margin: 20px auto;
            display: block;
            border-radius: 5px;
        }
        button:hover {
            background-color: darkgreen;
        }
    </style>
</head>
<body>
    <h1><b>MEU FIRST SITE HTML</b></h1>
    <h4>NÃO SE ESQUEÇA DE PREENCHER CORRETAMENTE</h4>
    <div class="divprincipal">
        <form action="#">
            <label for="txtNome">Nome:</label>
            <input id="txtNome" type="text" placeholder="Digite seu nome" required />

            <label for="txtSobrenome">Sobrenome:</label>
            <input id="txtSobrenome" type="text" placeholder="Digite seu sobrenome" required />

            <label for="txtAltura">Altura (cm):</label>
            <input id="txtAltura" type="number" placeholder="Digite sua altura em cm" required />

            <label for="txtCPF">CPF:</label>
            <input id="txtCPF" type="text" placeholder="Digite seu CPF" required pattern="\d{11}" title="Digite 11 números sem pontos ou traços" />

            <label for="intIdade">Data de Nascimento:</label>
            <input id="intIdade" type="date" required />

            <label for="selectLuz">Da luz Gay:</label>
            <select id="selectLuz" required>
                <option value="">Selecione</option>
                <option value="sim">SIM</option>
                <option value="super">SUPER</option>
                <option value="demais">DEMAIS</option>
            </select>
            
            <button type="submit" onclick="alert('REGISTRADO')">Salvar</button>
        </form>
    </div>
</body>
</html>
