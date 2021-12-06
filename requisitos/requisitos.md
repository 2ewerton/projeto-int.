 *<h1> Fenix Tecnologia <h1>*

 *<h3>- Dieta: </h3>* Este módulo vai contar com duas interfaces diferentes, onde a interface do profissional de nutrição irá alimentar uma lista com os tópicos de alimento, horário e quantidade.
 Na interface do paciente, irá aparecer todas as informações que foram passadas pela nutricionista ao mesmo, em contrapartida o paciente deverá alimentar a mesma lista, dizendo o que ele comeu em cada refeição, as quantidades e os horários. 

 *<h3>- Alarme: </h3>* Este módulo irá contar com duas interfaces diferentes, onde a interface do profissional de nutrição irá acrescentar horário para o paciente ingerir alimentos e água.
 Na interface do paciente, irá aparecer todas as informações que foram passadas pela nutricionista ao mesmo, em contrapartida o paciênte deverá alimentar a mesma lista,confirmando os horários ou alterando conforme sua disponibilidade.
 
 *<h3>- Acompanhamento de Peso: </h3>* Módulo que ajuda o usuário a compreender seus hábitos alimentares registrando as calorias consumidas. Vai possuir monitoramento de gordura, proteínas, carboidratos e colesterol.

 *<h3>- Gráfico de Evolução: </h3>* Gráfico que ficará disponível a ambos usuários que será alimentado pelas informações que o paciente inserir no aplicativo, como taxas de colesterol e glicose, calorias ingeridas e peso  atual.

 *<h3>- Atividade Física: </h3>* Neste módulo será opcional o uso do mesmo, se o profissional de nutrição julgar necessário a realização de exercícios físicos o mesmo poderá recomendar ao seu paciente, nele terá exercícios padrões e a opção de listar um outro exercício. Na interface do paciente ele poderá conferir quais exercícios foram recomendados para ele e também um exemplo de como o exercício é executado.

 *<h3>- Agendamento de consultas: </h3>* Módulo onde o paciente pode solicitar ao seu nutricionista uma consulta não prevista.

<h2> Documento de definição de requisitos </h2>

*<h3>Requisitos Funcionais</h3>*

Requisitos Func. | Descrição | Prioridade |Depende de|
|:-----------------:|:-----------:|:------------:|:----------:|
 RF 01 |Efetuar Cadastro| Alta|--|
 RF 02 |Efetuar Login| Média|RF 01|
 RF 03 |Atualização de cadastro| Média|RF 01 / RF 02|
 RF 04 |Primeiro acesso ( Questionário  )|Alta|RF 02|
 RF 05 | Menu com todas as funcionalidades do App|Alta |--|
 RF 06 |Criação e visualização de dieta|Alta|--|
 RF 07 |Estipulação de Horários|Alta|RF 06|
 RF 08 |Acompanhamento de peso|Média|--|
 RF 09 |Gráfico de Evolução|Média|RF 06 / RF 08|
 RF 10 |Atividade Física|Baixa|--|
 RF 11 |Agendamento de consultas|Médio|--|
 RF 12 |Efetuar LogOff|Alto|RF 01 / RF 02|


*<h3>Regras de Negócio</h3>*

Regras de Negócios| Descrição |Prioridade| Depende de.|
|:----------:|:-----------:|:------------:|:----------:|
 RN 01|O sistema deve conter autenticação de CEP e CPF|Alta|RF 01|
 RN 02|O sistema deve contar com um sistema ant-robô ( Captcha )|Alta|--|
 RN 03|O Sistema deve suportar um grande tráfego de pelo menos 1000 pessoas utilizando simultâneamente|Alta|--|
 RN 04|As informações guardadas em bancos de dados devem ser encriptadas|Alta|--|
 RN 05|As informações alteradas pelos usuários devem ser atualizadas no aplicativo em até 30 segundos|Média|--|
 RN 06|O sistema deve suportar informações sendo alteradas pelo Nutricionista e pelo paciente simultâneamente|Alta|--|
 RN 07|O sistema deve contar com interface Web e Mobile ( Rodar em diferentes navegadores como Chrome, Vivaldi, Opera. E sistemas Mobile como Android e IOS)|Alta|--|
 RN 08|Deverá existir a função de excluir todas as informações de usuário do sistema|Alta|--|
 RN 09|Senhas de usuários deverão contar com caracteres, numerais e símbolos, totalizando pelo menos 8 dígitos na senha|Alta|--|

*<h3>Requisitos não funcionais</h3>*
Requisitos Não F. | Descrição |  Categoria |  Escopo  |Prioridade| Depende de. |
:-----------------: |:-----------:|:------------:|:----------:|:----------:|:------------:|
 RNF 01|As Informações cadastradas deverão ser guardadas em um banco dados protegido por criptografia|Segurança de acesso|Sistema|Alta|RN 01|
 RNF 02|Informações cadastradas devem ser guardadas de forma criptografada nos bancos de dados do app|Segurança de acesso|Sistema|Alta|RF 02|
 RNF 03|O sistema deve oferecer a opção de leitura, alteração e exclusão de informações cadastradas|Segurança de dados|Funcionalidade|Alta|RF 03|
 RNF 04|Sistema deve apresentar um questionário inicial contendo algumas informações no primeiro acesso|Usabilidade|Sistema|Média|RF 04|
RNF 05|O Sistema deve conter funcionalidades diferentes nas interfaces do profissional e do  paciente.|Interoperabilidade|Sistema|Alta|--|
 RNF 06|O sistema deverá contar com gráficos e dashboard para os usuários acompanharem sua evolução|Usabilidade|Sistema|Média|RF 09|
 RNF 07|O sistema deverá ter um menu com recomendações de exercícios físicos que possam corroborar com as dietas estipuladas|Usabilidade|Funcionalidade|Baixa|--|
 RNF 08|O sistema vai contar com a opção de marcar consultas online ou presenciais fora de agenda.|Atratividade|Funcionalidade|Média|--|
 RNF 10 |O sistema deve permitir aos usuários estarem efetuando LogOff do sistema perdendo assim todos os acessos às informações confidenciais.|Segurança de informação|Sistema|Alta|RF 12 |


*<h3>Prototipação de telas</h3>*

Campo|Tipo|Tamanho|
:--:|:-------:|:--:|:--------:|
Cadastro|Vai conter campos
