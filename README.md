# CRUD
<hello name="{{ name }}"></hello>
<p>
  
<img class="img-responsive" src="https://www.cursosdesarrolloweb.com/static/60b0a53150f04957faba4a5630a0d938/88b18/angular_peque.jpg">
</p>

<html>
 <head>
 <title> Como criar um formulário completo em Crud, HTML, CSS e ANGULAR 11 </title>
 <meta name="description" content="Aprenda a criar um site completo que usa formulários em HTML">
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8"> 
 </head>

 <body>
  <h1> Buenos Dias!</h1> 
  <h2> Linguagem usadas Angular, HTML & CSS</h2><br />

<form action="Script_do_Formulario.php" method="post">

<!-- DADOS PESSOAIS-->
<fieldset>
 <legend>Dados Pessoais</legend>
 <table cellspacing="10">
  <tr>
   <td>
    <label for="nome">Nome: </label>
   </td>
   <td align="left">
    <input type="text" name="email">
   </td>
   <td>
    <label for="sobrenome">Sobrenome: </label>
   </td>
   <td align="left">
    <input type="text" name="sobrenome">
   </td>
  </tr>
  <tr>
   <td>
    <label>Nascimento: </label>
   </td>
   <td align="left">
    <input type="text" name="dia" size="2" maxlength="2" value="dd"> 
   <input type="text" name="mes" size="2" maxlength="2" value="mm"> 
   <input type="text" name="ano" size="4" maxlength="4" value="aaaa">
   </td>
  </tr>
  <tr>
   <td>
    <label for="rg">RG: </label>
   </td>
   <td align="left">
    <input type="text" name="rg" size="13" maxlength="13"> 
   </td>
  </tr>
  <tr>
   <td>
    <label>CPF:</label>
   </td>
   <td align="left">
    <input type="text" name="cpf" size="9" maxlength="9"> - <input type="text" name="cpf2" size="2" maxlength="2">
   </td>
   
  </tr>
 </table>
</fieldset>

<br />
<!-- ENDEREÇO -->
<fieldset>
 <legend>Dados de Endereço</legend>
 <table cellspacing="10">

  <tr>
   <td>
    <label for="rua">Rua:</label>
   </td>
   <td align="left">
    <input type="text" name="rua">
   </td>
   <td>
    <label for="numero">Numero:</label>
   </td>
   <td align="left">
    <input type="text" name="numero" size="4">
   </td>
  </tr>
  <tr>
   <td>
    <label for="bairro">Bairro: </label>
   </td>
   <td align="left">
    <input type="text" name="bairro">
   </td>
  </tr>
  <tr>
   <td>
    <label for="estado">Estado:</label>
   </td>
   <td align="left">
    <select name="estado"> 
    <option value="ac">Acre</option> 
    <option value="al">Alagoas</option> 
    <option value="am">Amazonas</option> 
    <option value="ap">Amapá</option> 
    <option value="ba">Bahia</option> 
    <option value="ce">Ceará</option> 
    <option value="df">Distrito Federal</option> 
    <option value="es">Espírito Santo</option> 
    <option value="go">Goiás</option> 
    <option value="ma">Maranhão</option> 
    <option value="mt">Mato Grosso</option> 
    <option value="ms">Mato Grosso do Sul</option> 
    <option value="mg">Minas Gerais</option> 
    <option value="pa">Pará</option> 
    <option value="pb">Paraíba</option> 
    <option value="pr">Paraná</option> 
    <option value="pe">Pernambuco</option> 
    <option value="pi">Piauí</option> 
    <option value="rj">Rio de Janeiro</option> 
    <option value="rn">Rio Grande do Norte</option> 
    <option value="ro">Rondônia</option> 
    <option value="rs">Rio Grande do Sul</option> 
    <option value="rr">Roraima</option> 
    <option value="sc">Santa Catarina</option> 
    <option value="se">Sergipe</option> 
    <option value="sp">São Paulo</option> 
    <option value="to">Tocantins</option> 
   </select>
   </td>
  </tr>
  <tr>
   <td>
    <label for="cidade">Cidade: </label>
   </td>
   <td align="left">
    <input type="text" name="cidade">
   </td>
  </tr>
  <tr>
   <td>
    <label for="cep">CEP: </label>
   </td>
   <td align="left">
    <input type="text" name="cep" size="5" maxlength="5"> - <input type="text" name="cep2" size="3" maxlength="3">
   </td>
  </tr>
 </table>
</fieldset>
<br />

<!-- DADOS DE LOGIN -->
<fieldset>
 <legend>Dados de login</legend>
 <table cellspacing="10">
  <tr>
   <td>
    <label for="email">E-mail: </label>
   </td>
   <td align="left">
    <input type="text" name="email">
   </td>
  </tr>
  <tr>
   <td>
    <label for="imagem">Imagem de perfil:</label>
   </td>
   <td>
    <input type="file" name="imagem" >

   </td>
  </tr>
  <tr>
   <td>
    <label for="login">Login de usuário: </label>
   </td>
   <td align="left">
    <input type="text" name="login">
   </td>
  </tr>
  <tr>
   <td>
    <label for="pass">Senha: </label>
   </td>
   <td align="left">
    <input type="password" name="pass">
   </td>
  </tr>
  <tr>
   <td>
    <label for="passconfirm">Confirme a senha: </label>
   </td>
   <td align="left">
    <input type="password" name="passconfirm">
   </td>
  </tr>
 </table>
</fieldset>
<br />
<input type="submit">
<input type="reset" value="Limpar">
</form>

 </body>
</html>
<script type="text/javascript">
function validaForm(frm) {
/*
o parâmetro frm desta função significa: this.form,
pois a chamada da função - validaForm(this) foi
definida na tag form.
*/
    //Verifica se o campo nome foi preenchido e
    //contém no mínimo três caracteres.
    if(frm.nome.value == """ || frm.nome.value == null || frm.nome.value.lenght < 3) {
        //É mostrado um alerta, caso o campo esteja vazio.
        alert("Por favor, indique o seu nome.");
        //Foi definido um focus no campo.
        frm.nome.focus();
        //o form não é enviado.
        return false;
    }
    //o campo e-mail precisa de conter: "@", "." e não pode estar vazio
    if(frm.email.value.indexOf("@") == -1 ||
      frm.email.valueOf.indexOf(".") == -1 ||
      frm.email.value == "" ||
      frm.email.value == null) {
        alert("Por favor, indique um e-mail válido.");
        frm.email.focus();
        return false;
    }
    // O utilizador necessita de selecionar um dos dois
    //radio buttons: Masculino ou Feminino.
    escolhaSexo = -1; //valor negativo default (padrão) que significa que nada foi escolhido ainda.
    //No bloco de código abaixo foi criado um ciclo entre
    //os radios button com o mesmo nome (sexo)
    for(x = frm.sexo.lenght -1; x > -1; x--) {
        /*
        x = frm.sexo.lenght -1 é a mesma coisa que: x = 2-
        1, que resulta em 1.
        x > -1 significa que o valor de x não pode ser igual a -1 e
        sim maior, porque -1 significa que nada foi escolhido.
        x-- significa que há um decremento no valor x, é algo como:
        x = 1, x= 0 e pára pois x não pode ser -1.
        */
        if(frm.sexo[x].checked) { //checked quer dizer selecionado,
           //então verifica se o primeiro (0) ou o
           //segundo (1) radio button foi selecionado (checked).
           escolhaSexo = x; //atribui à variável escolhaSexo o valor X.
        }
    }
    //se nenhuma das opções (masculino ou feminino) forem
    //escolhidas, mostra um alerta e cancela o envio.
    if(escolhaSexo == -1) {
        alert("qual o seu sexo?");
        frm.sexo[0].focus();
        return false;
    }
    /* valida a profissão:
    O utilizador tem de escolher uma entre as três opções
    (Programador, Designer e Tester).
    */
    if(frm.prof.value == "" || from.prof.value == "Todas") {
        alert("De momento, precisamos de especialistas nas três áreas indicadas");
        frm.prof.focus();
        return false;
    }
    //Valida a textArea, que é como validar um campo de texto simples.
    if(frm.sobre.value == "" || frm.sobre.value == null) {
        alert("Por favor, conte-nos um pouco sobre si.");
        frm.sobre.focus();
        return false;
    }
}
</script>
<form action="/action_page.php">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <form>
    <p>Qual sua idade?</p>
    <input type="radio" name="idade" value="18_22">18 a 22 <br>
    <input type="radio" name="idade" value="23_30">23 a 30 <br>
    <input type="radio" name="idade" value="mais31">acima de 31<br>
</form>
<script type="text/javascript" src="http://code.jquery.com/jquery-2.1.3.min.js"></script>
<script type="text/javascript" src="https://assets.moip.com.br/v2/bank-account-validator.min.js"></script>
<script type="text/javascript">
  $(document).ready(function() {
    $("#validate_bank_account").click(function() {
      Moip.BankAccount.validate({
        bankNumber         : $("#bank_number").val(),
        agencyNumber       : $("#agency_number").val(),
        agencyCheckNumber  : $("#agency_check_number").val(),
        accountNumber      : $("#account_number").val(),
        accountCheckNumber : $("#account_check_number").val(),
        valid: function() {
          alert("Conta bancária válida")
        },
        invalid: function(data) {
          var errors = "Conta bancária inválida: \n";
          for(i in data.errors){
            errors += data.errors[i].description + "-" + data.errors[i].code + ")\n";
          }
          alert(errors);
        }
      });
    });
  });
</script>
<form>
  <select id="bank_number">
    <option value="001">BANCO DO BRASIL S.A.</option>
    <option value="237">BANCO BRADESCO S.A.</option>
    <option value="341">BANCO ITAÚ S.A.</option>
    <option value="104">CAIXA ECONOMICA FEDERAL</option>
    <option value="033">BANCO SANTANDER BANESPA S.A.</option>
    <option value="399">HSBC BANK BRASIL S.A.</option>
    <option value="151">BANCO NOSSA CAIXA S.A.</option>
    <option value="745">BANCO CITIBANK S.A.</option>
    <option value="041">BANCO DO ESTADO DO RIO GRANDE DO SUL S.A.</option>
  </select>

  <input id="agency_number" placeholder="Agência" type="text"/>
  <input id="agency_check_number" placeholder="Dígito da agência" type="text" />
  <input id="account_number" placeholder="Conta corrente" type="text" />
  <input id="account_check_number" placeholder="Dígito da conta corrente" type="text" />

  <input type="button" value="Validar" id="validate_bank_account" />
</form>

  <input type="image" src="http://pereiralonas.com.br/uploads/med/2017420105456307.jpg" alt="Submit" width="150" height="100">
</form>
<form>
    Defina seu nível de satisfação:<br>
    pouco satisfeito
    <input type="range" name="satisfacao" min="0" max="10">
    muito satisfeito
</form>
<form>
    Link do seu WebSite: <input type="url" name="webpage">
</form>

<img class="img-responsive" src="http://4.bp.blogspot.com/_ZJm2dmGyJIY/S_lPybezE5I/AAAAAAAABAc/EPpqRt2H0N0/s320/descanso.png">
