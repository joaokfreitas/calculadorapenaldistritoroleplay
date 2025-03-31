<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora Penal</title>
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #1e1e2f;
            color: #fff;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        .container {
            max-width: 900px;
            margin: 0 aut<a href="https://CALCULADORA PENAL DISTRITO"><a><a href="https://CALCULADORA_PENAL_DA_DISTRITO_ROLEPLAY" title="CALCULADORA PENAL"><!DOCTYPE html>
o;
            padding: 20px;
            background-color: #2d2d44;
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
        }
        h1 {
            text-align: center;
            font-size: 30px;
            color: #00ff95;
        }
        .tabs {
            display: flex;
            justify-content: space-evenly;
            margin-bottom: 20px;
        }
        .tabs button {
            padding: 12px 20px;
            background-color: #44485a;
            border: 2px solid #00ff95;
            border-radius: 10px;
            color: white;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
        }
        .tabs button:hover {
            background-color: #00ff95;
            color: #2d2d44;
        }
        .tabs button.active {
            background-color: #00ff95;
            color: #2d2d44;
        }
        .tab-content {
            display: none;
            margin-top: 20px;
        }
        .tab-content.active {
            display: block;
        }
        input, textarea, select {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            background-color: #33354b;
            border: 2px solid #44485a;
            border-radius: 8px;
            color: white;
        }
        button {
            padding: 12px 30px;
            background-color: #00ff95;
            color: #2d2d44;
            border: none;
            border-radius: 10px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s;
        }
        button:hover {
            background-color: #2d2d44;
            color: #00ff95;
        }
        .crime-category {
            margin: 20px 0;
        }
        .crime-button {
            padding: 10px 20px;
            margin: 5px;
            background-color: #44485a;
            border: 2px solid #44485a;
            border-radius: 10px;
            color: white;
            cursor: pointer;
            transition: all 0.3s;
        }
        .crime-button.active {
            background-color: #00ff95;
        }
        .output {
            padding: 15px;
            background-color: #33354b;
            border-radius: 8px;
            margin-top: 20px;
            white-space: pre-wrap;
            word-wrap: break-word;
        }
        .clean-button {
            background-color: #ff4b4b;
            color: #fff;
            border-radius: 8px;
            margin-top: 15px;
        }
        .clean-button:hover {
            background-color: #ff1a1a;
        }
        .copy-button {
            background-color: #4CAF50;
            color: white;
            border-radius: 8px;
            margin-top: 15px;
        }
        .copy-button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Calculadora Penal</h1>

    <!-- Tabs -->
    <div class="tabs">
        <button onclick="showTab('nome')" class="active">Nome do Meliante</button>
        <button onclick="showTab('id')">ID do Meliante</button>
        <button onclick="showTab('atenuantes')">Atenuantes</button>
        <button onclick="showTab('crimes')">Crimes</button>
        <button onclick="showTab('acoes')">Ações</button>
        <button onclick="showTab('homicidios')">Homicídios</button>
        <button onclick="showTab('coleta_genetica')">Coleta de Material Genético</button>
    </div>

    <!-- Tab Contents -->
    <div class="tab-content active" id="nome">
        <h3>Nome do Meliante</h3>
        <input type="text" id="nome-meliante" placeholder="Digite o nome do meliante" oninput="atualizarPenaEMulta()">
    </div>

    <div class="tab-content" id="id">
        <h3>ID do Meliante</h3>
        <input type="text" id="id-meliante" placeholder="Digite o ID do meliante" oninput="atualizarPenaEMulta()">
    </div>

    <div class="tab-content" id="atenuantes">
        <h3>Atenuantes</h3>
        <textarea id="atenuantes-meliante" placeholder="Descreva as atenuantes, se houver." oninput="atualizarPenaEMulta()"></textarea>
    </div>

    <div class="tab-content" id="crimes">
        <h3>Crimes</h3>
        <div class="crime-category">
            <h4>Infrações de Trânsito</h4>
            <button class="crime-button" onclick="toggleCrime(this, 'alta_velocidade', 2000, 0)">Alta Velocidade</button>
            <button class="crime-button" onclick="toggleCrime(this, 'direcao_perigosa', 4000, 0)">Direção Perigosa</button>
            <button class="crime-button" onclick="toggleCrime(this, 'estacionar_local_proibido', 2000, 0)">Estacionar em Local Proibido</button>
            <button class="crime-button" onclick="toggleCrime(this, 'pousar_local_proibido', 30000, 0)">Pousar em Local Proibido</button>
            <button class="crime-button" onclick="toggleCrime(this, 'manobra_imprudente', 50000, 0)">Manobra Imprudente com Aeronave</button>
        </div>
        <div class="crime-category">
            <h4>Outros Crimes</h4>
            <button class="crime-button" onclick="toggleCrime(this, 'veiculo_abandonado', 1500, 0)">Veículo Abandonado</button>
            <button class="crime-button" onclick="toggleCrime(this, 'trafegar_contramao', 2000, 0)">Tráfego na Contra Mão</button>
            <button class="crime-button" onclick="toggleCrime(this, 'dano_patrimonio', 2000, 0)">Dano ao Patrimônio</button>
            <button class="crime-button" onclick="toggleCrime(this, 'veiculo_danificado', 2000, 0)">Veículo Danificado</button>
            <button class="crime-button" onclick="toggleCrime(this, 'bloquear_vtr', 10000, 10)">Bloquear ou Danificar VTR</button>
            <button class="crime-button" onclick="toggleCrime(this, 'ameaca', 1000, 10)">Ameaça</button>
            <button class="crime-button" onclick="toggleCrime(this, 'roubo', 2000, 30)">Roubo</button>
            <button class="crime-button" onclick="toggleCrime(this, 'roubo_vtr', 20000, 500)">Roubo a VTR</button>
            <button class="crime-button" onclick="toggleCrime(this, 'associacao_criminosa', 1000, 10)">Associação Criminosa</button>
            <button class="crime-button" onclick="toggleCrime(this, 'corridas_ilegais', 2000, 20)">Corridas Ilegais</button>
            <button class="crime-button" onclick="toggleCrime(this, 'denuncia_caluniosa', 1000, 10)">Denúncia Caluniosa</button>
            <button class="crime-button" onclick="toggleCrime(this, 'desacato', 6000, 30)">Desacato</button>
            <button class="crime-button" onclick="toggleCrime(this, 'desobediencia', 2000, 20)">Desobediência</button>
            <button class="crime-button" onclick="toggleCrime(this, 'dolares_ilicitos', 1000, 20)">Dólares Ilícitos</button>
            <button class="crime-button" onclick="toggleCrime(this, 'estelionato', 2000, 30)">Estelionato</button>
            <button class="crime-button" onclick="toggleCrime(this, 'falsidade_ideologica', 2000, 15)">Falsidade Ideológica</button>
            <button class="crime-button" onclick="toggleCrime(this, 'falso_testemunho', 2000, 10)">Falso Testemunho</button>
            <button class="crime-button" onclick="toggleCrime(this, 'furto', 2000, 15)">Furto</button>
            <button class="crime-button" onclick="toggleCrime(this, 'invasao_propriedade', 1000, 20)">Invasão de Propriedade</button>
            <button class="crime-button" onclick="toggleCrime(this, 'invasao_propriedade_publica', 10000, 500)">Invasão de Propriedade Pública</button>
            <button class="crime-button" onclick="toggleCrime(this, 'lesao_corporeal', 1000, 10)">Lesão Corporal</button>
            <button class="crime-button" onclick="toggleCrime(this, 'multas_nao_pagas', 0, 10)">Multas Não Pagas</button>
            <button class="crime-button" onclick="toggleCrime(this, 'obstrucao_justica', 3500, 20)">Obstrução de Justiça</button>
        </div>
    </div>

    <!-- Nova aba Ações -->
    <div class="tab-content" id="acoes">
        <h3>Ações</h3>
        <button class="crime-button" onclick="toggleCrime(this, 'barbearia', 30, 1500)">Barbearia</button>
        <button class="crime-button" onclick="toggleCrime(this, 'loja_armas', 40, 2000)">Loja de Armas</button>
        <button class="crime-button" onclick="toggleCrime(this, 'loja_departamento', 65, 2500)">Loja de Departamento</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_central_com_refem_sem_fuga', 115, 8000)">Banco Central com Refém sem Fuga</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_central_com_refem_e_fuga', 105, 8000)">Banco Central com Refém e Fuga</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_central_sem_refem', 95, 4000)">Banco Central sem Refém</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_paleio', 95, 6000)">Banco Paletó</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_fleeca_com_refem_sem_fuga', 115, 8000)">Banco Fleeca com Refém sem Fuga</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_fleeca_com_refem_e_fuga', 105, 8000)">Banco Fleeca com Refém e Fuga</button>
        <button class="crime-button" onclick="toggleCrime(this, 'banco_fleeca_sem_refem', 95, 4000)">Banco Fleeca sem Refém</button>
        <button class="crime-button" onclick="toggleCrime(this, 'carro_forte', 95, 4000)">Carro Forte</button>
        <button class="crime-button" onclick="toggleCrime(this, 'niobio', 95, 8000)">Nióbio</button>
        <button class="crime-button" onclick="toggleCrime(this, 'joalheria', 75, 6000)">Joalheria</button>
    </div>

    <div class="tab-content" id="homicidios">
        <h3>Homicídios (25 Pena / 1000 Multa, 30 Pena / 1500 Multa)</h3>
        <input type="number" id="homicidios-1" placeholder="Número de homicídios (25 Pena / 1000 Multa)" min="0" oninput="atualizarPenaEMulta()">
        <input type="number" id="homicidios-2" placeholder="Número de homicídios (30 Pena / 1500 Multa)" min="0" oninput="atualizarPenaEMulta()">
    </div>

    <div class="tab-content" id="coleta_genetica">
        <h3>Coleta de Material Genético</h3>
        <select id="coleta-genetica" onchange="atualizarPenaEMulta()">
            <option value="0">Não Realizada</option>
            <option value="1500">Coleta Realizada (1500 Multa)</option>
        </select>
    </div>

    <!-- Resultado -->
    <div class="output" id="resultado">
        Resultado:
    </div>

    <button class="clean-button" onclick="clearAll()">Limpar Tudo</button>
    <button class="copy-button" onclick="copyText()">Copiar Informações</button>
</div>

<script>
    let crimes = {};

    function toggleCrime(button, crimeName, pena, multa) {
        if (crimes[crimeName]) {
            delete crimes[crimeName];
            button.classList.remove("active");
        } else {
            crimes[crimeName] = { pena, multa };
            button.classList.add("active");
        }
        atualizarPenaEMulta();
    }

    function showTab(tabId) {
        const tabs = document.querySelectorAll('.tab-content');
        tabs.forEach(tab => tab.classList.remove('active'));
        document.getElementById(tabId).classList.add('active');
    }

    function atualizarPenaEMulta() {
        const nome = document.getElementById("nome-meliante").value;
        const id = document.getElementById("id-meliante").value;
        const atenuantes = document.getElementById("atenuantes-meliante").value;

        let resultado = `Meliante: ${nome || 'Não informado'} (ID: ${id || 'Não informado'})\nAtenuantes: ${atenuantes || 'Nenhuma'}\nCrimes cometidos:\n`;
        let penaTotal = 0;
        let multaTotal = 0;

        for (let crime in crimes) {
            const { pena, multa } = crimes[crime];
            resultado += `- ${crime}: ${pena} anos de pena / ${multa} de multa\n`;
            penaTotal += pena;
            multaTotal += multa;
        }

        const homicidios1 = document.getElementById('homicidios-1').value || 0;
        const homicidios2 = document.getElementById('homicidios-2').value || 0;
        penaTotal += homicidios1 * 25 + homicidios2 * 30;
        multaTotal += homicidios1 * 1000 + homicidios2 * 1500;

        const coletaGenetica = document.getElementById('coleta-genetica').value;
        if (coletaGenetica === "1500") {
            multaTotal += 1500;
        }

        if (penaTotal === 0) {
            resultado += `\nResultado: Nenhum crime cometido.\n`;
        } else {
            resultado += `\nPena total: ${penaTotal} anos\nMulta total: ${multaTotal}`;
        }

        document.getElementById("resultado").textContent = resultado;
    }

    function clearAll() {
        document.getElementById("nome-meliante").value = '';
        document.getElementById("id-meliante").value = '';
        document.getElementById("atenuantes-meliante").value = '';
        crimes = {};
        atualizarPenaEMulta();
        document.querySelectorAll(".crime-button").forEach(button => button.classList.remove("active"));
        document.getElementById('homicidios-1').value = '';
        document.getElementById('homicidios-2').value = '';
        document.getElementById('coleta-genetica').value = '0';
    }

    function copyText() {
        const resultadoText = document.getElementById("resultado").textContent;
        const textArea = document.createElement("textarea");
        textArea.value = resultadoText;
        document.body.appendChild(textArea);
        textArea.select();
        document.execCommand('copy');
        document.body.removeChild(textArea);
        alert("Informações copiadas para a área de transferência!");
    }
</script>

</body>
</html>
</a></a></a>
