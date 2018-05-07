# Mudança de Background de acordo com o tempo, em desenvolvimento Web.
Como o próprio nome já diz, neste "Script" mostra um método bem simples e de fácil compreensão que encontrei para aplicar mudança de cores/imagens no background de acordo com o horário.

<!DOCTYPE html>
<html>
<head>
<style>

.manha {
  background-color: lightblue;
}

.tarde {
  background-color: orange;
}

.noite {
  background-color: black;
}

</style>
</head>
<body>
  <script> 

   var date = new Date();

   var hour = date.getHours();

if (hour < 13) {
  document.body.classList.add('manha'); // De acordo com o horário, adicione uma class para o documento em body
} 
else if (hour < 18) {
  document.body.classList.add('tarde');
} 
else {
  document.body.classList.add('noite');
  
}

   </script>
</body>
</html>


Criando classes específicas para cada imagem diferente, as determinei por "manha", "tarde" e "noite", desde modo, cada um deles terá uma imagem de fundo diferente, dependendo do horário especificado também.
Usando o comando "document.body.classList.add('Nome da classe');" para criar um elemento. 
Configurando o em CSS também é simples: ".classe".

Peço perdão caso eu tenha cometido algum erro em relação aos diretórios do "post" e obrigado pela compreensão, espero que seja útil.
