<template>
  <main role="main" class="pb-5">
    <div class="container">
      <div class="row">
        <div class="col-md-8">
          <h3>Dados Pessoais</h3>
          <label class="form-label">Nome completo</label>
          <input type="name" name="nome" class="form-control">
          <br>
          <div class="row">
            <div class="col-md-6">
              <label for="exampleFormControlInput1" class="form-label">Email</label>
              <input type="email" name="email" class="form-control" id="exampleFormControlInput1">
            </div>
            <div class="col-md-6">
              <label for="inputPassword5" class="form-label">Senha</label>
              <input type="password" name="senha" id="inputPassword5" class="form-control"
                aria-describedby="passwordHelpBlock">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Data de Nascimento</label>
              <input type="text" name="data_nasc" class="form-control">
            </div>
            <div class="col-md-6">
              <label class="form-label">CPF</label>
              <input type="tel" name="celular" class="form-control">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Possui filhos ou dependentes?</label>
              <select name="filhos" class="form-control">
                <option>Selecione</option>
                <option value="Não">Não</option>
                <option value="Sim">Sim</option>
              </select>
            </div>
            <div class="col-md-6">
              <label class="form-label">Quantos filhos ou dependentes?</label>
              <select name="quantfilhos" class="form-control">
                <option>Selecione</option>
                <option value="Não possui">Não posssui</option>
                <option value="1">1</option>
                <option value="2">2</option>
                <option value="3">3</option>
                <option value="4">4</option>
                <option value="Mais de 5">Mais de 5</option>
              </select>
            </div>
          </div>
          <br>


          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Estado cívil</label>
              <select name="estadocivil" class="form-control">
                <option>Selecione</option>
                <option value="Casado(a)">Casado(a)</option>
                <option value="Divorciado(a)">Divorciado(a)</option>
                <option value="Solteiro(a)">Solteiro(a)</option>
                <option value="União Estavel">União Estavel</option>
                <option value="Viúvo(a)">Viúvo(a)</option>
              </select>
            </div>
            <div class="col-md-6">
              <label class="form-label">Sexo</label>
              <select name="sexo" class="form-control">
                <option>Selecione</option>
                <option value="feminino">Feminino</option>
                <option value="masculino">Masculino</option>
                <option value="outro">Outro</option>
              </select>
            </div>
          </div>
          <br>
          <form method="get" action=".">
     
          <div class="row">
            <div class="col-md-3">
              <label class="form-label">CEP</label>
              <input type="text" name="cep" id="cep" value="" size="10" maxlength="9" onblur="pesquisacep(this.value);" class="form-control">
              <small class="form-text text-muted">Seu endereço será preenchido automaticamente</small>
            </div>
          </div>
          <br>


          <div class="row">
            <div class="col-md-8">
              <label class="form-label">Endereço</label>
              <input name="rua" type="text" id="rua" class="form-control">
            </div>
            <div class="col-md-4">
              <label class="form-label">Número</label>
              <input type="text" name="numero" class="form-control">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Complemento</label>
              <input type="text" name="complemento" class="form-control">
            </div>
            <div class="col-md-6">
              <label class="form-label">Bairro</label>
              <input name="bairro" type="text" id="bairro" class="form-control">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Estado</label>
              <input name="uf" type="text" id="uf" class="form-control">
            </div>
            <div class="col-md-6">
              <label class="form-label">Cidade</label>
              <input name="cidade" type="text" id="cidade" class="form-control">
            </div>
          </div>
          <br>
        </form>
          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Telefone Residencial</label>
              <input type="text" name="email" class="form-control">
            </div>
            <div class="col-md-6">
              <label class="form-label">Telefone Comercial</label>
              <input type="text" name="senha" class="form-control">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Telefone de Contato</label>
              <input type="text" name="data_nasc" class="form-control">
            </div>
            <div class="col-md-6">
              <label class="form-label">Ramal</label>
              <input type="tel" name="celular" class="form-control">
            </div>
          </div>
          <br>
          <label class="form-label">Telefone Celular</label>
          <input type="name" name="nome" class="form-control">
          <br>
          <div class="row">
            <div class="col-md-6">
              <label class="form-label">Possui alguma deficiência?</label>
              <select class="form-control" name="def">
                <option value="">Selecione</option>
                <option value="0">Não</option>
                <option value="1">Sim</option>
              </select>
            </div>
            <div class="col-md-6">
              <label for="inputPassword5" class="form-label">Qual deficiência?</label>
              <input type="text" name="deficiencia" class="form-control">
            </div>
          </div>
          <br>


          <h3>Formação Complementar</h3>

          <h4 class="font-weight-bolder text-smalt-blue text-uppercase">Curso <span id="count">01</span></h4>

          <div class="row">
            <div class="col-md-6">
              <label>Formação </label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="2">1º Grau (5º a 9º Série)</option>
                <option value="3">2º Grau (1º a 3º Ano)</option>
                <option value="5">3º Grau (Graduação)</option>
                <option value="1">Ensino Fundamental (1º a 4º Série)</option>
                <option value="9">Pós Graduação (Doutorado)</option>
                <option value="6">Pós Graduação (Especialização)</option>
                <option value="7">Pós Graduação (MBA)</option>
                <option value="8">Pós Graduação (Mestrado)</option>
              </select>
            </div>
            <div class="col-md-6">
              <label>Curso</label>
              <input type="text" class="form-control" name="" value="">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label>Situação do Curso</label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="1">Concluído</option>
                <option value="2">Cursando</option>
                <option value="3">Trancado</option>
              </select>
            </div>
            <div class="col-md-6">
              <label>Mês e Ano de conclusão</label>
              <input type="text" class="form-control" name="">
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label>Turno</label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="M">Matutino</option>
                <option value="V">Vespertino</option>
                <option value="N">Noturno</option>
                <option value="I">Integral</option>
              </select>
            </div>
            <div class="col-md-6">
              <label>Instituição</label>
              <input type="text" class="form-control" name="" value="">
            </div>
          </div>
          <br>

          <button class="more blue add-formation" type="button">+ Formação Complementar</button>

          <h3>Cursos Adicionais</h3>
          <label>Nível de Experiência em Espanhol</label>
          <select class="form-control" name="CurriculumCourseAdditional[6][nivel]">
            <option value="">Selecione</option>
            <option value="N">Nenhuma</option>
            <option value="B">Básico</option>
            <option value="I">Intermediário</option>
            <option value="A">Avançado</option>
          </select>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label>Nível de Experiência em Excel</label>
              <select class="form-control" name="CurriculumCourseAdditional[1][nivel]">
                <option value="">Selecione</option>
                <option value="N">Nenhuma</option>
                <option value="B">Básico</option>
                <option value="I">Intermediário</option>
                <option value="A">Avançado</option>
              </select>
            </div>
            <div class="col-md-6">
              <label>Nível de Experiência em Informática</label>
              <select class="form-control" name="CurriculumCourseAdditional[7][nivel]">
                <option value="">Selecione</option>
                <option value="N">Nenhuma</option>
                <option value="B">Básico</option>
                <option value="I">Intermediário</option>
                <option value="A">Avançado</option>
              </select>
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label>Nível de Experiência em Inglês</label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="N">Nenhuma</option>
                <option value="B">Básico</option>
                <option value="I">Intermediário</option>
                <option value="A">Avançado</option>
              </select>
            </div>
            <div class="col-md-6">
              <label>Nível de Experiência em Internet</label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="N">Nenhuma</option>
                <option value="B">Básico</option>
                <option value="I">Intermediário</option>
                <option value="A">Avançado</option>
              </select>
            </div>
          </div>
          <br>

          <div class="row">
            <div class="col-md-6">
              <label>Nível de Experiência em PowerPoint</label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="N">Nenhuma</option>
                <option value="B">Básico</option>
                <option value="I">Intermediário</option>
                <option value="A">Avançado</option>
              </select>
            </div>
            <div class="col-md-6">
              <label>Nível de Experiência em Word</label>
              <select class="form-control" name="">
                <option value="">Selecione</option>
                <option value="N">Nenhuma</option>
                <option value="B">Básico</option>
                <option value="I">Intermediário</option>
                <option value="A">Avançado</option>
              </select>
            </div>
          </div>
          <br>

          <label>Outros</label>
          <div class="block">
            <input type="text" class="form-control" name="" value="">
          </div>


          <h3>Experiência Profissional</h3>

          <div id="copy-professional">
            <h4 class="box_header font-weight-bolder text-smalt-blue text-uppercase">
              Experiência <span id="count">01</span>
            </h4>

            <div class="row">
              <div class="col-6">
                <div class="form-group">
                  <label>Empresa</label>
                  <input type="text" class="form-control" name="" value="">
                </div>
              </div>
              <div class="col-6">
                <div class="form-group">
                  <label>Cargo</label>
                  <input type="text" class="form-control" name="" value="">
                </div>
              </div>
            </div>
            <br>

            <div class="row">
              <div class="col-6">
                <div class="form-group">
                  <label>Período de</label>
                  <input type="text" class="form-control" name="">
                </div>

              </div>
              <div class="col-6">
                <div class="form-group">
                  <label>até</label>
                  <input type="text" class="form-control" name="">
                </div>
              </div>
            </div>
            <br>

          </div>
          <div class="text-right">
            <button class="more blue add-professional" type="button">+ Experiência Profissional</button>
          </div>


          <h3>Informações Adicionais</h3>


          <div class="form-group">
            <label>Informações adicionais</label>
            <textarea class="form-control" name="" rows="5"></textarea>
          </div>
          <br>

          <div class="form-group">
            <label>Disponibilidade de horário</label>
            <select class="form-control" name="" aria-required="true">
              <option value="">Selecione</option>
              <option value="M">Manhã</option>
              <option value="T">Tarde</option>
              <option value="N">Noite</option>
              <option value="I">Integral</option>
            </select>
          </div>
          <br>

          <div class="form-group">
            <label>Área pretendida</label>
            <select class="form-control" name="">
              <option value="">Selecione</option>
              <option value="20">Administrativo</option>
              <option value="19">Aprendizes</option>
              <option value="23">Central de Guias</option>
              <option value="2">Compras</option>
              <option value="10">Comunicação</option>
              <option value="22">Contabilidade</option>
              <option value="3">Copa</option>
              <option value="4">Enfermagem</option>
              <option value="5">Farmácia</option>
              <option value="6">Faturamento</option>
              <option value="7">Financeiro</option>
              <option value="8">Fisioterapia</option>
              <option value="9">Informática</option>
              <option value="11">Limpeza</option>
              <option value="18">Medicina do Trabalho</option>
              <option value="21">Motorista</option>
              <option value="12">Nutrição</option>
              <option value="14">Portaria</option>
              <option value="13">Psicologia</option>
              <option value="15">Recepção</option>
              <option value="16">Recursos Humanos</option>
              <option value="1">Serviço Social</option>
              <option value="17">Tesouraria</option>
            </select>
          </div>
          <br>

          <div class="form-group">
            <label for="">Função</label>
            <select id="" class="form-control">

            </select>
          </div>

          <br>
          <button type="submit" class="more blue">Enviar</button>
        </div>



        <div class="col-md-4">
          <div class="blue-box">
            <h3>Entre em contato</h3>
            <p>Você pode entrar em contato conosco por telefone, por e-mail ou pelo nosso nosso
              <a href="https://hospcoracao.com.br/contato"
                style="border-bottom: 1px solid rgba(254, 250, 250, 0.65)">formulario de
                contato </a>
            </p>
            <ul class="list-unstyled">
              <li><i class="fa fa-phone"></i> (43) 3315-2000</li>
              <li><i class="fa fa-envelope"></i> <a
                  href="mailto:rh@hospcoracao.com.br?subject=Contato">rh@hospcoracao.com.br</a><br>
              </li>
              <li><i class="fa-clock-o"></i> 24 horas<br></li>
              <li><i class="fa fa-map-marker"></i> Rua Paes Leme, 1351 Londrina, PR 86060-610<br></li>
            </ul>
          </div>
          <br><br>
          <h3>Hospital do Coração de Londrina</h3>
          <ul class="list-unstyled columns no_padding page_margin_top clearfix">
            <li class="column_left">Rua Paes Leme, 1351 Londrina, PR 86060-610</li>
          </ul>
          <ul class="list-unstyled contact_data page_margin_top">
            <li class="clearfix">
              <span class="social_icon phone"></span>
              <p class="value"><strong>(43) 3315-2000</strong></p>
            </li>
            <li class="clearfix">
              <span class="social_icon mail"></span>
              <p class="value"><a href="mailto:rh@hospcoracao.com.br">rh@hospcoracao.com.br</a></p>
            </li>
          </ul>

          <h3 class="page_margin_top">Telefones Úteis</h3>
          <ul class="list-unstyled contact_data page_margin_top">
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Agendamento de consultas (WhatsApp): <strong>(43) 3315-2145</strong></p>
            </li>
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Hemodinâmica: <strong>(43) 3315-2058</strong></p>
            </li>
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Imprensa: <strong>(43) 3315-2133</strong></p>
            </li>
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Tesouraria: <strong>(43) 3315-2065</strong></p>
            </li>
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Unidade Bandeirantes: <strong>(43) 3315-2145</strong></p>
            </li>
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Unidade Bela Suíça: <strong>(43) 3305-8200</strong></p>
            </li>
            <li class="clearfix"><span class="social_icon phone"></span>
              <p class="value">Unidade Paes Leme: <strong>(43) 3315-2000</strong></p>
            </li>
          </ul>

          <h3 class="page_margin_top">Processo Seletivo de Residência Médica</h3>
          <p>Inscreva-se no Programa de Residência Médica do Hospital do Coração de Londrina por telefone, e-mail ou
            pelo
            nosso formulário de inscrição.</p>
          <ul class="list-unstyled contact_data">
            <li class="clearfix">
              <span class="social_icon phone"></span>
              <p class="value">
                <a href="tel:4333152137">(43) 3315-2137</a>
              </p>
            </li>
            <li class="clearfix">
              <span class="social_icon mail"></span>
              <p class="value">
                <a href="mailto:cep@hospcoracao.com.br">cep@hospcoracao.com.br</a>
              </p>
            </li>
            <li class="clearfix">
              <span class="social_icon time"></span>
              <p class="value">Seg a Sex: 8h30 às 12h | 13h às 18h</p>
            </li>

            <li class="clearfix">
              <span class="social_icon home"></span>
              <p class="value">Rua Paes Leme, 1351 - Londrina/PR</p>
            </li>
          </ul>
        </div>

      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.breadcrumb {
  background: none;
  border-bottom: 1px solid #cecece;
  border-top: 1px solid #cecece;
  text-transform: uppercase;
  font-size: 12px;
}

.breadcrumb-item+.breadcrumb-item::before {
  content: '>';
}

h3 {
  margin: 0 0 20px;
  /* font-weight: bold; */
  font-size: 24px;
  margin: 20px 0 10px;
  font-weight: 400;
  border-bottom: 2px solid #DDD;
  /* color: #45b3ee; */
  padding-bottom: 15px;
  line-height: 30px;
}

.blue-box {
  background: #41b3e5;
  color: #fff;
  padding: 25px 25px 0;
}

.blue-box h3 {
  color: #fff;
  border-bottom: 1px solid #FFF;
  line-height: 30px;
  font-weight: 400;
  font-size: 24px;
  margin: 0;
  padding-bottom: 15px;
  margin-bottom: 15px;
}

.blue-box ul li {
  border-top: 1px solid #7bcaed;
  font-weight: 300;
  padding: 20px 0;
}

.blue-box a {
  COLOR: #FFF;
}

.blue-box ul li i {
  font-size: 18px;
  margin-right: 10px;
}

.blue-box p {
  font-size: 14px;
  font-weight: 300;
  line-height: 25px;
}

.more {
  color: #0072B4;
  line-height: normal;
  background: #FFFFFF;
  padding: 20px 50px;
  text-transform: uppercase;
  text-decoration: initial;
}

.more.blue {
  /* border-color: #3156A3; */
  background-color: #0072B4;
}

.more.blue {
  font-size: 1em;
  font-weight: 600;
  line-height: 34px;
  padding: 10px 30px;
  color: #FFF;
  border: 1px solid #FFF;
}

.contact_data li {
  padding: 10px 0;
}

.contact_data li {
  padding: 10px 0 !important;
  color: #666;
  border-bottom: 1px solid #E0E0E0;
}

.text-smalt-blue {
  color: #4F8987;
}

h4 {
  font-size: 1em;
  margin: 1.33em 0;
  line-height: 20px;
}

p {
  line-height: 170%;
  font-size: 0.9em;
}
</style>
