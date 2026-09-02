# ☕ Café & Companhia — Landing Page

Página web simples com tema de cafeteria, criada utilizando apenas HTML e CSS.

## 🎯 Objetivo

Criar uma interface inicial intuitiva para apresentar a cafeteria e permitir que os clientes façam reservas de forma online.

## 💻 Tecnologias

* HTML5
* CSS3
* Design responsivo
* Sem frameworks ou bibliotecas externas

## 📄 Código

```html
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Café & Companhia - Reservas</title>
<style>
    /* Configuração geral da página */
body {
    font-family: Arial, sans-serif;
    background-color: #f5eee6;
    color: #3e2723;
    padding: 20px;
}

/* Tamanho e alinhamento da Logo */
.logo {
    display: block;
    width: 150px;
    margin: 0 auto;
}

/* Caixa principal do formulário */
#reservas {
    background-color: white;
    max-width: 500px;
    margin: 20px auto;
    padding: 20px;
    border-radius: 10px;
}

/* Título principal */
h2 {
    text-align: center;
    color: #5d4037;
}

/* Subtítulos de cada campo */
h3 {
    font-size: 14px;
    margin-top: 15px;
    margin-bottom: 5px;
}

/* Campos para digitar e caixa de seleção */
input, select {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
}

/* Caixinha do ambiente (interno/externo) */
fieldset {
    margin-top: 15px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

/* Ajuste dos botões redondos de opção */
fieldset input[type="radio"] {
    width: auto;
}

/* Botão de enviar */
button {
    width: 100%;
    padding: 12px;
    margin-top: 20px;
    background-color: #6d4c41;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
}

/* Cor do botão ao passar o mouse */
button:hover {
    background-color: #4e342e;
}
</style>
</head>

<body>

    <!-- Logo -->
    <img src="logo-cc.png" alt="Logo do Café & Companhia" class="logo">

    <!-- Área de reserva -->
    <section id="reservas">

        <h2>Reserve sua mesa para garantir sua experiência</h2>

        <!-- Formulário -->
        <form>

            <h3>Informe seu nome:</h3>
            <input type="text" id="nome" name="nome"
                placeholder="Digite seu nome..." required>

            <h3>Informe seu e-mail:</h3>
            <input type="email" id="email" name="email"
                placeholder="Digite seu e-mail..." required>

            <h3>Informe seu telefone:</h3>
            <input type="tel" id="telefone" name="telefone"
                placeholder="Digite seu telefone..." required>

            <h3>Data da reserva:</h3>
            <input type="date" id="data" name="data" required>

            <h3>Horário da reserva:</h3>
            <input type="time" id="horario" name="horario" required>

            <h3>Quantidade de pessoas:</h3>

            <select id="pessoas" name="pessoas" required>
                <option value="">Selecione</option>
                <option value="1">1 pessoa</option>
                <option value="2">2 pessoas</option>
                <option value="3">3 pessoas</option>
                <option value="4">4 pessoas</option>
                <option value="5">5 pessoas</option>
            </select>

            <!-- Ambiente -->
            <fieldset>

                <legend>Escolha o ambiente:</legend>

                <label>
                    <input type="radio" name="ambiente" value="interno">
                    Ambiente interno
                </label>

                <label>
                    <input type="radio" name="ambiente" value="externo">
                    Ambiente externo
                </label>

            </fieldset>

            <!-- Botão -->
            <button type="submit">Confirmar Reserva</button>

        </form>

    </section>

</body>

</html>
