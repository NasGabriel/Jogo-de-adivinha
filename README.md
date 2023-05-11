<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adivinhação</title>
</head>
<body>
    
</body>
</html>

<script>
    function pularLinha() {
        document.write("<br><br>");
    }

    function mostra(frase) {
        document.write(frase);
        pularLinha();
    }

    var numeroPensado = Math.round(Math.random() * 10);
    var tentativas = 1;

    while(tentativas <= 3) {
        var chute = parseInt(prompt("Digite o seu chute!"));

        if (chute == numeroPensado) {
            mostra("Você ACERTOU, o número pensado era " + numeroPensado);
            break;
        } else {
            mostra("Você ERROU!");
        }

        tentativas++;
    }

    mostra("FIM!")
</script>
